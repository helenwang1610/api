#Login 

------------

Used to collect a Token for a registered User.

URL : /api/login/

Method : POST

Auth required : NO

Data constraints

{
    "username": "[valid email address]",
    "password": "[password in plain text]"
}
Data example

{
    "username": "ilovemu@example.com",
    "password": "myzou123"
}
Success Response
Code : 200 OK

Content example

{
    "token": "23434rsadfad32465sdfg346745721fdsfa545546"
}
Error Response
Condition : If 'username' and 'password' combination is wrong.

Code : 400 BAD REQUEST

Content :

{
    "non_field_errors": [
        "Unable to login with provided credentials."
    ]
}

------------

###End