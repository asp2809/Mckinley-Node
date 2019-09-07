# McKinley and Rice - Node.js

For deployment, `Heroku` or `Glitch` can be used.

## APIs

TYPE: `POST`

ROUTE: `/api/users/login`

BODY: `{email, password}`

RESPONSE:

<u>Success</u>

```
{
    "success": true,
    "token": "Bearer faksjdfkjsafjdsjfasdkjasfdk123kjdkjfadfjk"
}
```

<u>Error</u>

```
{
    "email": "User not found!"
}
```

or

```
{
    "password": "Wrong Password"
}
```

<hr>

TYPE: `POST`

ROUTE: `/api/users/register`

BODY: `{name, email, password, password2}`

RESPONSE:

<u>Success</u>

```
{
    "_id": "5d7414d21017f008e45aec45",
    "name": "noble2809",
    "email": "test1234@gmail.com",
    "password": "$2a$10$l2jNWTwIGSMrfAx70D/hh.6BjyZfPgB/bcuj.07b5hbmaAc8paOP.",
    "date": "2019-09-07T20:36:34.205Z",
    "__v": 0
}
```

<u>Error</u>

```
{
    "email": "Email already exists"
}
```
