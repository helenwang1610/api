# Create User's Account 

------------

Create an Account for the authenticated User if an Account for that User does not already exist. Each User can only have one Account.

URL : /api/accounts/

Method : POST

Auth required : YES

Permissions required : None

Data constraints

Provide name of Account to be created.

{
    "name": "[unicode 64 chars max]"
}
Data example All fields must be sent.

{
    "name": "Build something project dot com"
}
Success Response
Condition : If everything is OK and an Account didn't exist for this User.

Code : 201 CREATED

Content example

{
    "id": 123,
    "name": "Build something project dot com",
    "url": "http://testserver/api/accounts/123/"
}
Error Responses
Condition : If Account already exists for User.

Code : 303 SEE OTHER

Headers : Location: http://testserver/api/accounts/123/

Content : {}

Or
Condition : If fields are missed.

Code : 400 BAD REQUEST

Content example

{
    "name": [
        "This field is required."
    ]
}

------------

### End