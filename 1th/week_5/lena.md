# 기간
2021.02.01 ~ 2021.02.07

## 목표

🔥 이번주는 재밌는거 위주로 달립니다 ㅎㅎㅎ 🔥


### 목표 1. 블로그 글쓰기 - 2 개

묵혀놨던 draft 글을 완성하는 위주로 블로그에 글을 작성하려고 합니다. 2개 🤓

- [x] 1 
- [x] 2

| 블로그 글               |
| ------------------ |
| [Swift의 Automatic Reference Counting(ARC) vs Java의 Garbage Collection(GC)](https://lena-chamna.netlify.app/post/automatic_reference_counting_vs_garbage_collection/) |
| [의존성 주입 (Dependency Injection)](https://lena-chamna.netlify.app/post/dependency_injection/) |


### 목표 2. SwiftUI 토이 프로젝트

부담없이 흥미와 자존감을 높이는 '유튜브 보고 SwiftUI 화면 클론 코딩' 1개 🥳 

- [x] 1 

| Github                |
| ------------------ |
|[Custom Inline Curves And Shapes](https://github.com/dev-Lena/SwiftUI/tree/main/CustomInlineCurvesAndShapes) |

<img src = "https://github.com/dev-Lena/SwiftUI/raw/main/CustomInlineCurvesAndShapes/Media/CustomInlineCurvesAndShapes.gif" width = "30%">



### 목표 3. 오픈소스 라이브러리 PR 보내기

- [x] 오픈소스 라이브러리 코드 분석
- [x] 오픈소스 라이브러리 이슈 보내기

| 오픈소스 라이브러리      | PR                |
| ------------------ | ------------------ |
| [YPImagePicker](https://github.com/Yummypets/YPImagePicker) |[Issue](https://github.com/Yummypets/YPImagePicker/issues/633#issue-802872663) |



### 목표 4. 커스텀 프레임워크 만들기

- [x] 프레임워크로 만들 코드 작성
- [x] 프레임워크화 하기

지금 하고 있는 동아리에서 iOS 개발자 한 분과 협업하고 있는데, 모든 뷰에서 사용되는 뷰를 프레임워크로 만들어서 import해서 바로 사용할 수 있도록 구현해봤습니다!

![image](https://user-images.githubusercontent.com/52783516/107142900-4387de80-6975-11eb-85f7-34bc7f714008.png)



## 회고

### 목표 1. 블로그 글쓰기 - 2 개

이펙티브 자바 책으로 [이펙티브 스위프트 스터디](https://github.com/TheSwiftists/effective-swift)하면서 자유분방하게 공부한 내용을 정리하고 있는데요. 

스터디 하면서 개인적으로  

1. 주제 연관성, 적합성을 고려했을 때 주제와 맞지 않아서 스터디 자료에는 적지 않게 됐지만 공부한 내용이 있을 때 아쉽다
2. 스터디 후 수정 / 디벨롭 된 내용을 나의 생각과 함께 기록하고 싶다

는 아쉬움이 있었는데 저번주, 이번주 윜뱈 목표 달성하면서 평소 아쉬웠던 점을 해결했습니다! 스터디를 위한 자료를 만들 때 정리했었거나 스터디 자료로 올린 문서를 블로그에 좀 더 다듬어서 올렸어요! 다음주도 블로그 글 작성을 목표로 할 계획이에요! 

### 목표 2. SwiftUI 토이 프로젝트

유튜브 보면서 만들어보고 싶은 화면을 따라서 만들어보는 클론코딩을 지난주에 이어 하고 있는데, 이번에 SwiftUI로 동아리에서 프로젝트하면서 여기서 클론코딩하면서 배운 걸 아주 유용하게 활용하고 있습니다. 다음주도 할 예정입니다!

### 목표 3. 오픈소스 라이브러리 PR 보내기

ㅎ.. 원래는 PR을 보내고 싶은 오픈소스 라이브러리([AppPear/ChartView](AppPear/ChartView))가 있었어요.
ChartView를 사용했을 때 Touch가 들어온 Row의 value를 알 수 있도록 하고싶었지만 아직 SwiftUI에 익숙하지 않아서 제가 원하는 기능을 구현하지 못했습니다. 

대신에 다른 오픈소스 라이브러리([YPImagePicker](https://github.com/Yummypets/YPImagePicker))에 PR을 보내려고 했는데 Permission Denied 됐어요.😭 그래서 일단 Issue로 남겼습니다!

오픈소스 기여의 시작은 오타수정부터 ㅎ

![image](https://user-images.githubusercontent.com/52783516/107143634-716f2200-6979-11eb-8563-9b5b1f7c4923.png)

달성 결과를 아쉽지만 그래도 목표로 설정해서 어떤거에 PR을 보낼까 고민하면서 여러 개의 오픈 소스 라이브러리를 좀 요모조모 뜯어보고 분석하면서 어떤 기능이 더 있으면 좋을까 고민했던건 의미있었습니다!

### 목표 4. 커스텀 프레임워크 만들기

사실 그냥 Shared 폴더에 View를 하나 만들어서 써도 되지 않을까? 라는 생각에 커스텀 프레임워크를 만들수 있다더라는 카더라만 알고 있고 실제로 만들어본 적은 없는데요. 이번에 목표 설정 덕분에 간단한 프레임워크를 만들어 봤습니다. 자주 쓰는 기능이나 공통으로 쓰는기능들은 중복 코드를 줄이고 협업할 때 효율을 높이기 위해 프레임워크로 만들면 좋은 것 같아요! 한번 만들어보는게 어렵지 앞으로 또 만들어서 사용할 것 같아요! 이번에는 xcodeproj 안에 프레임워크를 만들었는데 나중에는 배포(?)도 해서 다른 분들도 쓸 수 있는 프레임워크를 만들어보고 싶네요!