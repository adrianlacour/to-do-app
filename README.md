# Go To Do App

This is a to-do list application.

## Stack

### Backend
* [Golang](https://golang.org/)
* HTTP request multiplexer [Gorilla](https://github.com/gorilla/mux)
* Environment variable loader [godotenv](https://github.com/joho/godotenv)
* Go [MongoDB driver](go.mongodb.org/mongo-driver) 
* [MongoDB](https://www.mongodb.com/)

### Front-end
* [Javascript](https://www.javascript.com/)
* Javascript UI library [React](https://reactjs.org/)
* [Semantic-ui-react](https://react.semantic-ui.com/)

---

## Getting started

### Install requirements

1. Install [golang](https://golang.org/dl/)
1. Install the gorilla/mux package for routing `go get -u github.com/gorilla/mux`
1. Install the mongo-driver package to connect with MongoDB `go get go.mongodb.org/mongo-driver`
1. github.com/joho/godotenv to access the environment variable. `go get github.com/joho/godotenv`

### Create the React client

From the base application directory:

`create-react-app client`

### Start the application

1. Start your MongoDB instance. `mongod --dbpath /usr/local/var/mongodb --logpath /usr/local/var/log/mongodb/mongo.log --fork`
1. Create a `.env` file inside the `go-server` and copy the keys from `.env.example` and update the **DB_URI** field.
1. From go-server directory, open a terminal and run:
   `go run main.go`
1. From the client directory,  
   a. Install all of the dependencies. `npm install`  
   b. Start the client. `npm start`
1. Open the application at http://localhost:3000

## Walkthrough

### Base page

![]()

### Create tasks

In the input field, enter a task and press **Enter**.

![]()

### Complete Task

On completion of a task, select **Done** on the task card.

![]()

Upon completion of the task, the card's bottom line color changes from yellow to green.

### Undo a task

To undo a copmleted task, select on **Undo** on the task card.

![]()

Upon undoing copmletion of the task, the card's bottom line color changes from green to yellow.

### Delete a task

To delete a task, select **Delete** on the task card.

![]()

---

# License

[MIT License](https://github.com/adrianlacour/to-do-app/blob/main/LICENSE)

Copyright (c) 2021 Adrian LaCour