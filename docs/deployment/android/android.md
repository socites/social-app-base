# Create Android Certificate
1. Download and install Java.
2. Set Java_Home directory.

3. Open the command prompt (cmd.exe) as an Administrator, then Run the following command:
keytool -genkey -v -keystore [keystore_name].keystore -alias [alias_name] -keyalg RSA -keysize 2048 -validity 10000

4. Keytool will ask for keystore password. Enter password and confirm:
5. Next, keytool will ask for additional information. Supply appropriately:
6. Next, keytool will ask password for Alias. Return if it's the same as keystore password. Othewise enter password and confirm.
7. Your signing key is now ready to submit.
