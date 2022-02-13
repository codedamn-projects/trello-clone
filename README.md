# Codedamn Projects - Trello Clone

![header image](https://raw.githubusercontent.com/codedamn-projects/trello-clone/master/designs/Moving%20Cards.gif)
## Hello developer!

Welcome to Trello Clone Project on Codedamn. This is one of the many projects available on [codedamn](https://codedamn.com/projects) to reinforce your learning by building. If you want to become a full stack developer and learn by practicing, feel free to attempt this challenge. Feel free to check out the codedamn [Full Stack Web Development Learning Path](https://codedamn.com/learning-paths/fullstack) to learn more about how to become an awesome full stack developer.

## Project Overview

You have to build a functional Kanban board system where the user can Drag and Drop Cards between lists. 

## Instructions

Your challenge is to build out this project and get it looking as close to the design as possible.

You can use **any tools or technologies** you like to help you complete the challenge. So if you've got something you'd like to practice, feel free to give it a go.

Your project should:

-   Be responsive for desktop and mobile phones
-   Have minimum functionalities and effects working

Want some support on the challenge? [Join our discord community](https://cdm.sh/discord) and ask questions in the **#general** channel.

There is no limit you can go beyond the mentioned criteria and create additional functionalities

### Landing Page

At `/` route.

![landing page](https://raw.githubusercontent.com/codedamn-projects/trello-clone/master/designs/Home.png)

### Login

The login functionality should be implemented in the `/login` route.

![login image](https://raw.githubusercontent.com/codedamn-projects/trello-clone/master/designs/Login%20%5BDesktop%7D.png)

When the user clicks on the Log In button the a POST request should be sent to `api/login` to validate the user credentials. If the user exists and has entered the correct data, you should redirect to `/boards` page. 

### Signup

At `/signup` route.

![Sign UP page]()

### Boards
At `/boards` route

![/boards](https://raw.githubusercontent.com/codedamn-projects/trello-clone/master/designs/Board%20%5BDesktop%5D.png)
### Board

## API Routes 

### `/api/auth/login`

To verify the user credentials on Sign In, taking the parameters as the roll number and the password 

### `/api/auth/register` 

To register a new student and add the document to the database

### `/api/messages` 

 To get the previous messages in the conversation. Make sure to pass in the Conversation ID to retrieve the messages 

 ### `/api/conversations`

 To list out all the open conversations on the chat application. 


### MongoDB User document
```
{ 
    "username" : string,
    "email" : string,
    "password" : string
}
```

### MongoDB Message document
```
{
    "conversationId" : string,
    "sender" : string, 
    "message" : string
}
```
Take a look at the mongoose schema to get the perfect Idea. 

### MongoDb Conversation document
```
{
    "conversationId" : string,
    "members" : array
}
```

### Ports 
The Codedamn Playgrounds exposes only `1337` and `1338` ports on the internet. So you'll be using `localhost` for connecting to the mongodb instance as they are hosted on the same docker container. You can specify it as `localhost:27017` or simple write `localhost`. 

You have to use the `1338` port for the web socket connection. 

You are free to use any third party libraries for the web sockets or any other part of the application. 

To understand about web sockets, you can refer to this [blog](https://codedamn.com/news/backend/what-are-web-sockets-how-is-it-different-from-http)
## Recommended Technologies 

1. Mongoose for mongodb object modelling and effective type system 
1. Tailwind CSS for User Interface






## Where to find everything

Your task is to build out the project as per the provided screenshots.

The designs are in image formats can be found in `/designs`.



## Send feedback!

We love receiving feedback! We're always looking to improve our challenges and our platform. So if you have anything you'd like to mention, please visit [codedamn feedback page](https://codedamn.com/contact)