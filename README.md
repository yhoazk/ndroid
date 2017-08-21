# ndroid
Learning materials, practices and resoruces for android development



For the error in idea.log when trying to create an AVD:

[https://stackoverflow.com/questions/29112107/how-to-solve-unable-to-run-mksdcard-sdk-tool-when-installing-android-studio-on?rq=1](https://stackoverflow.com/questions/29112107/how-to-solve-unable-to-run-mksdcard-sdk-tool-when-installing-android-studio-on?rq=1)
For Fedora:
```
sudo dnf install  compat-libstdc++-296.i686 compat-libstdc++-33.i686 ncurses-libs.i686 compat-libstdc++-33.x86_64
sudo dnf install  zlib.i686 ncurses-libs.i686 bzip2-libs.i686
```


## Debug with ionic

The command:
```
ionic cordova build android --prod --release
```

Instructs to eliminate the debug mode in the apk, so there's no way to see the app running in `chrome://inspect/#devices`
in order to see the process run the command as:

```
ionic cordova build android 
```

An apk will be generated in:
```
$approot/platforms/android/build/outputs/apk/android-debug.apk
```
The apk should be available in chrome by visiting: `chrome://inspect/#devices`
