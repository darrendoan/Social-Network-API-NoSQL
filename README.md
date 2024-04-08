# Social-Network-API-NoSQL

## Description
This is another homework submission for the USYD Coding Bootcamp. In this challenge, we were tasked with creating a RESTful API that allows a social media markup to perform CRUD operations on users, thoughts and reactions aswell as allowing them to add friends using a NoSQL Database. The data models include friends, users, thoughts, and reaction data models, and they can be retrieved by ID or all of them. This API is built using Node.js and Mongoose, and it provides a simple and scalable way to handle social networking data without the restrictions of traditional relational databases.

# Overview

## The Challenge
The challenge for this assignment was to create a RESTful API that allows a social media markup to perform crud operations on users, thoughts and reactions. The API must be built using Node.js, mongoose and must be able tp provide endpoints on large amounts of unstructured data.

The API must allow users to: 
 - Create and delete user accounts
 - Create, read, update and delete thoughts
 - Add and remove reactions to thoughts
 - Add and remove friends to a user's friend list

To test this API I used insomnia to send HTTP requests to the API endpoints to verify that the responses were correct. You can use any other similar tool to do this too, I just prefer Insomnia. 

## User Story 
```md 
AS A social media startup
I WANT an API for my social network that uses a NoSQL database
SO THAT my website can handle large amounts of unstructured data
```

## Acceptance Criteria
```md
GIVEN a social network API
WHEN I enter the command to invoke the application
THEN my server is started and the Mongoose models are synced to the MongoDB database
WHEN I open API GET routes in Insomnia for users and thoughts
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia
THEN I am able to successfully create, update, and delete users and thoughts in my database
WHEN I test API POST and DELETE routes in Insomnia
THEN I am able to successfully create and delete reactions to thoughts and add and remove friends to a user’s friend list
```

## Usage Instructions
1. Clone or Fork this repository
2. Create a .env file in the root directory of the project 
3. Open intergrated terminal in the root directory and type in `npm start`
4. Once the server is running, use insomnia to test http://localhost:3001 with the following route endpoints: GET, POST, PUT and DELETE  

### Availiable Endpoints
Each endpoint must include the necessary data in the request body or URL parameters as specified in the acceptance criteria.

GET /api/users - get all users
GET /api/users/:userId - get a single user by ID
POST /api/users - create a new user
PUT /api/users/:userId - update a user by ID
DELETE /api/users/:userId - delete a user by ID
GET /api/thought - get all thought
GET /api/thought/:thoughtId - get a single thought by ID
POST /api/thought - create a new thought
PUT /api/thought/:thoughtId - update a thought by ID
DELETE /api/thought/:thoughtId - delete a thought by ID
POST /api/thought/:thoughtId/reactions - add a reaction to a thought
DELETE /api/thought/:thoughtId/reactions/:reactionId - remove a reaction from a thought
POST /api/users/:userId/friends/:friendId - add a friend to a user's friend list
DELETE /api/users/:userId/friends/:friendId - remove a friend from a user's friend list

## Video Link
https://app.screencastify.com/v3/watch/nyYstOm4aZXTRhHxcBPR 

## Contact
Github : https://github.com/darrendoan/Social-Network-API-NoSQL
