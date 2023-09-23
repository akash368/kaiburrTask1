# kaiburrTask1

## Use Doc-task1 file to get all API's endpoint, input and output screenshot.

# Java REST API Application for Server Management

This project involves implementing a Java application that provides a REST API for managing server objects, utilizing MongoDB as the database. The application includes endpoints for searching, creating, and deleting server objects.

## Endpoints

### GET /user/

- Returns all servers if no parameters are passed.
- Returns a single server or 404 if the server ID is provided and no such server exists.

### POST /user/ 

- Adds a new server using the server object provided in a JSON-encoded message body.

### PUT /user/upadate/:id

- Update an existing user by using the given userID.
  
Example:
```json
{
    "id": "6",
    "name": "Akash",
    "language" : "PHP",
    "framework" : "Larvel"
}
```

### GET /user/usersName/:name
- Finds server(s) based on a provided string for the server name.
- Returns one or more servers found that contain the specified string.
- Returns 404 if no servers are found.

### DELETE 
-/user/delete:id
Deletes a server based on the provided server ID.

### Database
-The server objects are stored in a MongoDB database.

### Usage
-Clone the repository.
-Open the project in IntelliJ.
-Ensure MongoDB is installed and running on the specified port (8070).
-Run the application to start the server.
-Use an HTTP client like Postman or cURL to interact with the API and test the endpoints.
