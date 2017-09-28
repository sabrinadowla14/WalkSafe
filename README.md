# WalkSafe

> Mobile app on Android and iOS that provides the user crime density heatmap, real time crime updates using SpotCrime API, and many more safety features


## Table of Contents

1. [Team](#team)
1. [Demo](#demo)
1. [Initial Setup](#Initial Setup)
    1. [iOS Setup](#iOS Setup)
    1. [Android Setup](#Android Setup)
1. [Requirements](#requirements)
1. [Development](#development)
    1. [Installing Dependencies](#installing-dependencies)
    1. [Tasks](#tasks)
1. [WalkSafe Server](https://github.com/f-4/WalkSafe-server)
1. [Contributing](#contributing)


## Team

  - __Product Owner__: Fredy-Edwin Esse
  - __Scrum Master__: Rick Gallegos
  - __Development Team Members__: Sonrisa Chen and Brian Kim

## Demo

View the app in action [here](https://www.youtube.com/watch?v=R41ELsbPc04)

## Initial Setup

> __Environment Variables__ WalkSafe requires a Mapbox Access Token to use the Mapbox API on the frontend. We have used the .env package, which allows environment variables to be set easily with the .env file in the root directory of the project. An example of the necessary variables for WalkSafe been provided here in this repo.

> __Backend server and Local Host__ A fair warning when entering in the environmental variables for HOST, PORT, FACEBOOK_URL, and GOOGLE_URL.  These variables should connect to your backend server but emulated Android devices on Android Studio and iOS devices on Xcode run their own local host so setting these environmental variables to route to 127.0.0.1 will have requests that never reach their destination.  Use the appropriate IP address to connect to your backend server.

- Fork and clone the repo

> __NOTE__ Download Xcode and or Android Studio depending on what platform you want to develop on.

### iOS Setup

- [Download](https://developer.apple.com/xcode/) and install Xcode
- INSTRUCTIONS HERE
- Install dependencies from the root of the repo by running
```sh
npm install
```

- Link dependencies to iOS code by running
```sh
react-native link
```
> __NOTE__ If this does not work go to the npm module website for each dependency and follow the Android instructions for manually linking.

- Start backend server
- Start app by running:
```sh
react-native run-ios
```

### Android Setup

- [Download](https://developer.android.com/studio/install.html) and install Android Studio
- Create a WalkSafe project in Android Studio
- Click Tools on the toolbar
- Click Android
- Click AVD Manager
- Create a virtual device
- In Android Virtual Device Manager launch virtual device by double clicking on it
- Install dependencies from the root of the repo by running
```sh
npm install
```
- Link dependencies to Android code by running
```sh
react-native link
```
> __NOTE__ If this does not work go to the npm module website for each dependency and follow the Android instructions for manually linking.

- Start backend server
- Start app by running:
```sh
react-native run-android
```

> __NOTE__ Building and compiling the React Native JavaScript code into Java will initially take a couple of minutes.

> __NOTE__ It is important to not have the android folder nor any of its contents open in your text editor as this may cause the build to fail.

> __NOTE__ After making changes in JavaScript code in your text editor double tap R to reload WalkSafe and have it reflect your new changes!  Push Ctrl + M on the screen to open up the menu to enable remote debugging through Chrome. While debugging it is important to have that Chrome tab in the foreground as it will use up a lot of your computer's resources otherwise.

## Requirements

- Node 0.10.x
- React Native 0.47.0
- [WalkSafe-server](https://github.com/f-4/WalkSafe-server)
- [Xcode](https://developer.apple.com/xcode/)
- [Android Studio](https://developer.android.com/studio/install.html)

## Development

### Installing Dependencies

From within the root directory:

```sh
npm install
```
[Download](https://neo4j.com/download/community-edition), install and run neo4j

### Roadmap

View the project roadmap [here](https://github.com/f-4/WalkSafe/issues)

## WalkSafe Server Repo

View the WalkSafe server repo
[here](https://github.com/f-4/WalkSafe-server)

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for contribution guidelines.
