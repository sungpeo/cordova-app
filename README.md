# cordova-app

## Development Environment
 - macOS Mojave
 - XCode 10.x
 - npm

## Prerequite

 - sudo npm install -g cordova


### Install pre-requisites for building
Ref.
https://cordova.apache.org/docs/en/latest/guide/cli/#install-pre-requisites-for-building
https://medium.com/chequer/cordova-환경-구성-git-ignore-설정-61d057bd1b59

``` bash
cordova prepare

cordova requirements
```

## cordova emulate ios
``` bash
cordova emulate ios --buildFlag="-UseModernBuildSystem=0"
```

## cordova emulate android
Ref.
https://cordova.apache.org/docs/en/latest/guide/platforms/android/index.html#requirements-and-support

For emulating android, you should install Android Studio. Then, open SDK Manager to install SDK Platform, AVD Manager to install avd.

In my case, I used Pixel 2 API 27 for Android Virtual Device.

``` bash
cordova emulate android  # emulate android virtual device
cordova emulate          # refreshes the emulator image to display the lastest application.
```

## cordova serve
Ref.
https://cordova.apache.org/docs/en/latest/reference/cordova-cli/#cordova-serve-command

Run a local web server for www/ assets using specified port for default of 8000. Access projects at: http://HOST_IP:PORT/PLATFORM/www

 - I think this is the easiest way to test my app via corodva.

```
cordova serve [port]
```


