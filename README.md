This project is the final project for the Udacity FSND

The project is about a casting agency. This includes having actors and movies and assigning actors to movies. 

This project has two models/tables: A movie table that holds all the movies and an actors table that holds all the actors. For each movie, there are many actors so there is a one to many relationship there. 

To login or set up an account, go to the following url: 

https://abhkar.auth0.com/authorize?audience=casting&response_type=token&client_id=fFG0Rk7761WnCS9DBeKWnxbQ11OsDK0R&redirect_uri=https://abhkar1.herokuapp.com/login-results

There are three roles within the API. 

1) Casting Assistant 
2) Casting Director and 
3) Executive Producer. 

The logins for the three roles has been provided in the separate notes 

The url for the API:
https://abhkar1.herokuapp.com/

The endpoints are : 

GET '/movies'
    This endpoint fetches all the movies in the database and displays them as json 

GET '/actors'
    This endpoint fetches all of the actors in the databse and displays them as json 

POST '/movies/create'
    This endpoint will create a new movie in the database based on the json which is in the body of the request 

POST '/actors/create'
    This endpoint will create a new actor in the database based on the json which is in the body of the request 

DELETE '/movies/delete/int:movie_id'
    This endpoint will delete the movie that corresponds to the movie ID which is passed into the url 

DELETE '/actors/delete/int:actor_id'
    This endpoint will delete the actor that corresponds to the actor ID which is passed into the url 

PATCH '/actors/patch/int:actor_id' 
    This endpoint will modify the actor that corresponds to the actor ID which is passed into the url based on the json that is passed into the body of the request 

PATCH '/movies/patch/int:movie_id'
    This endpoint will modify the movie that corresponds to the movie ID which is passed in the url based on the json that is passed into the body of the request