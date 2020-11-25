# CodePush-RN-Android
A barebones Android app with React-Native and App Center CodePush

### Setup

`./gradlew assembleRelease` creates the initial release from the ./android folder, places the apk in ./android/app/build/outputs/apk/release/app-release.apk

`appcenter distribute release -f app-release.apk --group Collaborators --app mismith/CodePush-Test` distributes the apk from above to the Collaboratos of the application

`appcenter codepush release-react -a mismith/CodePush-Test -d Production` creates a CodePush of the react-native diff changes as a release

### Local Dev

`npx react-native run-android` intalls the app on a local device/emulator & runs metro server
