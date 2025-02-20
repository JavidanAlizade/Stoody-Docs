# What's package.json
The `package.json` file is the main configuration file used in Node.js and Next.js projects.
It stores essential information such as project dependencies, scripts, and metadata.



## How to Create a package.json file?
 ## 1.Create Automatically

To create a `package.json` file, run the following command in the terminal:

`pnpm init`

This command will prompt you with questions about your project, such as its **name, version, description**, etc.
If you want to create it with default values without answering any questions, you can use:

`pnpm init -y`

This will generate the `package.json` file with default settings.

 ## 2.Create Manually
Create Manually
If you prefer to create the package.json file manually:

Open your project folder and create a new file named package.json.
Add the following content to the file:

```json
{ 
  "name": "stoody-turborepo",
  "private": true,
  "scripts": {
  "build": "turbo build",
  "build:backend": "turbo run build --filter=backend",
  "build:web": "turbo run build --filter=web",
  "build:packages": "turbo run build --filter=@repo/*",
  "dev": "turbo dev",
  "dev:web": "turbo dev --filter=web",
  "dev:backend": "turbo dev --filter=backend",
  "lint": "turbo lint",
  "clean": "turbo clean",
  "format": "prettier --write \"**/*.{ts,tsx,md}\""
  },
  "devDependencies": {
  "prettier": "^3.2.5",
  "turbo": "^2.3.3",
  "typescript": "5.5.4"
  },
  "packageManager": "pnpm@9.0.0",
  "engines": {
  "node": ">=18"
  }
}
```