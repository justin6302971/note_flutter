# flutter note

## installation

1. homebrew
2. fvm

```bash
# use homebrew to install fvm, can use other method to install fvm depends on your preference
brew tap leoafarias/fvm
brew install fvm

# check available sdk for installation
fvm releases

# install certain version flutter sdk
fvm install 3.7.7
fvm install stable

#check installed versions
fvm list

# add path variables
echo 'export PATH=/Users/yii/fvm/versions/stable/bin:$PATH' >> .zshrc

# 

```
3. flutter


```bash
# check installed status
flutter docker
```

4. xcode 
```bash

sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer
sudo xcodebuild -runFirstLaunch


# open simulator
open -a Simulator
```
5. gem
```bash

sudo gem install activesupport -v 6.1.7.3
sudo gem install cocoapods
# apple silicon chip
sudo gem uninstall ffi && sudo gem install ffi -- --enable-libffi-alloc

```

6. android
``` bash
# download android studio

# access android studio to install Android SDK Command-line Tools
flutter config --android-sdk /Users/justinchien/Library/Android/sdk

flutter config --android-studio-dir /Applications/Android\ Studio.app/

# java issue 
cd /Applications/Android\ Studio.app/Contents/ 
ln -s jbr jre


flutter doctor --android-licenses
```


## project commands
```bash

#create project
flutter create app

#check available devices
flutter devices



```



## reference

1. [stackoverflow suggestion](https://stackoverflow.com/questions/72782659/installing-flutter-using-homebrew)
2. [installation tutorial](https://yiichenhi.medium.com/輕鬆完成flutter開發環境-最新版-3a70e805bd1a)
3. [android studio setup](https://stackoverflow.com/questions/60475481/flutter-doctor-error-android-sdkmanager-tool-not-found-windows)
4. [flutter setup tutorial](https://ithelp.ithome.com.tw/articles/10261640)
5. [jave issue for flutter](https://stackoverflow.com/questions/51281702/unable-to-find-bundled-java-version-on-flutter/68575967#68575967)