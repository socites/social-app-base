# Process for creating the development certificate for your application

## 1. Create App Certificate "iOS App Development"
Create and download the development certificate.
**Note**: You have to create only one App Certifcate to sign all applications of your Organization.

1. Enter to https://developer.apple.com/account/
2. Go to **Certificates, Identifiers & Profiles**.
3. Go to **All**, it is an item under the **Certificates** list.
4. Click on the plus button at the right top of the **iOS Certificates** panel.
5. Select **iOS App Development** and click **Continue**.
5. Upload the CRS file.
6. Download the certificate.

Create and download the certificate.
The name of the certificate is **'ios_development.cer'**

The **distribution certificate** only has the signature of the .certSigningRequest.
It IS NOT associated with the App ID.

## 2. Register the devices where the application will be tested.
1. Enter to https://developer.apple.com/account/
2. Go to **Devices**.
3. Click on the plus button at the right top of the **iOS Certificates** panel.
4. Register the UUID of the devices where the application will be tested.

## 3. Create the "iOS Provisioning Profiles" for development
Create and download the provisioning profile for development.

1. Enter to https://developer.apple.com/account/
2. Go to **Provisioning Profiles**, then select "Development" - "iOS App Development".
3. Click on the plus button at the right top of the panel.
4. Select **iOS App Development** as the provisioning profile that you need.
5. Select App ID.
6. Select the distribution certificate.
7. Select devices.
8. Enter a profile name.
9. Download the provisioning profile file.
