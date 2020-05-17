This project is the final project for the Udacity FSND

The project is about a casting agency. This includes having actors and movies and assigning actors to movies. 

This project has two models/tables: A movie table that holds all the movies and an actors table that holds all the actors. For each movie, there are many actors so there is a one to many relationship there. 

To login or set up an account, go to the following url: 

https://abhkar.auth0.com/authorize?audience=casting&response_type=token&client_id=fFG0Rk7761WnCS9DBeKWnxbQ11OsDK0R&redirect_uri=https://abhkar1.herokuapp.com/login-results

There are three roles within the API. 

1) Casting Assistant 

Sample Login Credentials:

Email: test.assist@mail.com
Password: /TesT123/

2) Casting Director and 

Email: test.direct@mail.com
Password: /TesT123/

3) Executive Producer. 

Email: test.prod@mail.com
Password: /TesT123/

The logins for the three roles has been provided in the separate notes 

The url for the API:
https://abhkar1.herokuapp.com/

Client ID:

fFG0Rk7761WnCS9DBeKWnxbQ11OsDK0R

Client Secret:

vyTpeTi5H8DBp1mIAjOHwdiVWuVf24FEYvwDCRHE6XdtjQMbdCIXrcfJMB5xHK3A


JWT with Casting Assistant Access:

eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6InRRd3BwZDBzeUZfa0FnSE56UjZoVSJ9.eyJpc3MiOiJodHRwczovL2FiaGthci5hdXRoMC5jb20vIiwic3ViIjoiYXV0aDB8NWVjMTgzNTE0MGZhNTYwYzc1NjRjOGY5IiwiYXVkIjoiY2FzdGluZyIsImlhdCI6MTU4OTc0MDUzNywiZXhwIjoxNTg5NzQ3NzM3LCJhenAiOiJmRkcwUms3NzYxV25DUzlEQmVLV254YlExMU9zREswUiIsInNjb3BlIjoiIiwicGVybWlzc2lvbnMiOlsiZ2V0OmFjdG9ycyIsImdldDptb3ZpZXMiXX0.V4HKST0WE25m0I0En4NMIdXjYNcOW9SQh0rNlVrpSVGMLbO321vCipfUPAVglOqt7DYqB-rMFRyOzAW7hGh-O2gH-8eCZY7VLOXuSIV25_dL1F1orxVKRpaEbSM1_V1IwUIt9vz_GK7XMksCy4z2K_PNZ-IN-DPPMH5E3H9SByPAo_agO4kftARzhsOeCu5mDA8hK2m6GbNkS-daJeccndBmkiGfcBpeE3OHCUX-f7KFCL94uTinsTd_GH6qkgCi9r6nQyUZKeuWa8VwKhl6vxIZ6sx14RMcxyqm-SUZ4RaIpCDQ0nlGuLMZSpWOdZAqxEEt-RsJtbEqpnTFkQGCsQ

Sample Result From jwt.io

{
  "iss": "https://abhkar.auth0.com/",
  "sub": "google-oauth2|107904555616145504204",
  "aud": "casting",
  "iat": 1589739612,
  "exp": 1589746812,
  "azp": "fFG0Rk7761WnCS9DBeKWnxbQ11OsDK0R",
  "scope": "",
  "permissions": [
    "delete:actors",
    "get:actors",
    "get:movies",
    "patch:actors",
    "patch:movies",
    "post:actors"
  ]
}


JWT with Casting Director Access:

eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6InRRd3BwZDBzeUZfa0FnSE56UjZoVSJ9.eyJpc3MiOiJodHRwczovL2FiaGthci5hdXRoMC5jb20vIiwic3ViIjoiYXV0aDB8NWVjMTg3ODY0NTNlMjMwYzcxZDk5MWU5IiwiYXVkIjoiY2FzdGluZyIsImlhdCI6MTU4OTc0MTU3NCwiZXhwIjoxNTg5NzQ4Nzc0LCJhenAiOiJmRkcwUms3NzYxV25DUzlEQmVLV254YlExMU9zREswUiIsInNjb3BlIjoiIiwicGVybWlzc2lvbnMiOlsiZGVsZXRlOmFjdG9ycyIsImdldDphY3RvcnMiLCJnZXQ6bW92aWVzIiwicGF0Y2g6YWN0b3JzIiwicGF0Y2g6bW92aWVzIiwicG9zdDphY3RvcnMiXX0.PE8B6NbzqtBl0mMnEKrJqTAfp2ZKJ55m3al8Ptsl2_rCmXNVe6iGS08GsNS2VyWmuq6YCkT8lFZNgLl_SXEE93CH26kgP1o4xrTCFbFRpkfUsVIqEv-fATzlkKCeKrN3YLKNzby65mI2roUD7eGHagxZexY4UmTvQaardK-NLt6oiZc6ysHxGcsUu7DuuprrNw7x8x4YX39Arx2afb_hiZ9TYj1RCLfDR9y1eeLn1puDvOnMFLZCPZRj2eEx43WRGL9tqOvWtTk_q7xMgxXlEwsqW8KngHyK1XeLNNJFbkwHxew40d63jIAMeiBWu_at2asiDVL0PuTF9QNKowA4uQ


Sample Result from jwt.io

{
  "iss": "https://abhkar.auth0.com/",
  "sub": "auth0|5ec18786453e230c71d991e9",
  "aud": "casting",
  "iat": 1589741574,
  "exp": 1589748774,
  "azp": "fFG0Rk7761WnCS9DBeKWnxbQ11OsDK0R",
  "scope": "",
  "permissions": [
    "delete:actors",
    "get:actors",
    "get:movies",
    "patch:actors",
    "patch:movies",
    "post:actors"
  ]
}


JWT with Casting producer Access:

eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCIsImtpZCI6InRRd3BwZDBzeUZfa0FnSE56UjZoVSJ9.eyJpc3MiOiJodHRwczovL2FiaGthci5hdXRoMC5jb20vIiwic3ViIjoiYXV0aDB8NWVjMTg4ODc1ODMwYTkwYzZmZWExZWQwIiwiYXVkIjoiY2FzdGluZyIsImlhdCI6MTU4OTc0MTc2MywiZXhwIjoxNTg5NzQ4OTYzLCJhenAiOiJmRkcwUms3NzYxV25DUzlEQmVLV254YlExMU9zREswUiIsInNjb3BlIjoiIiwicGVybWlzc2lvbnMiOlsiZGVsZXRlOmFjdG9ycyIsImRlbGV0ZTptb3ZpZXMiLCJnZXQ6YWN0b3JzIiwiZ2V0Om1vdmllcyIsInBhdGNoOmFjdG9ycyIsInBhdGNoOm1vdmllcyIsInBvc3Q6YWN0b3JzIiwicG9zdDptb3ZpZXMiXX0.CvBl68b96GVRhpsfLeSPDLfQrtvMHXRbjxxN9lgvNKnUvLs3Orwf5DFtSq66Ke8wBvtjT0aUdVQ94ROhgxGMb4uphD-Eo4y9_Jd9_-Owmd8dPYeevVV_VzaFydybhkBfKb_vgOYBCRC87GQ0z97Xl1moOp5khGOuscSMsLnKNP-VKEFlYgC0J2KjC9Hbcx600GFejI6gCjzpiw5SG5Q13g5Q_q5GSHKjdOdfWXgQrkD9exleuoi9kfJIW2hzuAsjdOhFzY0WVBLb4kzUBNHVBd83ospPb6xgsFiLB9EacmCg6Mf2mw9OFOrhFbMWzqfehfRrQVI4ORjuo9MBsjnJyw

Sample Result from jwt.io

"iss": "https://abhkar.auth0.com/",
  "sub": "auth0|5ec188875830a90c6fea1ed0",
  "aud": "casting",
  "iat": 1589741763,
  "exp": 1589748963,
  "azp": "fFG0Rk7761WnCS9DBeKWnxbQ11OsDK0R",
  "scope": "",
  "permissions": [
    "delete:actors",
    "delete:movies",
    "get:actors",
    "get:movies",
    "patch:actors",
    "patch:movies",
    "post:actors",
    "post:movies"
  ]
}


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