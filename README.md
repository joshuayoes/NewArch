# Turbo Native Modules

Repository to follow along [Turbo Native Modules](https://reactnative.dev/docs/the-new-architecture/pillars-turbomodules) section in The New Architecture docs in React Native.

## Install

_Each code block assumes you are running from root directory_

```bash
cd RTNCalculator
yarn install
cd ../MyApp
yarn install
```

### iOS

```bash
node MyApp/node_modules/react-native/scripts/generate-artifacts.js \
  --path MyApp/ \
  --outputPath RTNCalculator/generated/

cd MyApp/ios
bundle install
RCT_NEW_ARCH_ENABLED=1 bundle exec pod install
```

### Android

```bash
cd android
./gradlew generateCodegenArtifactsFromSchema
```

## Run

### iOS

```bash
cd MyApp
yarn ios
```

### Android

```bash
cd MyApp
yarn android
```
