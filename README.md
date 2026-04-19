# Get Me Into Vet School

A mobile app built with Expo (React Native) to help students get into veterinary school. Targets iOS (App Store) and Android (Google Play Store).

Original app hosted on Replit:
https://25950503-0bb3-485a-a5ef-efd74721e54a-00-3beir74u7dppo.expo.riker.replit.dev/

## Prerequisites

- [Node.js](https://nodejs.org/) 18+
- [EAS CLI](https://docs.expo.dev/eas/): `npm install -g eas-cli`
- Expo account at [expo.dev](https://expo.dev)
- Apple Developer account access — for iOS builds
- Google Play Console account — for Android builds

## Getting Started

```bash
npm install
npx expo start
```

Scan the QR code with the **Expo Go** app on your phone to preview.

## Submitting to the App Store

### Step 1: Get the Source Code
- Export/download the app from Replit (or clone the linked GitHub repo)
- Run `npm install` in the project directory

### Step 2: Configure EAS Build

```bash
eas login
eas build:configure
```

Make sure the `bundleIdentifier` in `app.json` matches what is registered in the Apple Developer account.

### Step 3: Set Up App Store Connect
- Go to [appstoreconnect.apple.com](https://appstoreconnect.apple.com)
- Create a new App listing (Bundle ID, app name, SKU)
- Fill in metadata: description, screenshots, category, privacy policy URL

### Step 4: Build for iOS

```bash
eas build --platform ios
```

This produces an `.ipa` file ready for submission.

### Step 5: Submit to the App Store

```bash
eas submit --platform ios
```

Then in App Store Connect:
- Select the uploaded build
- Fill in version info and review notes
- Click **Submit for Review**

## Submitting to Google Play

### Build for Android

```bash
eas build --platform android
```

Produces an `.aab` file (recommended).

### Submit to Google Play

```bash
eas submit --platform android
```
