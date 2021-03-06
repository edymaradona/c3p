# Contributing
Contributions are welcome, including bug fixes, features, documentation, or samples.

## Building
The following commands from the repo root should build everything:

    npm install
    gulp build

The only exception is that iOS components are skipped when building on Windows, and Windows components are
skipped when building on Mac OS.

## Testing
When possible, features and most bug fixes should include new automated test cases for all applicable platforms
and target app frameworks. And of course, existing tests should continue to pass.

## Test Plugin
Test plugin code is at `test/plugin`. It consists of Android (Java), iOS (Obj-C) and Windows (C++ and C#) code
exposing a variety of API constructs. The test plugin APIs are used as the target for test cases in each of the
test applications.

## Test Applications
Test applications are at `test/app/cordova`, `test/app/reactnative`, and `test/app/xamarin`. Each of the apps
executes a similar suite of automated test cases to validate the test plugin APIs and plugin runtime library.

See [test/app/cordova/README.md](test/app/cordova/README.md) for more details about the Cordova test app.
Similar documents for React Native and Xamarin test apps haven't been written yet.
