# Stoody User Guide
## Introduction

This guide will walk you through the process of setting up **Stoody**, using the key features, and troubleshooting common issues.

## System Requirements
**Operating System:** Windows 10 or macOS 10.14+

**Web Browser:** Google Chrome (latest version), Mozilla Firefox (latest version)

**Node.js:** Version 18.0 or above

**MongoDB:** Required for local database setup (if using a local instance)

## Installation

### 1. Clone the Repository
   Clone the Stoody repository from GitHub to your local machine:

`git clone https://github.com/Stoody-LLC/stoody-turborepo`

`cd stoody`

### 2. Install Dependencies
   To install the necessary dependencies for both the frontend and backend, run:

`npm install`

#### Backend Setup and Build
Before you can start the Stoody backend, you need to build it first.

#### Build the Backend
If you are using TypeScript for the backend, first compile the TypeScript code to JavaScript.

`npm run build`

This will create the compiled production code in the `dist/` folder.

### 3. Run the Application
   Once the setup is complete, run the development server:

`npm run dev`
The app will be available at http://localhost:3000/ for the frontend and http://localhost:8080/ for the backend.
