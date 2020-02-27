# RESTful Web API Doc

This RESTful Web API is about a website users and accounts management [referring to Django REST framework](https://www.django-rest-framework.org/ "Django REST framework"). It is documented on a [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet "Markdown") page hosted in my [GitHub](https://github.com/helenwang1610/api/blob/master/README.md "Honglei Wang's RESTful Web API Design") public repository.  In this API, two entities are used. One is userS, the other is accountS.

------------

## Open Endpoints

------------


Open endpoints requires no Authentication.
- [Login](https://github.com/helenwang1610/api/blob/master/login.md "Login the Website") : POST /api/login/


------------

## Close Endpoints 

------------

Closed endpoints require a valid string to be included in the header of the request as authentication. A string can be acquired from the Login view above.

### User Actions
Each endpoint manipulates or displays information about the user whose token is provided with the request.
- [View user profile](https://github.com/helenwang1610/api/blob/master/getUserInfo.md "View user information") : POST /api/login):               GET /api/user/
- [Update user information](https://github.com/helenwang1610/api/blob/master/updateUserInfo.md "Update user information"):   PUT /api/user/


### Account Actions
Endpoints for viewing and manipulating the Accounts that the Authenticated User has permissions to access.
- [Show Accessible Accounts](https://github.com/helenwang1610/api/blob/master/showAccounts.md "Show Accessible Accounts"): GET /api/accounts/
- [Create an Account](https://github.com/helenwang1610/api/blob/master/createAccount.md "Create an Account"): POST /api/accounts/
- [Show An Account]](https://github.com/helenwang1610/api/blob/master/viewSingleAccount.md "View a single account information"): GET /api/accounts/:sg/
- [Update An Account]](https://github.com/helenwang1610/api/blob/master/updateAccount.md "Update an Account"): PUT /api/accounts/:sg/
- [Delete An Account]](https://github.com/helenwang1610/api/blob/master/deleteAccount.md "delete an Account"): DELETE /api/accounts/:sg/


## End