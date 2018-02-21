# Twitter app back-end

## Stack

  - Twitter API
  - Postman //testing tool
  - Redis //access token storage
  - MongoDB //noSQL database
  - Express //API server
  - RabbitMQ //messaging

## Structure

  - server
    - config
    - models
        - user
        - post
    - controllers
        - auth
        - post
    - view
    - index.js
    - package.json
    - router.js

## API calls

- Registration
POST /user {login, pass}
- Login
PUT /user/#id {login, pass}
- Get tweet with #id
GET /tweet/#id [AUTH]->(text)
- Get all tweets
GET /wall [AUTH]->([text])
- Post new tweet
POST /tweet [AUTH] (text)
