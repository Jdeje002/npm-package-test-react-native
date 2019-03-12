
# react-native-test

## Getting started

`$ npm install react-native-test --save`

### Mostly automatic installation

`$ react-native link react-native-test`

### Manual installation


#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `react-native-test` and add `RNTest.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNTest.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNTestPackage;` to the imports at the top of the file
  - Add `new RNTestPackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-test'
  	project(':react-native-test').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-test/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-test')
  	```

#### Windows
[Read it! :D](https://github.com/ReactWindows/react-native)

1. In Visual Studio add the `RNTest.sln` in `node_modules/react-native-test/windows/RNTest.sln` folder to their solution, reference from their app.
2. Open up your `MainPage.cs` app
  - Add `using Test.RNTest;` to the usings at the top of the file
  - Add `new RNTestPackage()` to the `List<IReactPackage>` returned by the `Packages` method


## Usage
```javascript
import RNTest from 'react-native-test';

// TODO: What to do with the module?
RNTest;
```
  # npm-package-test-react-native
