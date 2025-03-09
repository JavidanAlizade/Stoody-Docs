# What's repository
**Repository** is a place where a project’s source code, documentation, and other necessary resources are stored. Using version control systems (VCS) like Git, it is possible to track and manage code changes.

# Mono Repository
**Mono repository** is a single codebase that hosts multiple projects used by the same organization or team.

## Advantages:
- Easier code reuse.
- Seamless integration between projects.
- Easier to maintain version compatibility.
- Centralized CI/CD (Continuous Integration/Continuous Deployment).

# Turborepo
**TurboRepo** is a high-performance monorepo tool designed for Node.js and JavaScript projects. It optimizes monorepo structures to improve code reusability and performance.

## Features of TurboRepo:
Designed for monorepo structures, it supports package managers like pnpm, yarn, npm, and bun. With its cloud service, build results can be shared across devices.

### Installation:
```sh
npm install -g turbo
```

### Creating a Project with TurboRepo:
```sh
npx create-turbo@latest my-monorepo
cd my-monorepo
```

### turbo.json Configuration:
TurboRepo’s configuration is stored in the `turbo.json` file:
```json
{
  "tasks": {
    "build": {
      "env": [
        "ALLOWED_ENVIRONMENT_KEYS",
        "AUTH_PUBLISHABLE_KEY",
        "AUTH_SECRET_KEY",
        "CLERK_WEBHOOK_SIGNING_SECRET_USER_CREATED",
        "AWS_REGION",
        "AWS_ACCESS_KEY_ID",
        "AWS_SECRET_ACCESS_KEY",
        "FILE_SERVICE_UPLOAD_STANDARD_MISC_FILES_BUCKET_NAME",
        "FILE_SERVICE_CLOUDFRONT_DOMAIN_NAME",
        "RTC_HOST",
        "RTC_API_KEY",
        "RTC_SECRET_KEY",
        "FILE_SERVICE_ENCRYPTION_KEY",
        "STRIPE_SECRET_KEY",
        "STREAM_API_SECRET",
        "NEXT_PUBLIC_STREAM_API_KEY",
        "WS_API_KEY",
        "OPENAI_API_KEY",
        "MONGODB_URI"
      ]
    }
  },
  "extends": ["//"]
}

```
