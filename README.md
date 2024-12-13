# React Native Android: Runtime Error - Native Module Linking Issue

This repository demonstrates a common React Native Android bug related to improper linking of third-party libraries with native modules. The application functions correctly on iOS, but crashes on Android due to missing or improperly linked native dependencies.

## Problem Description

When integrating a native module (e.g., a library using platform-specific code), a runtime error can occur on Android.  The app works perfectly on iOS, suggesting a problem specific to the Android build process. This typically happens because the Android build system doesn't correctly include and link the native library components.

## Solution

The solution involves ensuring proper linking and configuration of the native modules within the Android project's build files (specifically, `build.gradle` files). This usually involves adding necessary dependencies, settings, and potentially manual linking steps if the library doesn't automatically handle it.