# 기간
2021.01.25 ~ 2021.01.31

## 목표

### 블로그 글쓰기 - 2 개

- [x] 1
- [x] 2
| 제목    | 링크 |
| ------------- | ---- |
| Hit-Testing in iOS | [Hit-Testing in iOS](https://lena-chamna.netlify.app/post/hit_testing_in_ios/) |
| Hit test 사용하기 | [Hit test 사용하기](https://lena-chamna.netlify.app/post/practical_use_of_hit_test/) |

 (블로그에 적힌 날짜는 draft 날짜입니다. 실제 작성 후 업로드는 이번주차에 했어요!)

### 알고리즘 풀기 - 2 문제

- [x] 1
- [x] 2


| 문제       | 제출 |
| ------------- | ---- |
| leetcode - 88. Merge Sorted Array | [leetcode - 88. Merge Sorted Array](https://leetcode.com/problems/merge-sorted-array/) |
| leetcode - 202. Happy Number | [leetcode - 202. Happy Number](https://leetcode.com/problems/happy-number/) |



## 회고

이번주 저의 최고 목표는 회복이었습니다. 템포를 늦추고 쉬면서 하니까 좋더라구요 🌝 

1. 제가 3주차 TIL 에도 적었는데 그동안 관심있었지만 우선순위에 밀려서 못보고 있었던 SwiftUI나 이벤트를 처리할 UIView 객체를 찾는 방법, 메모리 등 재밌는 주제들을 공부해 봤습니다. 비록 저번주 목표달성 벌칙으로 한 TIL이지만 TIL 작성하면서 되게 재미있었어요.👻 

2. 10-20분 남짓되는 유튜브 보면서 SwiftUI로 짧게 짧게 화면 만들어보는거 재미있는것 같아서 다음주에 또 해보려고 합니다. 

3. 블로그를 쓰면 개발 및 구현에 치중하는 것을 방지해서 개발과 학습의 밸런스를 맞출 수 있는 것 같아요. 뭔가 공부한 걸 기록하기는 하지만 어찌됐든 public으로 남기려면 최대한 검증하고 정리해서 해야하니까 공들여서 공부하고 정리하게 되더라구요. (그래서 더 안쓰게 되는것도 있지만요ㅠ) 블로그 글도 많지 않은데 왜인지 모르겠지만 주기적으로 제 블로그 글 보고 연락이 종종 오는 것 같아서 블로그에 취미를 붙여볼까 합니다. 사실 블로그 글쓰는거 재밌는것 같아요 ㅎㅎㅎ

4. 터치 이벤트가 발생했을 때 이벤트를 처리할 UIView 객체를 찾아가는 과정에 대해 공부했습니다.
   hit-testing에 대한 블로그 글을 쓰면서 알아보던 중 읽은 글에서 이벤트를 처리할 UIView 객체를 찾는 프로세스에서 reverse pre-order depth-first traversal algorithm 을 쓴다고 하는데 흥미로웠어요. 제가 잠깐 찾아보고 이해한 바로는 깊이 우선 탐색 알고리즘의 변형? 응용? 버전인것 같은데요. (DFS)

   <img src="https://miro.medium.com/max/1680/0*miG6xdyYzdvrB67S.gif" alt="Breadth-first vs Depth-first Tree Traversal in Javascript | by Kenny Hom |  Medium" width="70%;" />
   hit-testing에서 이벤트를 처리할 UIView 객체를 찾아가는 과정이 이렇거든요. 
   <img src="http://d33wubrfki0l68.cloudfront.net/60d215400d2340e2334016ea6914aef24cfe6939/d4938/images/hit-test-depth-first-traversal.png" alt="계층 깊이 우선 순회보기" width="70%;" />

   오 뭔가 흥미로웠습니다. 재밌네요 👻 뭔가 좀더 이쪽으로 파서 공부해보고 싶은 마음이 들었어요. 알고리즘을 공부하거나 직접 구현해보면 재밌을 것 같아요.  

5. 알고리즘은 진짜 약간 나랑 동떨어져있다는 느낌을 많이 받았었는데 이렇게 실사용 예를 보니까 엄청 흥미가 생기네요. 그런 의미로 이번주 목표였던 알고리즘은 warm up 의 의미로 지난번에 풀었던 문제를 복습해봤습니다 (난이도 Easy ㅎ)

6. 그리고 저번에 제이를 통해 눕강이라는 좋은 걸 알게됐는데 눕강이 꽤나 장점이 큰것 같아요. 뭔가 본격적으로 정리하고 꼼꼼히 이해하면서 보려고 하니까 정말 시작을 안하게 되더라구요. WWDC(Apple Worldwide Developers Conference) 영상 보기가 저한테는 그렇거든요. 근데 눕시청을 하니까 뭔가 맘편하게 보게 되더라구요. 오히려 한번 보고나니까 의욕이 생겨서 아 이거 다시 정리하면서 보고싶다라는 의지가 생겼습니다 👍🏻

7. 퍼센트 플래너를 작성하면서 이제 제가 시간을 어떻게 쓰는지 파악한지도 한 달 정도 된것 같아요. 1월을 빗대어서 표현하자면 턱끝까지 폭식한 느낌인데요. 왜 그럴까 원인을 좀 생각해봤어요. 그러다가 퍼센트 플래너로 제 시간 사용을 돌아보면서 느낀점은 제 시간의 주체가 제가 아니라 외부요소인 것 같더라구요. 새로 들어간 동아리나 아니면 체인지업 스터디나 아니면 이펙티브 스위프트 스터디, 크로스핏 수업 등등. 하루에 제가 쓸 수 있는 시간은 정해져있는데 다른 사람들과의 약속을 우선순위 최상단에 두다 보니까 다른 사람과 연관되어있지 않은 나만의 일은 영원히 계속 뒤로 밀리더라구요. 그래서 다음주인 2월부터는 개선해야겠다는 생각이 들었습니다. 어떤걸 학습하거나 개발할 때는 덩어리 시간을 만들어서 하는게 중요하다고 생각하는데 다음 주차부터는 덩어리 시간을 확보하려고 노력하려구요.

8. WeekBack을 시작하고 이번 주차에 처음 목표달성을 해봤습니다. 윜뱈 멤버분들이 '목요일이나 금요일 기준으로 할 수 있는 목표를 세우면 목표 달성할 수 있다'라는 팁을 주셨는데 아주 적절한 꿀팁인 것 같습니다. 다음 주차 목표를 세울 때도 그렇게 해야겠어요!

9. toggl 이라는 앱으로 생산적인 활동에 대한 타임 트래킹도 하고 있는데, 지난주까지는 내가 어디에 시간을 썼는지 파악하는 용도로만 썼었습니다. 그런데 유튜브에서 [한 영상](https://youtu.be/a5k_UIz94ys) 을 봤는데 프리랜서인 분이 시간을 돈으로 환산해서 계산을 하더라구요. 뭔가 시간은 금이다라고하지만 진짜 시간을 돈으로 환산해서 계산하고 중요도를 나누고 이렇게 접근하는게 신선하더라구요. 그래서 이번주에는 toggl로 타임 트래킹을 하면서 '이 일은 30분 정도 안에 끝낼만한 일 30분이 여의치 않다면 50분 안에는 끝내야 돈(시간)이 아깝지 않다' 라는 마음으로 했었는데 그러다보니까 집중도와 효율이 개선된 것 같아요. 👍🏻



## 이번주 TIL 

### 01.26.Tue TIL

유튜브를 보고 SwiftUI로 Bar Graph를 만들어봤습니다. -> [Github](https://github.com/dev-Lena/SwiftUI/tree/main/ChartPractice)

<img src="https://github.com/dev-Lena/SwiftUI/raw/main/ChartPractice/Media/swiftui_chart_light_mode.gif" alt="img" width="20%">

### 01.28.Thu TIL

SwiftUI에서 사용되는 프로퍼티 래퍼(Property Wrapper)에 대해 알아봤습니다. (@State의 역할 등)

1. [A guide to SwiftUI’s state management system](https://www.swiftbysundell.com/articles/swiftui-state-management-guide/)
2. [What does the SwiftUI `@State` keyword do?](https://stackoverflow.com/questions/56438730/what-does-the-swiftui-state-keyword-do)
3. [Understanding of Property Wrappers in SwiftUI](https://medium.com/mindful-engineering/understanding-of-property-wrappers-in-swiftui-3789a72515c0)



### 01.29.Fri TIL

[WWDC 2018 iOS Memory Deep Dive](https://developer.apple.com/videos/play/wwdc2018/416/) 눕시청했습니다. 눕시청했는데 내용이 좋아서 나중에 다시 보며 정리할 예정입니다!



### 01.30.Sat TIL

터치 이벤트가 발생했을 때 이벤트를 처리할 UIView 객체를 찾아가는 과정에 대해 공부했습니다.
hit-testing에 대한 블로그 글을 쓰면서 알아보던 중 읽은 글에서 이벤트를 처리할 UIView 객체를 찾는 프로세스에서 reverse pre-order depth-first traversal algorithm 을 쓴다고 하는데 흥미로웠습니다. 제가 잠깐 찾아보고 이해한 바로는 깊이 우선 탐색 알고리즘의 변형? 응용? 버전인것 같은데요.

<img src="https://miro.medium.com/max/1680/0*miG6xdyYzdvrB67S.gif" alt="Breadth-first vs Depth-first Tree Traversal in Javascript | by Kenny Hom |  Medium" width="70%;" />
<br>여기서 왼쪽 DFS가 깊이 우선 탐색 알고리즘인데
<img src="http://d33wubrfki0l68.cloudfront.net/60d215400d2340e2334016ea6914aef24cfe6939/d4938/images/hit-test-depth-first-traversal.png" alt="계층 깊이 우선 순회보기" width="70%;" />

이벤트를 처리할 UIView 객체를 찾아가는 과정이 이렇거든요.

오 뭔가 흥미로웠습니다. 재밌네요 👻

1. [hitTest:withEvent:](https://developer.apple.com/documentation/uikit/uiview/1622469-hittest?language=objc)
2. [hitTest(_:with:)](https://developer.apple.com/documentation/uikit/uiview/1622469-hittest)
3. [Hit-Testing in iOS](http://smnh.me/hit-testing-in-ios/)



 ([TIL](https://github.com/back-stage/WeekBack/pull/34#issuecomment-770243534)에도 남겼습니다!)

