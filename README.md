<p align="center">
  <a href="https://img.ly/video-sdk?utm_campaign=Projects&utm_source=Github&utm_medium=VESDK&utm_content=React-Native-Demo">
    <img src="https://img.ly/static/logos/VE.SDK_Logo.svg" alt="VideoEditor SDK Logo"/>
  </a>
</p>
<p align="center">
  <a href="https://npmjs.org/package/react-native-videoeditorsdk">
    <img src="https://img.shields.io/npm/v/react-native-videoeditorsdk.svg" alt="NPM version">
  </a>
  <a href="https://npmjs.org/package/react-native-videoeditorsdk">
    <img src="https://img.shields.io/badge/platforms-android%20|%20ios-lightgrey.svg" alt="Platform support">
  </a>
  <a href="http://twitter.com/VideoEditorSDK">
    <img src="https://img.shields.io/badge/twitter-@VideoEditorSDK-blue.svg?style=flat" alt="Twitter">
  </a>
</p>

# VideoEditor SDK React Native Example App

This project shows how to integrate [VideoEditor SDK](https://img.ly/video-sdk?utm_campaign=Projects&utm_source=Github&utm_medium=VESDK&utm_content=React-Native-Demo) into a React Native application with the [React Native module for VideoEditor SDK](https://github.com/imgly/vesdk-react-native) which is available via NPM as [`react-native-videoeditorsdk`](https://www.npmjs.com/package/react-native-videoeditorsdk).

## Getting started

After cloning this repository, perform the following steps to run the example application:

```sh
# install
yarn install
cd ios && pod install && cd .. # CocoaPods on iOS needs this extra step
# run
npx react-native run-ios
# or
npx react-native run-android
```

## Unlock the SDK

VideoEditor SDK is a product of img.ly GmbH. Without unlocking, the SDK is fully functional but a watermark is added on top of the video preview and any exported videos.
In order to remove the watermark and to use VideoEditor SDK within your app **you'll need to [request a license](https://img.ly/pricing?product=vesdk&?utm_campaign=Projects&utm_source=Github&utm_medium=VESDK&utm_content=React-Native-Demo) for each platform and load the license file(s)** in your [`App.js`](./App.js#L30-L36) with the following single line of code that automatically resolves multiple license files via [platform-specific file extensions](https://reactnative.dev/docs/platform-specific-code#platform-specific-extensions):

```js
VESDK.unlockWithLicense(require('./vesdk_license'));
```

## VideoEditor SDK for iOS & Android

The React Native module for VideoEditor SDK includes a rich set of most commonly used [configuration and customization options](https://github.com/imgly/vesdk-react-native/blob/master/configuration.ts) of VideoEditor SDK for iOS and Android. The native frameworks provide **fully customizable** video editors. Please refer to [our documentation](https://img.ly/docs/vesdk?utm_campaign=Projects&utm_source=Github&utm_medium=VESDK&utm_content=React-Native-Demo) for more details.

Native customization for iOS is demonstrated in the [`AppDelegate`](./ios/VESDKExample/AppDelegate.m#L36-L47) of the example application.

## License Terms

Make sure you have a [commercial license](https://img.ly/pricing?product=vesdk&?utm_campaign=Projects&utm_source=Github&utm_medium=VESDK&utm_content=React-Native-Demo) for VideoEditor SDK before releasing your app.
A commercial license is required for any app or service that has any form of monetization: This includes free apps with in-app purchases or ad supported applications. Please contact us if you want to purchase the commercial license.

## Support and License

Use our [service desk](http://support.img.ly) for bug reports or support requests. To request a commercial license, please use the [license request form](https://img.ly/pricing?product=vesdk&?utm_campaign=Projects&utm_source=Github&utm_medium=VESDK&utm_content=React-Native-Demo) on our website.
