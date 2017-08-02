## Sharely-api requirements
##### General provisions
Content-Type: application/json
After authorization in all the queries put a token in the header

<a name="authorization"></a>
### AUTHORIZATION

* [Login](docs/authorization.md#login)
* [Login by refresh token](docs/authorization.md#loginByRefreshToken)
* [Logout](docs/authorization.md#logout)
* [Check phone on server](docs/authorization.md#checkPhoneOnServer)
* [Check email on server](docs/authorization.md#checkEmailOnServer)
* [Check iban on server](docs/authorization.md#checkIbanOnServer)
* [Register](docs/authorization.md#register)
* [SMS Password](docs/authorization.md#smsPassword)
* [Forgot Password](docs/authorization.md#forgotPassword)
* [APNs token](docs/authorization.md#apnsToken)

<a name="user"></a>
### USER

* [Get user details](docs/user.md#userDetails)
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
