# TASKLY-API-TESTING-PROJECT
This project involves API testing for the **Taskly** application using Postman. The purpose of this collection is to validate core functionalities of the Taskly backend, such as user authentication and task management.

## 📁 Project Structure

The Postman collection includes the following endpoints:

### 🧑‍💻 Authentication
- **Sign Up**: `POST /api/v1/auth/sign-up`  
  Create a new user account.

- **Sign In**: `POST /api/v1/auth/sign-in`  
  Authenticate the user and retrieve a JWT token.

### ✅ Task Management
- **Create Task**: `POST /api/v1/tasks`  
  Create a new task with subtasks and tags (Requires Bearer Token).

- **Get User Tasks**: `GET /api/v1/tasks/user/:userId`  
  Fetch all tasks associated with a specific user.

- **Get a Single Task**: `GET /api/v1/tasks/:taskId`  
  Retrieve details of a single task by task ID.

- **Update Task**: `PATCH /api/v1/tasks/:taskId`  
  Update a task including status, title, subtasks, and other metadata.

- **Delete Task**: `DELETE /api/v1/tasks/delete/:taskId`  
  Remove a task permanently by ID.

## 🔐 Authorization

All task-related routes require a Bearer Token (JWT) returned from the **Sign In** endpoint. Add the token to the `Authorization` header in Postman:

```
Authorization: Bearer <your_token>
```

## ✅ Test Scenarios Covered

- User registration and login flow
- Creating tasks with multiple subtasks
- Retrieving all tasks of a user
- Fetching individual task details
- Updating task properties such as title, status, and tags
- Deleting a task

## 🌐 Base URL

```
https://tasklybe.vercel.app/api/v1
```

## 🧪 Tools Used

- **Postman**: API test automation and environment simulation
- **JWT**: For secure user session management
- **Vercel**: Hosting the backend

## 🧑‍🎓 Author

**Vasantharaja V**  
Email: [vasantharajavijayakumar@gmail.com](mailto:vasantharajavijayakumar@gmail.com)  
LinkedIn: [linkedin.com/in/vasantharaja04](https://linkedin.com/in/vasantharaja04)

## 📎 Postman Collection Link

[Click here to view the Postman collection](https://vasanth-4707298.postman.co/workspace/vasanth's-Workspace~279551e5-5b89-4bc5-8013-7381002ec747/collection/45401203-069b066e-d4b2-4f0e-992d-4894c6617990?action=share&source=collection_link&creator=45401203)

