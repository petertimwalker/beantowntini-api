# beantowntini-api
This is the API for BeanTown-tini
## Devise endpoints for User
### POST /signup
```
{
    "user": {
        "email": "test@test.com",
        "password": "123456",
        "name": "John"
    }
}
{
    "status": {
        "code": 200,
        "message": "Signed up successfully."
    },
    "data": {
        "id": 1,
        "email": "test@test.com",
        "name": "John"
    }
}
```
### POST /login
```
{
    "user": {
        "email": "test@test.com",
        "password": "123456"
    }
}
{
    "status": {
        "code": 200,
        "message": "Logged in successfully.",
        "data": {
            "user": {
                "id": 1,
                "email": "test@test.com",
                "name": "John"
            }
        }
    }
}
```
### DELETE /logout
Add JWT token to Authorization in Header
```
{
    "status": 200,
    "message": "Logged out successfully."
}
```
