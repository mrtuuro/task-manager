# Welcome to Tas-Manager API! 

With this API you can create a list that contains your **to-do**s. For now API does not include a Web GUI though it is in progress!

## --> How to use <--

You will need an API testing application like 'Postman'. So that you can send requests to server and also get responses back.

## --> Requests <-- 

### url = https://tuuro-todoapp.herokuapp.com/

> Create user 
- **POST** --> {{url}}/users
- Send a request that JSON body with --> "name", "email", "password"

> Create task 
- **POST** --> {{url}}/tasks
- Send a request that JSON body with --> "description", "completed"

> Login user 
- **POST** --> {{url}}/users/login
- Send a request that JSON body with --> "email", "password"

> Logout user 
- **POST** --> {{url}}/users/logout

> Logout All 
- **POST** --> {{url}}/users/logoutAll

> Upload avatar 
- **POST** --> {{url}}/users/me/avatar
- Send a request with key "avatar" and value that is chosen by you from your computer.

> Read profile 
- **GET** --> {{url}}/users/me

> Read tasks
- **GET** --> {{url}}/tasks
- key=sortBy, value=createdAt:asc || value=createdAt:desc

> Update user 
- **PATCH** --> {{url}}/users/me
- You can udate you profile credentials.

> Update task
- **PATCH** --> {{url}}/tasks/<taskID>
- You can update your task.
  
> Delete user 
- **DELETE** --> {{url}}/users/me
  
> Delete task
- **DELETE** --> {{url}}/tasks/<taskID

> Delete avatar
- **DELETE** --> {{url}}/users/me/avatar
