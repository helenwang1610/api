# View User Profile 

------------

Get the details of the currently Authenticated User along with basic subscription information.

URL : /api/user/

Method : GET

Auth required : YES

Permissions required : None

```json
Success Response
Code : 200 OK

Content examples

For a User with ID 123 on the local database where that User has saved an email address and name information.

{
    "id": 123,
    "first_name": "Honglei",
    "last_name": "Wang",
    "email": "hwd29@mail.missouri.edu"
}
For a user with ID 321 on the local database but no details have been set yet.

{
    "id": 321,
    "first_name": "",
    "last_name": "",
    "email": ""
}

```
### Notes
If the User does not have a UserInfo instance when requested then one will be created for them.


------------

### End