# Facebook configuration

## 1.Development
Replace **app_alias** and **file_name**.
keytool -exportcert -alias app_alias -keystore file_name.keystore | openssl sha1 -binary | openssl base64

## 2.Production. Download "App signing certificate" from Google.
1. Go to "Release management", then "App signing"
2. Download certificate "App signing certificate"
3. cat deployment_cert.der |openssl sha1 -binary | openssl base64
