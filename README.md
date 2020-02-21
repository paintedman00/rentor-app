# Rentor

A rental movie app created using NodeJS, Express and MongoDB with authentication and authorization.

There is a rentor-postman-collection-api with in the files for execution .

API end points :
==============
POST /api/users : you can create a new user. accept a body parameter (name, email, password)

POST /api/auth : you need to authenticate a registered user and get a valid token. accept a body parameter (email, password)

POST /api/genres : user can create a new genre. accept a body parameter (name)

POST /api/movies : user can create a new movie. accept a body parameter (title, genreId, numberInStock, dailyRentalRate)

POST /api/customers : user can create a new customer. accept a body parameter (name, isGold, phone)

POST /api/rentals : user can create a new rentals. accept a body parameter (customerId, movieId)

GET /api/users/me: will give all current user stored in database that need a valid jsonwebtoken.

GET /api/genres: will give all genres stored in database.

GET /api/movies: will give all movies stored in database.

GET /api/customers: will give all users stored in database.

GET /api/rentals: will give all users stored in database.

PUT /api/customers/<customer_id>: update a customer completely. accept a body parameter(name, isGold, phone)

PUT /api/genres/<genres_id>: update a genres completely. accept a body parameter (name)

PUT /api/movies/<movies_id>: update a movies completely. accept a body parameter (title, genreId, numberInStock, dailyRentalRate)

DELETE /api/customers/<customer_id>: delete a customer completely

DELETE /api/genres/<genres_id>: delete a genres completely

DELETE /api/movies/<movies_id>: delete a movies completely
