
## Endpoints and Methods (GET, POST, PUT, DELETE)

**POST** /api/users: Adds a new user

**GET** /api/users/{id}: Retrieves user data

**PUT** /api/users/{id}: Updates user data

**DELETE** /api/users/{id}: Deletes a user

## Request and Response JSON Structures:
### POST /api/users:
```json
{
"name": "John Doe",
"email": "johndoe@example.com"
}
```
### Response:
```json 
{
"id": "123",
"name": "John Doe",
"email": "johndoe@example.com"
}
```

### HTTP Response Codes:

200: Successful operation
400: Bad request
500: Server error
