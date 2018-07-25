# Process for application deployment in the Apple App Store

## 1. Add an App ID
1. Enter to https://developer.apple.com/account/
2. Go to **Certificates, Identifiers & Profiles**.
3. Go to **App IDs**, it is an item under **Identifiers**.
4. Set the field **description** with the name of your application.
5. Set the Bundle ID: reverse-domain name style string. Example: '**com.example.application**'.
6. Set the app services: **+ push notifications**.
7. Confirm the form by clicking the **Register** button.

Now you have set the **App ID** for your application.

## 2. Add Certificates

### 2.1 Create a CSR file
To create a CSR file [Follow this link](./csr.md).
**Note**: Only generate one CSR file that represents the company that is developing the application.

### 2.2 Create Organization Certificates
To create the organization certificates [Follow this link](./organization.md).

### 2.3 Create Certificate "Apple Push Notification service SSL (Sandbox & Production)"
Create and download the certificate:
1. Enter to https://developer.apple.com/account/
2. Go to **Certificates, Identifiers & Profiles**.
3. Click on the plus button at the right top of the panel.
4. Select the App ID.
5. Upload the CRS file.
6. Download the certificate.

The name of the certificate is **'aps.cer'**
The **push notification certificate** IS associated to the App ID.


### 2.4 Create the "iOS Provisioning Profiles" for production
Create and download the provisioning profile for production.

1. Enter to https://developer.apple.com/account/
2. Go to **Provisioning Profiles**, then select "Distribution" - "App Store".
3. Click on the plus button at the right top of the panel.
4. Select App ID.
5. Select the distribution certificate.
6. Enter a profile name.
7. Download the provisioning profile file.


### 2.5 Create the "iOS Provisioning Profiles" for development
Create and download the provisioning profile for development.

1. Enter to https://developer.apple.com/account/
2. Go to **Provisioning Profiles**, then select "Development" - "iOS App Development".
3. Click on the plus button at the right top of the panel.
4. Select App ID.
5. Select the distribution certificate.
6. Select devices.
7. Enter a profile name.
8. Download the provisioning profile file.


### 2.6 Convert the "App Store and Ad Hoc" ('ios_distribution.cer') certificate to .p12 extension
Generating the p12 certificate.

1. Open the **Keychain Access** application.
2. If the certificate is not already added to Keychain, select File > Import. 
Then navigate to the certificate file (the .cer file).
3. Select the Keys category in Keychain Access.
4. Select the private key associated with your iPhone Development Certificate. The private key is identified by the iPhone Developer: public certificate that is paired with it.
5. Control-click the iPhone Developer certificate and select, Export "iPhone Developer: Name...".


### 2.7 Convert the "Push Notifications" ('aps.cer') certificate to .pem extension

1. Launch Keychain Access.
2. Import aps.cer certificate (File - Import Items).
3. Go to "Certificates".
3. Find the certificate "Apple Push Services: app_bundle". 
4. Ctl-click - export "Apple Push ...". 
5. Save as .p12. If .p12 option is disabled, check that you are in the "Certificates" option in the menu.
6. openssl pkcs12 -in aps.p12 -out aps.pem -nodes -clcerts
