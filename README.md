# electron-quickstart-mas

**Starter app to test building for the Mac App Store.**

This is the electron-quick-start app (see https://github.com/electron/electron-quick-start) set up to be built for the Mac App Store. 

This app goes along with the tutorial https://www.techandstartup.com/tutorials/release-electron-app-on-mac-app-store

**Steps to build this app for the mac app store:**

- Load the development dependencies electron and electron-builder: `npm install`
- Run it in dev mode to make sure it works: `npm run start`
- Add your own MacAppStore.provisionprofile to the build directory.
- Add your own TeamID.appID in the entitlements.mas.plist file on line 9.
- In the package.json file at a minimum change the name and appId properties to your information.
- Build the app for the mac app store: `electron-builder --mac`

**To build a Development version of this app (for testing) make the following changes:**

- Add your own AppleDevelopment.provisionprofile to the build directory.
- Make the following changes to the package.json file:
  - Change "target": "mas" to "target": "mas-dev".
  - Change "type": "distribution" to "type": "development".
  - Change "provisioningProfile": "build/MacAppStore.provisionprofile" to "provisioningProfile": "build/AppleDevelopment.provisionprofile".
