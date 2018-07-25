# Deploy your application

# Android Certificate
1. Create Android certificate following [this instructive](./android/android.md).
2. Upload Android certificate to https://build.phonegap.com

# iOS process
2. Create iOS certificates following [this instructive](./apple/apple.md).
2. Upload the iOS certificates and provisioning profiles to https://build.phonegap.com

# Create and configure Facebook application
1. Enter https://developers.facebook.com/
2. Add and configure new application

# Create Firebase application for Android push notifications

# Create Analytics account
1. Create analytics account (analytics.google.com)
2. Configure analytics ID

# Create and configure Social Graphs application
1. Text of email for *account validation on registration*
2. Text of email for *account validation on password reset*
3. Text of email for *welcome message*
4. Facebook App ID and Secret Key
5. Firebase Sender ID and Server Key
6. Apple aps certificate (for push notifications)

# Register the owner of the application in Social Graphs
1. Register a new user that will be the owner of the application
2. Set the graph id of the new user as the owner of the application

# Create icons & screens
Install and use
https://www.npmjs.com/package/splashicon-generator

# Configure application.json
1. Configure Social Graphs application ID and secret key (graph id + frappuccino)
2. Configure facebook App ID
3. Configure firebase push notifications
4. Configure markets urls params.markets (used by web_warning page)
5. Configure params.auth.footerLink.[href & title]

# Configure config.xml
1. Set the id and version
2. Set name, description and author
3. Configure facebook plugin cordova-plugin-facebook4
4. Configure push notifications plugin phonegap-plugin-push

# Publish application - Android
1. https://play.google.com/apps/publish

# Publish application - iOS
1. https://itunesconnect.apple.com

# Publish application - web version
1. Compile application
2. Create bitbucket repository for web, android and iOS
3. Copy compiled resources
4. Update web server
5. Publish to markets

## Check website server configuration
1. OG redirects
2. Site certificate
3. Web warning customized
4. Check Back End API version

# Configure Mercadopago if required
Configure Mercadopago by following [this instructive](./mercadopago.md).
