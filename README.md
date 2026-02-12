# SGTM Analytics iOS Sample

A sample iOS app demonstrating server-side Google Tag Manager (sGTM) analytics integration.

## Setup

### 1. Firebase Configuration

This project requires a Firebase `GoogleService-Info.plist` file, which is not included in the repository for security reasons.

1. Go to the [Firebase Console](https://console.firebase.google.com/)
2. Select your project (or create a new one)
3. Add an iOS app and download the `GoogleService-Info.plist` file
4. Place the file in the `iOS SGTM/` directory

### 2. URL Types Configuration

You need to update the URL Types in Xcode to match your own Firebase project:

1. Open the project in Xcode
2. Select the **iOS SGTM** target
3. Go to the **Info** tab
4. Scroll down to **URL Types**
5. Update the **Identifier** to your app's bundle identifier (e.g. `com.yourcompany.yourapp`)
6. Update the **URL Scheme** in the sGTM expected format: `tagmanager.sgtm.c.{{package name}}` (e.g. `tagmanager.sgtm.c.com.ffgcvs.testapp`)
