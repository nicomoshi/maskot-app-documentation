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

(NPM)[https://www.notion.so/NPM-0036c999472444fdb92bcb4614d9e65d]
(Yarn)[https://www.notion.so/Yarn-04437ca66f35406a912494c2a9d4586b]
constants.js (Ask Developer)

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

> Before proceeding, you should get the local api project environment set up:
https://gitlab.com/maskot.co/maskot-frontend

**1.**  After your backend is running, add your constants.js file (Check Requirements) to:
> ./src/

**2.**  Make sure the file code is commented in Production and uncommented in Local to connect to local API.

## Run on iOS Device or Simulator

**1.**  Run on iOS:
```sh
npx react-native run-ios
```

## Run on Android

**1.**  Run on Android:
```sh
npx react-native run-android
```
