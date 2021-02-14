# 기간
2021.02.08 ~ 2021.02.14
( 설날 02.11 ~ 02.13 )

## 목표

### 목표 1. 블로그 글 또는 초고 작성 - 4개 이상(주제는 아래에서 선정)
* 주제 후보: 프레임워크 vs 라이브러리 차이 정리✅/ Delegation 패턴/  SwiftUI 관련✅/ 메모리 관련/ GCD 관련/ 디자인 패턴/ TDD vs BDD

- [x] 1 Swift Generic
- [x] 2 iOS에서 서버에 파일 보내는 이전 포스팅을 2개로 분리(HTTP 이해 /iOS에서 활용 예시) 및 iOS에서의 활용 예시 추가 
- [x] 3 Library vs Framework에 대한 초고 작성
  에버군이 알려준 [우테코 테코톡 영상 참고](https://www.youtube.com/watch?v=We8JKbNQeLo)
  솔라양이 알려준 [영상](https://youtu.be/t9ccIykXTCM)
  참고했습니다!
- [x] 4 SwiftUI Property Wrapper에 대한 초고 작성


| 블로그            |
| ------------- |
| [Swift - Generic](https://lena-chamna.netlify.app/post/introduce_swift_generic/) |
| [multipart/form-data 이용해서 사진/이미지 배열 업로드하기](https://lena-chamna.netlify.app/post/uploading_array_of_images_using_multipart_form-data_in_swift/) |

* 블로그 초고

<img src="https://user-images.githubusercontent.com/52783516/107873289-d89a5280-6ef4-11eb-9fd1-ece2c47106b2.png" alt="image" width="63%;" /><img src="https://user-images.githubusercontent.com/52783516/107873292-e51eab00-6ef4-11eb-912b-0ca7b72c05ab.png" alt="image" width="63%;" />




### 목표 2. SwiftUI 토이 프로젝트

흥미와 자존감을 높이는 '유튜브 보고 SwiftUI 화면 클론 코딩' 1개 이상 🥳 

- [x] [SwiftUI 2.0 Advance Map Kit Tutorials - Core Location - MVVM - Custom Search Bar - SwiftUI Tutorials](https://youtu.be/7HYIe5uHo78)

| Github                | Image |
| ------------------ | ------------------ |
|[AdvanceMapKit](https://github.com/dev-Lena/SwiftUI/tree/main/AdvanceMapKit) |<img src = "https://user-images.githubusercontent.com/52783516/107318898-1c4e2000-6ae1-11eb-9f5a-0a7026759138.png" width = "15%"><img src = "https://user-images.githubusercontent.com/52783516/107318917-23752e00-6ae1-11eb-9d4a-53fb29dd3f09.png" width = "15%"><img src = "https://user-images.githubusercontent.com/52783516/107318931-27a14b80-6ae1-11eb-8441-10f2682e7fb3.png" width = "15%"><img src = "https://user-images.githubusercontent.com/52783516/107318936-2a03a580-6ae1-11eb-8061-93fba5e19a64.png" width = "15%"> |

* 클론 코딩 후보: 
1. [Corona Virus World Metrics App Using JSON Parsing In SwiftUI - Corona Analytics App Using SwiftUI](https://youtu.be/UEjiDemnkoI)
2. [SwiftUI 2.0 Complex App UI - Chat App UI - macOS Tutorials - SwiftUI Tutorials](https://youtu.be/OtzOWYlyt0U)


### 목표 3. 원티드 성장하는 iOS 개발자되기 

- [x] 눕시청

![image](https://user-images.githubusercontent.com/52783516/107178905-8484ff00-6a18-11eb-8798-6e4aadff1c24.png)

* **후기** 🌝 
  세션이 새로운 기술 인사이트를 본인의 지식으로 습득하는 방법, 프로젝트를 여러명이서 같이 개발할 때 생기는 문제점과 해결방법, 지금 당장 (유사)BDD 시작하기  - 간단하게 BDD를 적용해보고 기존과 다르게 개발했던 경험 이렇게 3가지 였습니다.

  이중에 가장 유익하고 흥미로웠던 내용은 원티드 iOS 개발팀에서 사용한다는 CleanSwift 아키텍쳐와 BDD에 대한 내용이었습니다. 지금은 아 이런게 있구나 싶은 정도로만 이해를 했는데 CleanSwift와 BDD도 한번 알아보면 재밌을 것 같네요!

  **인상깊었던 부분**🎯

  > **Clean Swift**
  >
  > * ViewController(UI 디자인)
  >   * 뷰 이벤트를 Interactor에 전달, Presenter가 주는 데이터 표시
  > * Interactor (이벤트 처리)
  >   * 이벤트 처리, 상태 관리, 모든 비즈니스 로직을 담당 /Worker와 협력
  > * Presenter (ViewModel 생성)
  >   * Interactor에서 받은 데이터를 ViewModel로 바꿔서 View에 전달

  > **(유사)BDD**
  > 사용자 관점에서 시나리오를 UseCase로 정리하고, Use Case 별로 Jira 테스크를 생성, 개발하고 Test Case를 작성하여 확인했습니다.
  >
  > * 최종 사용자의 행동 중심 테스트
  > * 비즈니스 요구사항의 검증
  > * 작성된 테스트는 그 자체로도 문서화 (+ QA와 버그 감소)



## 회고

설날이 껴있기도 하고 생각도 많아져서 좀 여유 시간을 가지면서 하려고 했습니다. 😌
이번에 들었던 원티드 성장하는 iOS 개발자되기에서 BDD를 알게 된게 의미있었던 것 같아요.
그리고 블로그하고 SwiftUI 클론 코딩은 사실 WeekBack 목표가 아니었다면 하지 않았을 것 같은데 몇 주째 목표로 설정해놓으니까 매주 하게 되더라구요! WeekBack 덕분에 했습니다.

그리고 알고리즘 바킹독 강의를 듣기 시작했어요! 🤓

개인적으로 인생에 현타가 오는 한 주였습니다. '내가 지금 뭘하고 있는거지, 이러는게 무슨 의미가 있지, 단기적으로는 취업하는게 목표이지만 나는 어떤 곳에서 일하고 싶은거지, 일해서 뭐가 되고 싶은거지' 뭔가 구체적이고 궁극적인 목표가 없다는 느낌이 들어서 공허하더라구요. 이전에는 결말을 알 수 없고 기간도 알 수 없는 취준에 대한 불안감이었다면 이번주에 찾아온 현타는 좀 더 근본적인거 같아요. 여기에다가 좀 더 준비해서 지원해보고 싶다는 생각에 공부를 계속하고 있는데 작년과 비교해서 나는 얼마나 준비되었는가라는 생각이 더해져서 나아진게 들인 시간에 비해 있는건가 싶기도 해서 생각이 더 많아졌습니다. 그럼에도 불구하고 WEEKBACK 목표 덕분에 모든걸 내려놓지 않고 무언가를 할 수 있었던 것 같아요. WeekBack의 순기능 👍🏻

참, 이번에 픽사가 만든 영화 소울을 보고 왔는데 모두에게 강추합니다. 저는 두 번 봤는데 한 번 더 보고 싶어요 👍🏻