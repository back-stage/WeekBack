# 기간
2021.01.04 ~ 2021.01.10



### 목표 1: [포토 태그](https://github.com/SimLeeTag/photo-tag-iOS/issues)

- [ ] 프로젝트 마무리. 앱 완성.

### 목표 2: [이펙티브 스위프트 스터디](https://github.com/TheSwiftists/effective-swift)

- [x] 이펙티브 자바 item 34, 37읽기

- [x] item29: 이왕이면 제네릭 타입으로 만들라

  → [generic에 대한 자료](https://github.com/TheSwiftists/effective-swift/pull/64/files?short_path=27e5161#diff-27e51611c81ca8f1476beff3b325a33c773a78fdf380451cb8edb960b3d7753e) 업로드

- [x] item34: int 상수 대신 열거 타입을 사용하라
  → [enum에 대한 자료](https://github.com/TheSwiftists/effective-swift/pull/74/files?short_path=a99983e#diff-a99983e745db76884a38bb59cdc781c673576fb8c293bcb6b3069892e252c2b2) 업로드 

- [x] item37: ordinal 인덱싱 대신 EnumMap을 사용하라 
  → [swift에서 enummap 예시 자료](https://github.com/TheSwiftists/effective-swift/pull/75/files?short_path=65ff1ed#diff-65ff1edd2fdfabc3d23b69730c188a17e88e61c412a8db372220439547a931bb)

### 목표 3: [CS 기초 공부](https://gyoogle.dev/blog/computer-science/operating-system/System%20Call.html)

- OS(Operating System)운영체제
  - [ ] 프로세스와 스레드

  - [ ] 프로세스 주소 공간

  - [ ] 인터럽트(interrupt)

  - [ ] 시스템 콜(system call)



### 회고

무리한 목표를 세웠다.
쏟은 시간은 많지만 목표 달성은 하지 못해서 아쉬웠다.
**다음주에는 사용가능한 시간을 먼저 파악한 후 실현 가능한 목표를 정해야겠다.**

또한, 이번주에는 이펙티브 스위프트 스터디 자료를 만드는 데 몇 일동안 시간이 너무 오래걸린 다는 점을 발견했고
그 이유가 저자가 말하고자 하는 핵심을 파악 그 내용을 Swift/iOS에서도 찾아보는 데 시간이 오래 걸린다는 걸 발견했다. (자료 작성 소재 고르는 것)
다음 스터디에는 발표를 쉬는 주간이지만, 2월에는 **하루에 1-2시간씩 꾸준히** 해보려고 한다.

그리고 1월에 체인지업을 하고 있어 생활패턴은 많이 개선이 되었으나 주어진 시간에 언제 어떤 일을 할 건지에 대한건 개선이 필요했다.
다음주에는 **오전에는 우선순위가 밀리게 되지만 중요한 일(CS 공부, 알고리즘, 문서화 작업)** 을 하고 오후와 밤 시간에는 덩어리 시간을 만들어서 개발 / 개발 공부를 해야겠다고 느꼈다.

마지막으로 1월에 WeekBack을 포함한 새로운 곳에 많이 속하게 되어서 새로 만나게된 사람들과 회의하고 추가적으로 커뮤니케이션하고 새로운 규칙이나 해야할 일을 숙지해야하는게 많았다. 이번주는 이런 일이 매일 매일 있어서 한 일에 집중하는게 어려웠다. 수시로 확인해서 흐름을 깨는 것 보다 쉬는 시간에 정성들여 답장 해야겠다. 그 외의 팀 커뮤니케이션 관련 일들은 오전에 최대한 처리해야겠다.

## TIL

* 2021.01.11.Mon
  xib로 viewController를 만든 후 코드로 불러와 화면을 띄울 때 주의할 점
  1. 이 경우 view와 매칭되는 view controller 클래스는 custom class으로 지정하지 않고 file owner로 지정해야 한다.
  2. file owner의 view와 xib 파일의 view를 연결해줘야 한다. ([stackoverflow](https://stackoverflow.com/questions/4763519/loaded-nib-but-the-view-outlet-was-not-set) 참고)

* 2021.01.11.Tue

  multipart/form-data 타입의 HTTP 메시지 구성 방법
  클라이언트에서 서버에 파일을 업로드할 때, HTTP 요청의 multipart/formdata를 수동으로 구성해주는 방법에 대해 알아봤습니다.
  HTTP 이해하기: [multipart/form-data 타입의 HTTP 메시지 구성 방법](multipart/form-data 타입의 HTTP 메시지 구성 방법), [HTTP multipart/form-data raw 데이터는 어떤 형태일까?](https://lng1982.tistory.com/209)
  iOS 에서 파일 보내기: [[Swift] - MultiPart통신 (멀티파트 이미지업로드)](https://nsios.tistory.com/39), [Uploading images and forms to a server using URLSession](https://www.donnywals.com/uploading-images-and-forms-to-a-server-using-urlsession/), [How to Upload Image to Imgur in iOS using Swift](https://johncodeos.com/how-to-upload-image-to-imgur-in-ios-using-swift/), [Upload image to server using URLSessionUploadTask](https://fluffy.es/upload-image-to-server/)

* 2021.01.13.Wed![image](https://user-images.githubusercontent.com/52783516/104459823-a1ccd600-55f0-11eb-9f7e-545a1d1f6aa1.png)
  (이미지 출처: http://smnh.me/hit-testing-in-ios/)
  View가 겹쳐있을 때 HitTest로 Touch Event 받기
  : UIView에 있는 `hitTest(_:with:)`를 이용하여 가장 top의 있는 view가 touch event를 수신(receive)하지 않는다고 설정하면 그 뒤(behind)에 있는 view가 event를 받을 수 있습니다.
  앱에서 Event를 처리하는 과정

  * [Using Responders and the Responder Chain to Handle Events](https://developer.apple.com/documentation/uikit/touches_presses_and_gestures/using_responders_and_the_responder_chain_to_handle_events)
  * [UIResponder](https://developer.apple.com/documentation/uikit/uiresponder)
  * [UIEvent](https://developer.apple.com/documentation/uikit/uievent)
  * [hitTest(_:with:)](https://developer.apple.com/documentation/uikit/uiview/1622469-hittest)
