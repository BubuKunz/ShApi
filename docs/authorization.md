`POST /api/v1/authorize`

## Login

`POST /api/v1/authorize`

### Request body example

```json
{
    "login" : "useremail@gmail.com",
    "password" : "123456asd"
}
```

### Request results

* `200 OK`
* `500 Internal Server Error`
```json
{
    "error":{
        "message":"The given data failed to pass validation."
    },
    "status_code":500
}
```

### Response example
```json
{
    "message":  "token_generated",
    "data": {
      "token" : "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjU5MDcsImlzcyI6Imh0dHBzOi8vYXBpLXNoYXJlbHktc3RhZ2luZy5kZXZjb2Rpbi5jb20vYXBpL3YxL2F1dGhvcml6ZSIsImlhdCI6MTUwMTA4MTg0NiwiZXhwIjoxNTAxMDg1NDQ2LCJuYmYiOjE1MDEwODE4NDYsImp0aSI6Ijg0WEZIcjNFb21oTHUzRVkifQ.AY8X_PGUfKcWImfMOeOjNMldCgIAaolwfl5OO5_61B8",
      "expires_in" : 60
    }
 }

```

## Login by refresh token

`POST /api/v1/authorize/refresh`

### Request body example

```json
{
 "authorize":{
    "refreshToken": "8fee92d291026709a71d798f319c53987fc35609"
  }
}

```

### Request results

* `200 OK`

### Response example
```json
{
"id":12,
    "accessToken": "0c9ec4e5dfd95579123500e7c84ae4a944e7e0a7",
    "expires_in": 86400,
    "refreshToken": "8fee92d291026709a71d798f319c53987fc35609"
}


```

## Logout
`GET /api/v1/logout`

### Request results

* `200 OK`

### Response example

```json
{
  "code" : 2002,
  "description" : "success logout"
}


```

### Check phone on serve

`POST /api/v1/check/phone/`

### Request body example

```json
{
  "phone" : 380681111111
}

```

### Request results

* `200 OK`


### Success response example
```json
{
 "success": {
    "code" : 2002,
    "description" : "Phone XXXXXXXXXXX is not used"
  }
}


```

### Unsuccess  response example
```json
{
 "success": {
    "code" : 4004,
    "description" : "Phone XXXXXXXXXXX is used"
  }
}


```

## Check email on server

`POST /api/v1/check/email/`

### Request body example

```json
{
  "email " : "aaa@bbb.ccc"
}

```

### Request results

* `200 OK`


### Success response example
```json
{
 "success": {
    "code" : 2002,
    "description" : "Email aaa@bbb.ccc is not used"
  }
}


```

### Unsuccess  response example
```json
{
 "success": {
    "code" : 4004,
    "description" : "Email aaa@bbb.ccc is used"
  }
}


```

## Check iban on server

`POST /api/v1/check/iban/`

### Request body example

```json
{
  "iban" : 25634456332
}

```

### Request results

* `200 OK`


### Success response example
```json
{
 "success": {
    "code" : 2002,
    "description" : "Iban XXXXXXXXXXX is not used"
  }
}


```

### Unsuccess  response example
```json
{
 "success": {
    "code" : 4004,
    "description" : "Iban XXXXXXXXXXX is used"
  }
}


```

## Register

`POST /api/v1/user`

### Request body example

```json
{
    "email" : [string],
    "password" : [alphanumeric/5 min],
    "password_confirmation" : [alphanumeric/5 min],
    "firstname" : [string],
    "lastname" : [string],
    "phone": [00417********],
    "mspid":[string],
    "communityId": [integer]
}
```

### Request results

* `200 OK`
* `500 Internal Server Error`
```json
{
    "error":{
        "message":"The given data failed to pass validation."
    },
    "status_code":500
}
```

### Response example
```json
{
    "message":  "token_generated",
    "data": {
      "token" : "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjU5MDcsImlzcyI6Imh0dHBzOi8vYXBpLXNoYXJlbHktc3RhZ2luZy5kZXZjb2Rpbi5jb20vYXBpL3YxL2F1dGhvcml6ZSIsImlhdCI6MTUwMTA4MTg0NiwiZXhwIjoxNTAxMDg1NDQ2LCJuYmYiOjE1MDEwODE4NDYsImp0aSI6Ijg0WEZIcjNFb21oTHUzRVkifQ.AY8X_PGUfKcWImfMOeOjNMldCgIAaolwfl5OO5_61B8",
      "expires_in" : 60
    }
 }

```

## SMS Password

`POST /api/v1/password-recovery`

### Request body example

```json
{
    "phone": "+3801234567890",
    "otp" : "4356"
}

```

### Request results

* `200 OK`

### Response example
```json
{
    "success": {
        "code" : 2002,
        "description" : ""
    }
}


```


## Forgot Password

`POST /api/v1/password-recovery`

### Request body example

```json
{
    "email": "youremail@mail.com"
}

```

### Request results

* `200 OK`

### Response example
```json
{
    "success": {
        "code" : 2002,
        "description" : "instructions on how to recovery password sent to the email address",
        "email" : "youremail@mail.com"
    }
}


```

## APNs token

`POST /api/v1/push/ios/`

### Request body example

```json
{
    "deviceToken": "2ffca4ad6599adc9b5202d15a5286d33c19547d472cd09de44219cda5ac30207"
}


```

### Request results

* `200 OK`

### Response example
```json
{
    "success": {
        "code" : 2002,
        "description" : "instructions on how to recovery password sent to the email address",
        "email" : "youremail@mail.com"
    }
}


```
