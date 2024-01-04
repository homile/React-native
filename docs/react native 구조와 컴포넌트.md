# React Native 폴더 구조

- android: 안드로이드 네이티브 폴더
- ios: ios 네이티브 폴더
- node_modules: 노드 라이브러리
- app.json: name은 앱 컴포넌트 이름이니 함부로 바꾸면 안 됨, 이거 바꾸면 네이티브 컴포넌트 이름도 다 바꿔야함, displayName은 앱 이름 변경용
- ios/FoodDeliveryApp/AppDelegate.mm 의 moduleName
- android/app/src/main/java/com/fooddeliveryapp/MainActivity.java 의 getMainComponentName
- babel.config.js: 바벨 설정
- index.js: 메인 파일
- App.tsx: 기본 App 컴포넌트
- metro.config.js: 메트로 설정 파일(웹팩 대신 사용)
- tsconfig.json: 타입스크립트 설정
- android/app/src/main/java/com/fooddeliveryapp/MainActivity.java: 안드로이드 액티비티에서 js엔진 통해 리액트 코드 실행 + bridge로 소통

# React Native 코드 폴더 구조

- src 폴더 생성(지금 바로 생성 안 하고 폴더 안에 파일이 들 때 생성해도 됨)
- src/assets: 이미지, 폰트 등
- src/constants: 상수
- src/pages: 페이지 단위 컴포넌트
- src/components: 기타 컴포넌트
- src/contexts: context api 모음
- src/hooks: 커스텀 훅 모음
- src/modules: 네이티브 모듈
- src/store: 리덕스 스토어 세팅
- src/slices: 리덕스 슬라이스
- types: 타입 정의

# React Native 기본 컴포넌트

## App.tsx

- React로 만든 프로젝트를 React Native로 그대로 옮겨와서 사용할 수 없다.
- 다크모드를 지원한다.

  ```ts
  const isDarkMode = useColorScheme() === "dark";
  ```

- 기본적으로 style은 CSS 기반이다.
- 웹에서 사용하는 px 단위가 아닌 dp(density-independent pixel) 단위를 사용한다.
  - dp 단위(density-independent pixels, 다양한 화면 크기에 영향받지 않음)
  - dp = px \* 160 / ppi
  - px = dp \* ppi / 160
- flex에서는 flexDirection이 Column이 default
- View가 div, Text가 span이라고 생각하기(1대1 매칭은 아님)

  ```ts
  <View>
    <Text>Hello world!</Text>
  </View>
  ```

- SafeAreaView
  - 중첩된 콘텐츠를 렌더링하고 자동으로 패딩을 적용하여 탐색 모음, 탭 모음, 도구 모음 및 기타 상위 뷰로 덮이지 않은 뷰 부분을 반영한다.
  - 패딩이 둥근 모서리나 카메라 노치
- StatusBar
  - 앱의 상태 표시줄을 제어하는 ​​구성요소입니다. 상태 표시줄은 일반적으로 화면 상단에 있는 영역으로, 현재 시간, Wi-Fi 및 셀룰러 네트워크 정보, 배터리 잔량 및/또는 기타 상태 아이콘을 표시한다.
- ScrollView
  - 실제 공간보다 컨텐츠가 많을 경우 스크롤 할 수 있게 한다.
- FlatList
  - ScrollView를 사용했을 때 컨텐츠가 많을 경우 렌더링 속도가 느려지고 메모리 사용량이 증가하는 것을 대체하기 위해 사용한다.
  - 항목, 여러 열, 무한 스크롤 로딩 또는 기본적으로 지원하는 기타 기능 사이에 구분 기호를 렌더링하려는 경우에도 사용된다.
