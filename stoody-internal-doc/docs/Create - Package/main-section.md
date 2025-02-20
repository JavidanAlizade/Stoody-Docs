# Main Sections of `package.json`

## Metadata
Metadata is data that provides information about other data. It describes the characteristics, attributes, and context of a resource or data set, making it easier to understand, manage, and use that data.
Here are the main metadata fields typically found in a package.json:

**Name:** The name of the project or package.

**Example:**

``` js 
"name": "stoody-turborepo"
```

**Version:** The version number of the project, usually following semantic versioning.

**Example:**

``` js
"version": "0.1.0"
```

**Description:** A short description of what the project does.

**Example:**

``` js
"description": "A simple app for demonstrating package.json"`
```

**Main:** The entry point for the project (typically the main TypeScript file).

**Example:**

``` js
"main": "index.ts"`
```

**Keywords:** A list of keywords related to the project, which can help others find it.

**Example:**

``` js
"keywords": ["turbo", "typescript", "react"]`
```

**Author:** The name of the author or maintainer of the package.

**Example:**

``` js
"author": "Orkhan GG"`
```

**Repository:** Specifies where the project's code is hosted (e.g., GitHub URL).

**Example:**

``` js title
"repository": "https://github.com/Stoody-LLC/stoody-turborepo/repo"`
```

**Engines:** Specifies which versions of Node.js the project is compatible with.

**Example:** 

``` js title
  "engines": {
    "node": ">=18"
  }
```

 ## Scripts
The scripts section contains commands to run the project, build it, and test it.

**dev:** Starts the project in development mode

**Example:**

``` js
"dev": "turbo dev"
```

**build:** Builds the project for production

**Example:**

``` js
"build": "turbo build"
```

**start:** Starts the production build of the project

**Example:**

``` js
"start": "next start"
```

You can run a script like this:

`pnpm turbo dev`


 ## Dependencies 

 **Dependencies are categorized into two sections:**

**Dependencies** – The packages required for the project to run in production.

**DevDependencies** – The packages needed only for development purposes.

**To add a new dependency:**

`pnpm install next`

This will automatically add it to the dependencies section:

**Example:**

``` js title
"dependencies": {
"next": "14.2.15"
}
```

**If you need a development-only dependency:**

`pnpm install eslint --save-dev`

This will add the package to the **devDependencies** section.
