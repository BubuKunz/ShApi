## Sharely-api requirements
##### General provisions
Content-Type: application/json
After authorization in all the queries put a token in the header

<a name="authorization"></a>
### AUTHORIZATION

* [Login](docs/authorization.md#login)
* [Login by refresh token](docs/authorization.md#login-by-refresh-token)
* [Logout](docs/authorization.md#logout)
* [Check phone on server](docs/authorization.md#check-phone-on-server)
* [Check email on server](docs/authorization.md#check-email-on-server)
* [Check iban on server](docs/authorization.md#check-iban-on-server)
* [Register](docs/authorization.md#register)
* [SMS Password](docs/authorization.md#sms-password)
* [Forgot Password](docs/authorization.md#forgot-password)
* [APNs token](docs/authorization.md#apns-token)

<a name="user"></a>
### USER

* [Get user details](docs/user.md#user_details)
* [Update user profile](docs/user.md#updateProfile)
* Get my renting requests
* Update renting request status
* Delete renting requests
* Lease item
* Get my leasing requests
* Update leasing request status
* Delete leasing requests
* Add item to favorites
* Move item from favorites
* Create item
* Get items
* Update item
* Delete items
* Post Image
* Delete Image
* Post review

<a name="public_info"></a>
### PUBLIC INFO

* Get item reviews
* Get user reviews
* Get user items
* Get public profile
* Get public items
* Get item details

<a name="payment"></a>
### PAYMENT

* Create paycheck
* GET session ID

<a name="push_notification"></a>
### PUSH NOTIFICATIONS

* Favorite items update
* Favorite item add
* Favorite item remove
* My item update
* My item add
* My item remove
* Renting item update
* Leasing item update
* My profile update
* Message received
