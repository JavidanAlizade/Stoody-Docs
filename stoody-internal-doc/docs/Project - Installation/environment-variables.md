# Environment Variables
**Environment variables** allow applications to define different configurations based on the environment they are running in.

## .env 
The `.env` file is used to store sensitive and configurable information in projects.

Example:
``` sh
DATABASE_URL=mongodb://localhost:27017/mydb
API_KEY=123456789abcdef
```

### Reading in JavaScript and Node.js:
```js
require('dotenv').config();
console.log(process.env.DATABASE_URL);
```

### Adding in Next.js:
In Next.js, environment variables are added to the `.env.local` file:
``` md
NEXT_PUBLIC_API_URL=https://api.example.com
```

Then, they can be accessed using `process.env.NEXT_PUBLIC_API_URL`.
