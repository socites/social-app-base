# Certificates and Provisioning Profile for Production

## 1. Process for creating the certificate required to deploy your application in the Apple App Store
Follow the nexts steps to create and download the production certificate.

1. Enter to https://developer.apple.com/account/
2. Go to **Certificates, Identifiers & Profiles**.
3. Go to **All**, it is an item under the **Certificates** list.
4. Click on the plus button at the right top of the **iOS Certificates** panel.
5. Select **App Store and Ad Hoc** and click **Continue**.
6. Upload the CRS file.
7. Download the certificate.

**Notes**
The name of the certificate is **'ios_distribution.cer'**

The **distribution certificate** only has the signature of the .certSigningRequest.
It IS NOT associated with the App ID.


## 2 Create the "iOS Provisioning Profiles" for production
Create and download the provisioning profile for production.

1. Enter to https://developer.apple.com/account/
2. Go to **Provisioning Profiles**, then select "Distribution" - "App Store".
3. Click on the plus button at the right top of the panel.
4. Select App ID.
5. Select the distribution certificate.
6. Enter a profile name.
7. Download the provisioning profile file.
