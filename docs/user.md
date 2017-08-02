<a name="#user_details"></a>
## Get user details

`GET /api/v1/myaccount/`

### Response example
<b><u>Header</u></b>:<br/>
Authorization : Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOjU5MDcsImlzcyI6Imh0dHBzOi8vYXBpLXNoYXJlbHktc3RhZ2luZy5kZXZjb2Rpbi5jb20vYXBpL3YxL2F1dGhvcml6ZSIsImlhdCI6MTUwMTY2MjY2MiwiZXhwIjoxNTAxNjY2MjYyLCJuYmYiOjE1MDE2NjI2NjIsImp0aSI6Ik53aXNxa2JzcmJ0aDNxenoifQ.HXQcIjGQ_D2n71ytZvKeGVFtucJUZQFMwgkuViW-lR0

```json
{
  "id":5907,
  "parent_id":null,
  "media_id":null,
  "company":"",
  "title":"herr",
  "firstname":"test",
  "lastname":"test",
  "email":"test@test123.com",
  "phone":"+41 77 999 33 22",
  "vat_apply":0,
  "vat_id":"",
  "created":"2017-07-12 09:26:07",
  "modified":null,
  "is_active":1,
  "role_id":2,
  "subscribe_sms":1,
  "subscribe_email":0,
  "confirmed":1,
  "ogone_alias":null,
  "iban":null,
  "last_login":"2017-07-12 09:47:58",
  "preferred":"morgens",
  "is_facebook":0,
  "group_address_id":null,
  "emails_behavior":null,
  "status":"active",
  "idle_count":0,
  "idleLastCheck":null,
  "referalId":null,
  "communityId":null,
  "isFreeCommunity":null,
  "organization":"",
  "is_idle_manual":0,
  "block_reason":null,
  "ebanking_limit":null,
  "iban_id":null,"mspid":"",
  "address":{
    "id":5904,
    "parent_id":5907,
    "address_type":1,
    "is_private":0,
    "is_main":1,
    "company":"",
    "firstname":"test",
    "lastname":"test",
    "street":"Z\u00fcrcher Str.",
    "zip":"9015",
    "city":"Gossau",
    "country":null,
    "lat":47.4077,
    "lng":9.29263,
    "email":"test@test123.com",
    "date_of_birth":null,
    "created":"2017-07-12 09:26:08",
    "modified":null
  }
}
```

<a name="#update_profile"></a>
## Update user profile

`PUT /api/v1/myaccount/`

```json
{
    "salutationPicker" : "morning",
    "sex" : "male",
    "firstName" : "John Jonah",
    "lastName" :  "Jameson",
    "address" : {
           "country" : "Germany",
            "postIndex" : "060700",
            "city" : "Berlin",
            "street" : "LuftWafeStrasse",
            "lat" :  151.1960371,
            "lng" : -33.8665053
    },
    "mobile" : "+14155552671",
    "receive" : true,
    "iban" : "123.456.789",
    "companyName" : "My company",
    "avatar" : "http://some.url.com"
}

```
