## React Native CLI로 시작하기

해당 글은 Mac을 기준으로 작성했습니다.

공식 문서 상에서 iOS를 개발하기 위해서는 Expo Go로 생성을 하거나 macOS가 필요하다고 작성되어 있습니다.

### Mac OS로 Android 개발 시작하기

1.  개발 툴 설치 (IDE)
    - InteliJ, Visual Studio Code 등과 같이 Code를 작성할 수 있는 IDE를 설치합니다.
    - 저는 VSCode를 기반으로 작성하겠습니다.
    - [https://code.visualstudio.com/](https://code.visualstudio.com/)
2.  Hombrew 설치

    - Node, Watchman, JDK 등 패키지 설치를 하기위해 Homebrew를 설치합니다.
    - [https://brew.sh/ko/](https://brew.sh/ko/)

    ```
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

3.  Hombrew를 사용하여 Node, Watchman 설치
    - Node 18이상 설치.
    - Watchman
      - 파일 시스템의 변경 사항을 감시하기 위한 Facebook의 도구입니다. 파일이나 디렉토리의 변경을 감지하고, 변경 사항에 따라 사용자가 지정한 행동을 수행하는 데 사용합니다.
      - 파일의 변경을 감지하면, 변경된 파일만을 대상으로 변경사항이 즉시 반영됩니다.

```
brew install node brew install watchman
```

4.  JDK 설치

```
brew tap homebrew/cask-versions
brew install --cask zulu17

# Get path to where cask was installed to double-click installer
brew info --cask zulu17
```

5.  Android Studio 설치
    - [https://developer.android.com/studio?hl=ko](https://developer.android.com/studio?hl=ko)
    - 설치시 아래 3개의 항목이 선택되어 있는지 확인합니다.
      - Android SDK
      - Android SDK Platform
      - Android Virtual Device

6.  Android Studio SDK 설치
    - 위에서 Android SDK를 선택하지 않으셨다면 Android Studio SDK Manager -> SDK Tools 탭에서 설치하실 수 있습니다.

7.  Android_HOME 환경 변수 구성
    - 애뮬레이터를 실행할 수 있도록 아래의 환경변수를 구성합니다.
    - 이때, $HOME은 사용자의 컴퓨터 환경에 맞게 변경해줍니다.
      - SDK Manager의 Android SDK Location에 나와있는 /Library이전의 경로로 변경하여 주시면됩니다.
    - nano ~/.zprofile 또는 ~/.zshrc 또는 ~/.bash_profile 또는 ~/.bashrc 파일 중 한개에서 설정을 변경합니다.

```
export ANDROID_HOME=$HOME/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

8.  npx로 새 애플리케이션 생성
    - 이전에 react-native-cli를 설치한 적이 있으시다면 예상치 못한 에러를 발생할 수 있기때문에 제거합니다.

```
npm uninstall -g react-native-cli @react-native-community/cli
```

- react-native-cli를 설치한 적이 없으시다면 바로 아래 명령어를 통해 생성해주시면 됩니다.

```
# 최신버전
npx react-native@latest init AwesomeProject

# 특정버전
npx react-native@X.XX.X init AwesomeProject --version X.XX.X
```

9.  React Native 애플리케이션 실행
    1.  실행하게 되면 아래 사진과 같은 화면이 나오게 되며 첫 애플리케이션이 실행되게 됩니다.

```
npm start

# 해당 명령어를 실행하다보면 아래와 같은 선택지중 한가지를 선택하시면 됩니다.
i - run on iOS
a - run on Android
d - open Dev Menu
r - reload app
```
<img width="338" alt="스크린샷 2023-12-30 오전 12 13 34" src="https://github.com/homile/React-native-study/assets/56163157/23f3ef35-203e-4ef4-adf0-57c2a703abf3">