# test-react-native-callkit
[React] CallKit 예제 따라하기

#### 1. npm react-native 설치
```npm
npm install -g create-react-native-app

or

yarn add create-react-native-app
```


#### 2. react-native 설치
```npm

create-react-native-app project

```

#### 3. build 환경 설정
```npm
// android
// android에서 js build가 가능하게 해주는 역할을 한다.
mkdir android/app/src/main/assets

react-native bundle --platform android --dev false --entry-file index.js --bundle-output android/app/src/main/assets/index.android.bundle --assets-dest android/app/src/main/res

// ios
// ios에서 js build가 가능하게 해준다.

react-native bundle --dev false --entry-file index.js --bundle-output ios/main.jsbundle --assets-dest ./ios --platform ios
```


#### 4. react-native callkeep 설치
```npm
npm install --save react-native-callkeep

or 

yarn add react-native-callkeep


// native 환경에서 사용하는 명령어
react-native link react-natvie-callkeep
```

#### 5. 필요 패키지 설정
```npm
npm install --save uuid
npm install --save react-native-callkeep
npm install --save react-native-background-timer
npm install --save react-native-device-info

react-native link uuid
react-native link react-native-callkeep
react-native link react-native-background-timer
react-native link react-native-device-info

```
