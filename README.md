
# Chat_App_Doogle
## Description of the Project
This chat application DOOGLE helps one effortlessly  communicate with people anywhere in the world by sending and receiving messages in real time.This project provides the instant communication functionality between users. The users have the capability to do one to one communication and also they can communicate with in groupwhich is the most fascinating feature of this app. As a cherry on the top, the  User Authentication feature of this project boosts up its reliability of the users on DOOGLE.


## Deployment

To deploy this project after cloning,  run

```bash
  node backend/server.js
```

Otherwise just click

  [DOOGLE](https://chat-app-doogle.vercel.app/)



## Technologies Used

Express version 4.18.2  
React version 18.2.0  
Mongoose version 6.7.2  
Nodemon version 2.0.20  
Socket.io version 4.5.4
## API Reference

#### Register User

```http
  POST /api/user/
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `User details` | `json` | Takes the User data to the Database |

#### To login

```http
  GET /api/user/login
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `User Details`      | `json` | fetch the User Details from the Database |

#### Searching the Doogle Registered Users  

```http
  GET /api/user?search=
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `User Id`      | `json` | Checks for the Id in the Database of Doogle |

#### Fetching Chats of a User

```http
  GET /api/chat
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `User chat`      | `json` | It fetches the whole chat of a User  |

#### Accessing Chats of a User

```http
  GET /api/chat
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `User chat`      | `json` | It helps to get access to the chat of the User  |

#### To create a group

```http
  POST /api/chat
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `Users and Group name `      | `json` | It helps to create the group in the app  |

#### To rename the name of the group

```http
  PUT /api/chat
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `Chat Id and Chat name `      | `json` | To rename the group name  |

#### To send a message 

```http
  POST /api/message 
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `content of the message `      | `json` | Sending of the messages  |

#### To receive the messsage 

```http
  GET /api/message:chatId
```

 | Type     | Description                       |
 | :------- | :-------------------------------- |
 | `json` | fetching all messages of the selected chat  |


## Features

- Real time messeges
- Sign up and Sign in for users
- Fullscreen mode
- Push Notifications
- Responsive layout
- Group Chat feature to form community


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`MONGO_URI`

`JWT_SECRET`

`NODE_ENV`


## Tech Stack

**Client:** React, Chakra UI, Socket.io-client

**Server:** Node, Express, Socket.io


## Screenshots

The Sign up page 

[![Chat-App-1.jpg](https://i.postimg.cc/QMQK9sNd/Chat-App-1.jpg)](https://postimg.cc/TyP3FzWz)

The login page

[![Chat-app-2.jpg](https://i.postimg.cc/cH1Cvn5F/Chat-app-2.jpg)](https://postimg.cc/wtPgP7zN)

Chatting Interface

[![Chat-App-4.jpg](https://i.postimg.cc/ZKNbKH5T/Chat-App-4.jpg)](https://postimg.cc/w768whNP)
## Acknowledgements

 - [React JS](https://reactjs.org/docs/getting-started.html)
 - [Node JS](https://nodejs.org/dist/latest-v19.x/docs/api/)
 - [Express JS](https://expressjs.com/en/guide/routing.html)
 - [Mongoose ](https://mongoosejs.com/docs/guide.html)
 - [Chakra UI ](https://chakra-ui.com/getting-started)

