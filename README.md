# Expo CLI Error: 'NativeModules' is not defined in react-native-web

This repository demonstrates a common error encountered when developing Expo apps that target web platforms. The error, "'NativeModules' is not defined," arises from attempting to access native modules within a web-based environment.

## Problem

The `NativeModules` object, a core component of React Native, provides access to platform-specific native modules. However, these modules are unavailable in a web browser context.  Using `NativeModules` directly within code intended for web deployment results in the error.

## Solution

The solution involves conditional logic to prevent accessing `NativeModules` when targeting web. This typically requires checking the environment using `Platform.OS` and conditionally rendering or loading components/code based on the platform.

## Usage

1. Clone the repository.
2. Navigate to the project directory.
3. Install dependencies: `npm install` or `yarn install`
4. Run the app in web mode: `expo start --web`