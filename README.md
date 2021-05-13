# Maskot App - v2

Version 1 in branch `v1`

Version 2 officially started 25th Oct 2017

## Table of Contents

  * [Requirements](#requirements)
  * [Install](#install)
  * [Run with Local API](#run-with-local-api)
  * [Run on iOS Device or Simulator](#run-on-ios-device-or-simulator)
  * [Run on Android](#run-on-android)

## Requirements

- [NPM](https://www.notion.so/NPM-0036c999472444fdb92bcb4614d9e65d)
- [Yarn](https://www.notion.so/Yarn-04437ca66f35406a912494c2a9d4586b)
- constants.js (Ask Developer)

## Install

**1.**  Clone Project
```sh
git clone git@gitlab.com:maskot.co/maskot-app.git
```

**2.**  Install dependencies

```sh
npm install
```
```sh
yarn install
```

## Run with Local API

```diff
- Before proceeding, you should get the local api project environment set up:
```
[maskot-frontend](https://gitlab.com/maskot.co/maskot-frontend)

**1.**  After your backend is running, add your constants.js file (Check Requirements) to:
> ./src/

**2.**  Make sure the file code is commented in Production and uncommented in Local to connect to local API.

**3.**  In your local DB/maskot_frontend_dev-database/maskot_app_version-table add a new field:
| id  | version | created_at  | updated_at | 
| ------------- | ------------- | ------------- | ------------- |
| 1 | 3.1.5  | 2019-03-20 18:00:00  | 2019-03-20 18:00:00  |

## Run on iOS

**1.**  Before installing your pods change the following:
> ./node_modules/@react-native-community/netinfo/react-native-netinfo.podspec > Change 'React-Core' to 'React/Core'

**2.**  Install Pods:
```sh
cd ios
pod install
```

**3.**  Generate main.jsbundle:
```sh
yarn react-native bundle --entry-file ./index.js --platform ios --bundle-output ios/main.jsbundle
```

**4.**  Run on iOS:
```sh
npx react-native run-ios
```

## Run on Android

```diff
- Current Developer couldn't run local db in android. 
! The following steps install the application yet it might not run with your local database due to the emulator.
```

**1.**  Open a Device from Android Studio's AVD Manager.


**2.**  Create local.properties file in ./android, add the following and replace:
```sh
sdk.dir = /Users/YourName/Library/Android/sdk
```

**3.**  Set up Android X:
```sh
npx jetifier
```

**4.**  Run on Android:
```sh
npx react-native run-android
```

