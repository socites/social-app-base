# Mercadopago

## Create new application
1. Enter applications.mercadopago.com.ar:
2. Create new application.
3. Set the domain of the application in the redirect uri field. Example: https://domain.com
4. Set authorized Javascript Origins if the application has a different domain to be set. Example: dev.domain.com
5. Set read and write scopes.

## Get the public key and the private access token
1. Get the *public key* and the *private access token* for production and sandbox by accessing https://www.mercadopago.com/mla/account/credentials?type=basic

## Configure the application.json
1. Configure the *public key* in the application.json.

## Configure the backend
1. Set application_id, public key and private access token.
Note: Do not use the secret_key.

## Go to production
1. Enter https://www.mercadopago.com/mla/account/credentials?type=basic
2. Click the link "Quiero ir a producción"
