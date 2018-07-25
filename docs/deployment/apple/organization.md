# Create the organization certificates

## Create App Certificate "App Store and Ad Hoc"
Create and download the certificate.

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


## Create App Certificate "iOS App Development"
Create and download the development certificate.

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
