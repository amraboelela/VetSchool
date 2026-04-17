# Get Me Into Vet School

A mobile app built with Expo (React Native) to help students get into veterinary school. Targets iOS (App Store) and Android (Google Play Store).

## Prerequisites

- [Node.js](https://nodejs.org/) 18+
- [Expo CLI](https://docs.expo.dev/get-started/installation/): `npm install -g expo-cli`
- [EAS CLI](https://docs.expo.dev/eas/): `npm install -g eas-cli`
- Expo account at [expo.dev](https://expo.dev)
- Apple Developer account ($99/yr) — for iOS builds
- Google Play Console account ($25 one-time) — for Android builds

## Getting Started

```bash
npm install
npx expo start
```

Scan the QR code with the **Expo Go** app on your phone to preview.

## Building for Production

### Configure EAS

```bash
eas login
eas build:configure
```

### iOS (App Store)

```bash
eas build --platform ios
```

Produces an `.ipa` file. Submit via:

```bash
eas submit --platform ios
```

### Android (Google Play)

```bash
eas build --platform android
```

Produces an `.aab` file (recommended) or `.apk`. Submit via:

```bash
eas submit --platform android
```

## Project Source

Original app hosted on Replit:
https://25950503-0bb3-485a-a5ef-efd74721e54a-00-3beir74u7dppo.expo.riker.replit.dev/
