npm install @capacitor/core
npm install @capacitor/cli --save-dev
npm install @capacity/android
npm install cordova-res -g

steps:
1.构建dist：yarn build
2.添加安卓平台：npx cap add android
3.生成图标和闪屏并添加到项目工程：cordova-res android --skip-config --copy    yarn icon
4.安装测试:  yarn apks    yarn test
          java -jar bundletool-all-1.8.2.jar build-apks --bundle=android/app/release/app-release.aab --output=android/app/release/app-release-test.apks --ks=android/key.jks --ks-pass=pass:000000 --ks-key-alias=key --key-pass=pass:000000
          java -jar bundletool-all-1.8.2.jar install-apks --apks=android/app/release/app-release-test.apks

live coding
"server": {
  "url": "http://192.168.56.1:10888",
  "cleartext": true
}

https://cardgames.io/rummy/
