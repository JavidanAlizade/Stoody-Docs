# Problem Solving
## Issue 1:
### The application is not running.
### Solution:

Ensure all environment variables are correctly set, especially the database connection URL (DATABASE_URL).
If you're using MongoDB locally, make sure it's running. If MongoDB is not installed, follow the MongoDB installation guide for your platform.


## Issue 2:
### I can’t access the backend API.
### Solution:

Ensure the backend server is running on the correct port (http://localhost:8080/).
If it's not running, navigate to the backend directory and start the server using npm start.
If the server is running, but you're still facing issues, check the backend logs for any errors.


## Issue 3: 
### The app is slow or unresponsive.
### Solution:

Check your system's resources (CPU and memory) to ensure they are not overburdened.
If running the app on a server, ensure the server meets the necessary specifications.
Optimize the code and reduce the number of unnecessary API requests that could be slowing the system down.

## Issue 4: 
### Backend API requests return "403 Forbidden"
### Solution:

Ensure the backend has CORS configured properly:

``` json
const cors = require('cors');
app.use(cors({ origin: '*' }));
```

Check if the API requires an Authorization header. If using JWT authentication, ensure the token is correctly included in requests.

## Issue 5:
### MongoDB connection fails:
Backend startup logs show "MongoNetworkError: failed to connect to server".
### Solution:

Check if MongoDB is running:

`sudo systemctl status mongodb`

If using Docker, ensure the container is running:

`docker ps`

Verify the `DATABASE_URL` in `.env` is correct.

## Issue 6:
### Backend server stops running when the terminal is closed.

### Solution:

Use pm2 to keep the backend running:

```
pm2 start server.js --name stoody-backend
pm2 save
pm2 startup
```