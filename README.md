# electron-quickstart-mas

**Build a Hello-World app for the Mac App Store.**

This is the electron-quick-start app (see https://github.com/electron/electron-quick-start) set up to be built for the Mac App Store. 

This app goes along with the tutorial https://techandstartup.com/tutorials/release-electron-app-on-mac-app-store

**Steps to build this app for the mac app store:**

- Load the development dependencies electron and electron-builder: `npm install`
- Run it in dev mode to make sure it works: `npm run start`
- Add your own MacAppStore.provisionprofile to the project root directory.
- Add your own TeamID.appID in the entitlements.mas.plist file on line 9.
- In the package.json file at a minimum change the name and appId properties to your information.
- Build the app for the mac app store: `electron-builder --mac`
