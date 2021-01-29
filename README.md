# Go To Do App

This is a to-do list application.

**Server: Golang  
Client: React, semantic-ui-react  
Database: Local MongoDB**

---

## Application Requirement

### golang server requirement

1. golang https://golang.org/dl/
2. gorilla/mux package for router `go get -u github.com/gorilla/mux`
3. mongo-driver package to connect with mongoDB `go get go.mongodb.org/mongo-driver`
4. github.com/joho/godotenv to access the environment variable.

### react client

From the Application directory

`create-react-app client`

## :computer: Start the application

1. Make sure your mongoDB is started
2. Create a `.env` file inside the `go-server` and copy the keys from `.env.example` and update the DB connection string.
3. From go-server directory, open a terminal and run
   `go run main.go`
4. From client directory,  
   a. install all the dependencies using `npm install`  
   b. start client `npm start`

## Walk through the application

Open application at http://localhost:3000

### Index page

![]()

### Create task

Enter a task and Enter

![]()

### Task Complete

On completion of a task, click "done" Icon of the respective task card.

![]()

You'll notice on completion of task, card's bottom line color changed from yellow to green.

### Undo a task

To undone a task, click on "undo" Icon,

![]()

You'll notice on completion of task, card's bottom line color changed from green to yellow.

### Delete a task

To delete a task, click on "delete" Icon.

![]()

---

# License

[MIT License](https://github.com/adrianlacour/to-do-app/blob/main/LICENSE)

Copyright (c) 2021 Adrian LaCour