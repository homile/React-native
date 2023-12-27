# React native란 무엇인가?

**React Native는 Facebook에서 개발하고 관리하는 오픈 소스 모바일 애플리케이션 프레임워크입니다. 이 프레임워크는 웹 개발에 사용되는 JavaScript와 React를 기반으로 하고 있으며, iOS와 Android 모두에서 사용할 수 있는 앱을 만들 수 있습니다.**

# React native의 장점/특징

**React Native는 한 번의 개발로 iOS와 Android 모두에 대응할 수 있는 앱을 만들 수 있습니다. 이는 개발 시간을 줄이고, 유지 보수를 간편하게 합니다.**

**React Native는 JavaScript를 사용합니다. 따라서 웹 개발자들은 모바일 개발에 진입하는 데 높은 진입 장벽을 느끼지 않을 것입니다.**

# React native vs Flutter

## **React Native**

**React Native는 Facebook에서 개발한 오픈 소스 프레임워크로, JavaScript와 React를 사용하여 iOS 및 Android 애플리케이션을 개발할 수 있습니다. React Native는 기존의 React 웹 개발 경험을 바탕으로 배우기 쉽고, 빠르게 개발할 수 있다는 장점이 있습니다. 또한, React Native는 이미 많은 개발자가 사용하고 있기 때문에, 다양한 리소스와 지원을 받을 수 있습니다.**

## **Flutter**

**Flutter는 Google에서 개발한 오픈 소스 프레임워크로, Dart 언어를 사용하여 iOS 및 Android 애플리케이션을 개발할 수 있습니다. Flutter는 성능이 뛰어나고, 반응성이 좋으며, 다양한 플랫폼에 일관된 사용자 경험을 제공할 수 있다는 장점이 있습니다. 또한, Flutter는 아직 개발 초기 단계이지만, 빠르게 성장하고 있으며, Google의 적극적인 지원을 받고 있습니다.**

**실제로 채용공고를 보더라도 23년 상반기에는 React Native를 사용하는 곳이 많았지만 하반기로 올 수록 Flutter를 사용하는 기업이 늘어난다는 것을 확인할 수 있었습니다.**

## **차이점**

React Native와 Flutter의 주요 차이점은 다음과 같습니다.

| 특징 | React Native | Flutter |
| --- | --- | --- |
| 언어 | JavaScript, React | Dart |
| 빌드 방식 | JavaScript 코드를 네이티브 코드로 변환 | Dart 코드를 네이티브 코드로 변환 |
| 성능 | 뛰어나지 않음 | 뛰어남 |
| 반응성 | 뛰어나지 않음 | 뛰어남 |
| 플랫폼 호환성 | iOS, Android | iOS, Android |
| 개발 난이도 | 낮음 | 중간 |
| 커뮤니티 | 활발함 | 활발함 |

## **장단점**

React Native와 Flutter의 장단점은 다음과 같습니다.

| 특징 | React Native | Flutter |
| --- | --- | --- |
| 장점 | 배우기 쉽고, 빠르게 개발할 수 있음, 다양한 리소스와 지원을 받을 수 있음 | 성능이 뛰어나고, 반응성이 좋으며, 다양한 플랫폼에 일관된 사용자 경험을 제공할 수 있음 |
| 단점 | 성능이 뛰어나지 않고, 반응성이 뛰어나지 않음 | 개발 난이도가 높음, 커뮤니티가 아직은 크지 않음 |

## **비교**

React Native와 Flutter는 모두 뛰어난 기능을 제공하는 모바일 프레임워크입니다. 프로젝트에 가장 적합한 프레임워크를 선택하기 위해서는 다음과 같은 요소를 고려해야 합니다.

- **프로젝트의 규모 및 복잡도:** 규모가 크고 복잡한 프로젝트의 경우, Flutter의 성능과 반응성이 더 유리할 수 있습니다.
- **개발자의 기술 수준:** React Native는 배우기 쉽지만, Flutter는 개발 난이도가 높습니다.
- **프로젝트의 요구 사항:** React Native는 다양한 리소스와 지원을 받을 수 있다는 장점이 있습니다.

# React native 생성하기

React Native를 생성할 때는 Expo Go와 React Native CLI 두 가지 방법이 있습니다.

## **Expo Go**

Expo는 React Native를 기반으로 한 오픈 소스 프레임워크 및 개발 환경입니다. Expo를 사용하면 React Native를 더 쉽게 시작하고 관리할 수 있으며, 앱 개발을 더 빠르게 진행할 수 있습니다.

Expo의 주요 장점은 다음과 같습니다.

- **빠른 시작:** Expo는 기본 설정이 다 구성되어 있으며 native 파일을 숨겨놓고 자동으로 관리를 해줍니다. 또한 개발을 쉽게 해주는 많은 편리하고 유용한 특성을 가지고 있습니다.
- **간편한 개발:** Expo는 React Native의 기본적인 기능을 제공하며, 추가적인 설정이나 작업이 필요하지 않습니다. 따라서 React Native의 기본을 배우는 중간 또는 초보 개발자에게 유용합니다.
- **빠른 배포:** Expo는 웹 브라우저를 통해 앱을 실행할 수 있으며, iOS 및 Android에 앱을 쉽게 배포할 수 있습니다.

Expo의 주요 단점은 다음과 같습니다.

- **자유도가 낮음:** Expo는 기본적인 기능만 제공하며, 더 많은 기능을 추가하기 위해서는 Expo SDK를 사용해야 합니다. 따라서 복잡한 기능이나 더 높은 사용자 지정을 필요로 하는 프로젝트에는 적합하지 않을 수 있습니다.
- **앱 크기가 크다:** Expo는 모든 Expo SDK 솔루션으로 빌드되어 앱의 크기가 크다는 단점이 있습니다.

## React Native **CLI**

CLI는 React Native의 기본 빌드 도구입니다. CLI를 사용하면 React Native 앱을 직접 생성하고 관리할 수 있습니다.

CLI의 주요 장점은 다음과 같습니다.

- **자유도가 높음:** CLI는 Expo와 달리 기본적인 기능만 제공하지 않습니다. 따라서 개발자가 원하는 모든 기능을 추가할 수 있습니다.
- **앱 크기가 작다:** CLI는 Expo와 달리 앱의 크기가 작다는 장점이 있습니다.

CLI의 주요 단점은 다음과 같습니다.

- **배우기 어렵다:** CLI는 Expo와 달리 기본 설정이 되어 있지 않습니다. 따라서 React Native의 기본을 이해하고 있어야 합니다.
- **개발 시간이 오래 걸린다:** Expo와 달리 CLI는 기본적인 기능을 제공하지 않기 때문에, 개발자가 직접 추가해야 합니다. 따라서 개발 시간이 오래 걸릴 수 있습니다.

## **생성 방법**

### **Expo**

Expo를 사용하여 React Native 앱을 생성하는 방법은 아래와 같다.

1. 다음 명령을 실행하여 앱을 생성합니다.

```bash
npx create-expo-app AwesomeProject

cd AwesomeProject
npx expo start
```

이 명령은 다음과 같은 폴더를 생성합니다.

`my-app/
├── app.json
├── package.json
└── src/`

### React Native **CLI**

React Native CLI를 사용하여 React Native 앱을 생성하는 방법은 아래와 같다.

1. 개발 툴 설치 (IntelliJ, Visual Studio Code 등 IDE)
    1. React, Next.js를 개발 할 때 주로 사용했던 Visual Studio Code를 설치하였습니다.
2. Node.js 설치
3. Android Studio 설치
    1. Expo 같은 경우는 자체에 에뮬레이터를 가지고 있지만 React Native CLI로 개발을 할 경우 에뮬레이터를 가지고 있지 않습니다. 그렇기 때문에 에뮬레이터를 설치해주어야 테스트를 할 수 있습니다.
4. JDK 설치
    1. Android Studio를 사용하기 위해 설치해야한다.
        
        ```bash
        brew tap homebrew/cask-versions
        brew install --cask zulu17
        
        # Get path to where cask was installed to double-click installer
        brew info --cask zulu17
        ```
        
    2. Java Version 확인
        
        ```bash
        java -version
        ```
        
    3. 
5. 특정 버전을 사용하여 다운로드한 CLI을 제거한다.
    
    이전에는 CLI을 따로 설치해야했지만 현재 npx react-native <command>명령이 실행될 때 CLI의 현재 안정 버전이 다운로드되어 실행됩니다. 그렇기 때문에 충돌이 날 수 있기에 아래와 같은 명령어를 사용하여 CLI을 제거합니다.
    설치한적이 없다면 건너뛰어도 됩니다.
    

```bash
npm uninstall -g react-native-cli @react-native-community/cli
```

1. 다음 명령을 실행하여 앱을 생성합니다.

```bash
npx react-native@latest init AwesomeProject
```

이 명령은 다음과 같은 폴더를 생성합니다.

`my-app/
├── android/
│   ├── app/
│   │   ├── build.gradle
│   │   ├── ...
│   │   └── ...
│   └── ...
├── ios/
│   ├── App.xcodeproj
│   ├── ...
│   └── ...
├── package.json
└── src/`