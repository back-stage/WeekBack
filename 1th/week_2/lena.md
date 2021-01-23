# 기간
2021.01.11 ~ 2021.01.17



## 목표

### PhotoTag 

* 구현 완료

* Team 레포 / iOS 레포 README.md 정리

  * 화면 별 설명 추가하기
    * 영상 찍기 / 스크린샷 촬영
  * 프로젝트 기간 업데이트

  * 로그 시트 링크 추가하기
  * 기술 스택 추가하기



## 회고

음...😢 목표 달성을 위해 이번주에 사용한 시간이 37시간 12분 정도로 들인 시간은 많은편인 것 같다. 

 하지만 예상치 못하게 만난 복병에 몇 일을 소비하면서 목표를 달성하지 못했다. 

새삼 느낀건데 나는 간혹가다 해결하는 데에 몇 일씩 걸리는 문제를 만나곤하는데, 그럴 때 보면 디버깅하는 스킬이나 센스를 더 길러야 겠다는 생각이든다. 

<img src="https://user-images.githubusercontent.com/52783516/104847589-466a5300-5924-11eb-86b5-f5d1c91c1998.png" alt="image" style="zoom: 50%;" />

이번에 애먹은 복병은 이미지 파일을 서버에 올리는 거였는데, 블로그와 stackoverflow에서 코드를 찾아서 이거 저거 써보면서 해결하려고 했지 http 에 대해 이해하고 구현하려고 하지 않았던게 문제였던 것 같다. 사실 이 문제를 어떻게 해결해야할지 도저히 모르겠어서 2일째 고통받고있던 날 다른 친구들한테 물어봤었는데 아주 친절하게 화면 공유로 내 코드 같이 보면서 상의해주던 친구가 나에게 직언을 날려줬다. "지금 문제의 원인을 찾아서 이해하고 해결할려고 하는 것보다 단순히 이 상황에서 벗어나고 싶어하는 것 처럼 보인다"고. 아주 뼈맞았다. 그래서 미련을 버리지 못했던 주석처리된 코드와 관련 코드를 지워버리고 http multipart/form-data에 관련해서 공부부터 하고 [블로그](https://lena-chamna.netlify.app/post/uploading_array_of_images_using_multipart_form-data_in_swift/) 에 정리한 다음에 코드를 수정했다. 마지막 조각은 푸글✨ 덕분에 해결할 수 있었다. 

-> 이 문제를 해결하기 위해 공부한 내용을 정리한 [블로그](https://lena-chamna.netlify.app/post/uploading_array_of_images_using_multipart_form-data_in_swift/)

-> 이 문제를 해결하고 날린 [PR](https://github.com/SimLeeTag/photo-tag-iOS/pull/44) 

푸글이랑 약속한 일들이 있는데 전부다 밀려서 미안하다. 

마음같아서는 얼른 끝내고 싶어서 항상 곧 끝내겠다고 말했는데, 이렇게 말한지 얼마나됐는지 기억이 나질 않는다 😢

하지만 진짜로 거의 다 왔다. 그래도 끝까지 마무리 지어야지 😓



## TIL

### 01.18.Mon TIL
 `git merge dev -s ours`

* 상황:
  1. 브랜치 상황:
     **dev**, **branchA**(내가 PR을 보내서 dev로 merge했었음. 커밋 6개), **branchB**(branchA PR을 revert하면서 생긴 branch임), **branchC**(branchA에서 error를 fix해서 PR을 보냄. 커밋 2개), **branchD**(로컬에서 새로 만든 브랜치)
  2. 진행:
     branchD로 체크아웃
     branchA에 있는 커밋 6개를 cherry-pick으로 가져옴
     branchC에 있는 커밋 2개를 cherry-pick으로 가져옴
     변경 사항을 다 가지고 있는 branchD를 dev로 merge
     이 때 명령어가  `git merge dev -s ours`


[Why would one use “git merge -s ours”?](https://stackoverflow.com/questions/5077688/why-would-one-use-git-merge-s-ours#:~:text=Whenever%20you%20do%20a%20merge,creating%20a%20new%20common%20ancestor.)

## 

### 01.20.Wed TIL

Swift에서 배열 다루기

- 배열의 원소들을 하나로 묶는 방법
  `func joined(separator: String = "") -> String`

  ```swift
  // 기본
  let cast = ["Vivien", "Marlon", "Kim", "Karl"]
  let list = cast.joined(separator: ", ")
  print(list)
  // Prints "Vivien, Marlon, Kim, Karl"
  
  // 활용
  let ranges = [0..<3, 8..<10, 15..<17]
  // 'ranges' 배열에 for-in 루프를 사용하면 각각의 원소에만 접근할 수 있음
  for range in ranges {
      print(range)
  }
  // "0..<3"가 출력됨
  // "8..<10"가 출력됨
  // "15..<17"가 출력됨
  // 'joined()'를 사용하면 각각의 범위에 접근할 수 있음
  for index in ranges.joined() {
      print(index, terminator: " ")
  }
  // “0 1 2 8 9 15 16” 출력
  ```

  [joined(separator:)](https://developer.apple.com/documentation/swift/sequence/1641243-joined)

  [Swift joined 배열의 원소들을 하나로 묶는 방법](https://medium.com/@sunghyun_k/swift-joined-4fcc49098bd0)

- 두 배열 안에 공통 요소 찾는 방법
  [How to get list of common elements of 2 array in Swift?](https://stackoverflow.com/questions/32439289/how-to-get-list-of-common-elements-of-2-array-in-swift)

- 두 배열에서 다른 요소 찾는 방법

  ```swift
  extension Array where Element: Hashable {
      func difference(from other: [Element]) -> [Element] {
          let thisSet = Set(self)
          let otherSet = Set(other)
          return Array(thisSet.symmetricDifference(otherSet))
      }
  }
  
  let names1 = ["John", "Paul", "Ringo"]
  let names2 = ["Ringo", "Paul", "George"]
  let difference = names1.difference(from: names2)
  ```

  [difference between two arrays](https://www.hackingwithswift.com/example-code/language/how-to-find-the-difference-between-two-arrays)

- 시퀀스 안에 값이 포함되어있는지 확인하는 방법
  `func contains(_ element: Element) -> Bool`
  Complexity: **O(*n*)**, where *n* is the length of the sequence.

  ``` swift
  let cast = ["Vivien", "Marlon", "Kim", "Karl"]
  print(cast.contains("Marlon"))
  // Prints "true"
  print(cast.contains("James"))
  // Prints "false"
  ```

  [contains(_:)](https://developer.apple.com/documentation/swift/array/2945493-contains)

- A 시퀀스와 B 시퀀스에 동일한 요소가 동일한 순서로 포함되어 있는지 확인하는 방법
  `func elementsEqual<OtherSequence>(_ other: OtherSequence) -> Bool where OtherSequence : Sequence, Self.Element == OtherSequence.Element`
  Complexity: **O(*m*)**, where *m* is the lesser of the length of the sequence and the length of `other`.

  ```swift
  let a = 1...3
  let b = 1...10
  
  print(a.elementsEqual(b))
  // Prints "false"
  print(a.elementsEqual([1, 2, 3]))
  // Prints "true"
  ```

  [elementsEqual(_:)](https://developer.apple.com/documentation/swift/array/2853688-elementsequal)

  
### 01.22.Fri TIL

오늘 유난히 쓰레드 관련 에러를 많이 봐서 에러 메세지에 나온 내용을 찾아보다가 읽어봤습니다.

이전에 아주 간단하게 공부한 적이 있었는데 이쪽을 뭔가 좀 더 파고 싶네요. 굉장히 재밌어 보여요.

그리고 지금 네트워크에서 data와 image를 비동기적으로 가지고 와서 View에 표시할 때의 타이밍 문제를 계속 마딱드리고 있는데, 현재는 handler와 notificationCenter를 이용해서 타이밍을 맞추고 있지만 추후에 DispatchGroup을 이용할 수 있을 것 같다는 생각이 들었습니다.

* QoS
  1. [Prioritize Work with Quality of Service Classes](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/EnergyGuide-iOS/PrioritizeWorkWithQoS.html)
  2. [iOS ) Prioritize Work with Quality of Service Classes](https://zeddios.tistory.com/521)

* DispatchGroup

  1. [DispatchGroup](https://developer.apple.com/documentation/dispatch/dispatchgroup)
  
  2. [iOS ) GCD - Dispatch Queue사용법 (2) / DispatchWorkItem, DispatchGroup](https://zeddios.tistory.com/520)
  
     

### 01.23.Sat TIL

`@escaping closure`와 `nested function`의 특징에 대해 알아봤습니다.

`completionHandler` 클로저로 서버에서 비동기적으로 받아오는 데이터와 뷰에 표시해주는 타이밍을 맞추고 있다가 `completionHandler`에 `@escaping` 키워드를 붙이지 않았을 때 에러가 나는 걸 보고 이번에 다시 훑어봤습니다.

그리고 기존에 짜 놓은 코드를 살펴보다가 nested function으로 짠 코드가 있는데 문득 retain cycle이 걱정되어서 이것에 대해서도 알아봤습니다.

* `@escaping closure`
  [Escaping Closures](https://docs.swift.org/swift-book/LanguageGuide/Closures.html#ID546)

  [How To: Escaping Closures In Swift With @escaping](https://learnappmaking.com/escaping-closures-swift/)
  [What is @escaping in Swift?](https://www.donnywals.com/what-is-escaping-in-swift/)
  [Completion Handler in Swift with @escaping and @nonescaping closures.](https://medium.com/@dhavalkansara51/completion-handler-in-swift-with-escaping-and-nonescaping-closures-1ea717dc93a4)

* `nested function`
  [Nested Functions in Swift. Real experience](https://alexalmostengineer.medium.com/nested-functions-in-swift-real-experience-88cf00301f0e)

  [Nested Functions](https://docs.swift.org/swift-book/LanguageGuide/Functions.html#ID178)[What is the practical use of nested functions in swift? [duplicate\]](https://stackoverflow.com/questions/32968133/what-is-the-practical-use-of-nested-functions-in-swift)
  
  [What is the practical use of nested functions in swift? duplicate](https://stackoverflow.com/a/41984023)

