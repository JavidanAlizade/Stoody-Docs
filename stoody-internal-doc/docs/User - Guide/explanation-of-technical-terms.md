# Explanation of Technical Terms
Here are some key technical terms used in Stoody:

**Node.js:** A runtime environment that allows JavaScript to run on the server-side, enabling backend functionality.

**MongoDB:** A NoSQL database that Stoody uses to store and manage data such as courses, user profiles, and progress.

**API (Application Programming Interface):** A set of rules and definitions that allows applications to communicate with each other. Stoody’s backend provides a REST API for the frontend to fetch data.

**REST API:** A set of functions that allow Stoody to communicate with other applications via HTTP requests. These functions are exposed through endpoints.

**Frontend:** The part of Stoody that users interact with directly (the dashboard, settings, etc.). It's built using web technologies like HTML, CSS, and JavaScript.

**Backend:** The server-side part of Stoody that handles data processing, database interactions, and API requests. It is built using Node.js and connects to MongoDB.

**PM2:** A process manager that ensures Stoody’s backend runs continuously, even if the terminal is closed or the server restarts.

**CRUD Operations:** Create, Read, Update, Delete operations commonly used in APIs. Example: GET /api/courses retrieves all courses, and POST /api/courses creates a new course.

**CORS (Cross-Origin Resource Sharing):** A security feature that controls which domains can access backend resources. This is managed using the cors module in Express.js.

**WebSockets:** A protocol for real-time communication between a client and a server. Useful for features like live chat, notifications, and real-time updates.

**Authentication vs. Authorization:**

   Authentication verifies who a user is (e.g., login with email and password).

   Authorization determines what a user can do (e.g., admin access vs. regular user access).

**CI/CD (Continuous Integration & Continuous Deployment):** A process that automates testing and deployment of applications to ensure faster and more reliable releases.

**Docker & Containers:** A containerization tool that packages applications and their dependencies to ensure they run consistently across different environments.

**Webhooks:** A mechanism that allows services to send real-time updates to other applications when a specific event occurs (e.g., Stripe sending a webhook when a payment is completed).

**Middleware:** A software layer that processes requests before they reach the main application logic. Common examples include authentication middleware and logging middleware.

**Rate Limiting:** A security feature used to limit the number of API requests a user or IP address can make in a given period, preventing abuse.

**OAuth 2.0 & OpenID Connect:** Protocols used for secure authentication and authorization, allowing users to log in using third-party services like Google, Facebook, or GitHub.