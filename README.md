# kaiburrTask1

Use Doc-task1 file to get all apis, input and output

# Java REST API Application for Server Management

This project involves implementing a Java application that provides a REST API for managing server objects, utilizing MongoDB as the database. The application includes endpoints for searching, creating, and deleting server objects.

## Endpoints

### GET /servers

- Returns all servers if no parameters are passed.
- Returns a single server or 404 if the server ID is provided and no such server exists.

### PUT /server

- Adds a new server using the server object provided in a JSON-encoded message body.

Example:
```json
{
  "name": "my centos",
  "id": "123",
  "language": "java",
  "framework": "django"
}
```
DELETE /server/:id
Deletes a server based on the provided server ID.

Database
The server objects are stored in a MongoDB database.

Usage
Clone the repository.
Open the project in IntelliJ.
Ensure MongoDB is installed and running on the specified port (8070).
Run the application to start the server.
Use an HTTP client like Postman or cURL to interact with the API and test the endpoints.
