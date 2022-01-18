
# Beers & Burgers API 

This fake API made with JSON Server works on a burger shop application containing user's data and catalog's data.

## Endpoints

This API contains endpoints to register and login a user, display users, catalog, and register cart choices.

### SignUp 

This endpoint registers a new user and sends its data to "Users". Its required field is "email" and "password".

`POST /users - Request format `

```json
{
    "email": "barry@mail.com",
    "password": "123456"
}
```
`POST /users - Request response - 201 Created `

```json
{
  "email": "barry@mail.com",
  "password": "123456",
  "id": 2
}
```
### SignIn

`POST /login - Request format ` 
```json
{
	"email": "jondoe@gmail.com",
	"password": "987654321"
}
```
`POST /login - Request response - 200 OK `
```json
{
  "user": {
    "email": "jondoe@gmail.com",
    "id": 2
  }
}
```