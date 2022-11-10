# TrekApp
WSA_Project
Features:
Database 	HTTP Methods
Create 	POST
Retrieve 	GET
Update 	PUT
Delete 	DELETE
API Endpoints

=> POST http://127.0.0.1:5000/api/doLogin/

Parameters:

    email : required: Email of the registered user
    psw: required: Password of registered user

eg: Payload: { "email": "your email", "psw": "your password" }

Response:

    loggedin: Returns True or False based on login status
    message: A message after login is attempted
    token: A token to be used for authorization

=> POST http://127.0.0.1:5000/api/doRegister/

=> GET http://127.0.0.1:5000/api/treks/

    Response: JSON

=> POST http://127.0.0.1:5000/api/doAddTrek/

Parameters:

    title : required: text: Title of the trek
    days: required: number: Number of days required for the trek
    difficulty: required: text: Diffculty level
    total_cost: required: number: Total Cost

eg: Payload: { "title": "your email", "days": , "difficulty": "your password", "total_cost": <total_cost>, }

Response:

    message: A message after trek addition is attempted

Basic API Endpoints

    Register => POST - /api/doRegister

    Login => POST - /api/doLogin

    All Treks => GET - /api/treks

    Add Trek => POST - /api/doAddTrek

    Update Trek => PUT - /api/doUpdateTrek

    Delete Trek => DELETE - /api/doDeleteTrek

REST Framework

Resource: Treks

    All Treks => /api/treks => GET
    Add Treks => /api/treks => POST
    Update Treks => /api/treks => PUT
    Delete Treks => /api/treks => DELETE

Resource: Iternaries

/rest/iternaries

    GET /rest/iternaries
    POST /rest/iternaries
    PUT /rest/iternaries
    DELETE /rest/iternaries
