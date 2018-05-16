# Mercadopago

## Create new application
1. Enter applications.mercadopago.com.ar:
2. Create new application.
3. Set the domain of the application in the redirect uri field. Example: https://domain.com
4. Set authorized Javascript Origins if the application has a different domain to be set. Example: dev.domain.com
5. Set read and write scopes.

## Get the public key
Get the public key for production and sandbox by accessing https://www.mercadopago.com/mla/account/credentials?type=basic

## Configure the backend
1. Set application_id, secret_key and public key

## Go to production
1. Enter https://www.mercadopago.com/mla/account/credentials?type=basic
2. Click the link "Quiero ir a producción"
