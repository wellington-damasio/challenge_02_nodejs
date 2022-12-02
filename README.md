# Challenge 02 - Node.js (Rocketseat - Ignite)

## What is this?
This is a basic todo list API

## What was the challenge?
Given a code template with express routes with the functionality of each route already written, I had to write the middleware functions those routes were dependent on in order for the API to work.

There were 3 middleware functions I was supposed to wrote:
1. `checksExistsUserAccount()` - A function that receives an username as a header parameter and has to check in the users array if any user with that username exists, then return a response or the `next()` function accordingly
2. `checksCreateTodosUserAvailability()` - The API has a 'premium' functionality were users using the free plan can create only 10 todos. Basically this function checks if the user is in the free plan and if he/she has 10 todos and responds with an status `403` or `next()`
3. `checksTodosExists()` - Basically I had to write three validations and pass user information to the route function (`next()`) if the data received by this middleware passes all validations. **The validations were**:
- Check if user exists based on a username received by header parameters
- Check if the todo id received by route parameters is an valid `UUID`
- Check if a todo exists comparing the todo id received by route parameters if the ids of the user todos

Some of the functionalities of the API are:
- Create, read, update, delete todos
- Create an user accont
- Change done property of the todos from `false` to `true`

## What I learned with this challenge?
- How to write my own middlewares to make code clean and concise
- Better understanding of the `CRUD` functionalities of an API
- How to read and deal of tests when it comes to backend development
- How to validate an `UUID`
- I learned a lot about JavaScript 'new' array methods like `Array.some()` and `Array.find()`
