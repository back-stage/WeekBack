# 기간
2021.03.01 ~ 2021.03.07

## 목표

### 목표 1. Photo Tag 와 Daymoji 공통 부분 Public Library로 구현

Photo Tag 리팩토링 + Daymoji 처음부터 구현

- [ ] Library로 구현

(Network Manager, Use Case, End Point, Partial Sheet, Card View)

### 목표 2. 운동
- [x] Metcon 수업 (2021.3.3.Wed)
- [x] Metcon 수업 (2021.3.5.Fri)
- [x] 남산 정상 다녀오기

<img src="https://user-images.githubusercontent.com/52783516/109970310-4093ca00-7d38-11eb-8e12-25bf007b4440.png" alt="image" width="30%;" /><img src="https://user-images.githubusercontent.com/52783516/109970386-54d7c700-7d38-11eb-90e9-19381872011f.png" alt="image" width="30%;" /><img src="https://user-images.githubusercontent.com/52783516/110151635-0f90c380-7e24-11eb-9f2b-2998d633e976.png" width="50%;" />

### 목표 3. 기술 면접 질문 4개 답변 정리
- [x] 1
- [x] 2
- [x] 3
- [x] 4

<img src="https://user-images.githubusercontent.com/52783516/109969409-33c2a680-7d37-11eb-9e80-c7361b93001d.png" width ="70%;" />

### 목표 4. 지원하기
- [ ] 1
- [ ] 2



## 회고

1. 지금 우선순위가 뭔지 어떤걸 해야하는지 정리가 안되고 계속 큐에 쌓여만 가서 무기력해진 것 같네요.

2. 라이브러리를 만드는 걸 너무 만만하게 생각했던 것 같아요.

3. 클럽하우스에서 iOS 개발자 모임을 들었는데 후... 준비해야할 게 점점 더 많아지는 것 같아요 😢

4. 면접 질문 정리하는건 이전에 공부했던 내용을 다시 읽고 정리해봤는데 다시보니까 또 새로운 느낌이더라구요



## TIL



### 2021.03.08.MON TIL

LeetCode 문제 풀다가 stride 메서드라는걸 알게 됐습니다.

`stride(from:to:by:)` : from 에서부터 by의 간격으로 to "미만"의 범위에서 반복 연산을 수행한다.
`stride(from:through:by:)`: from 에서부터 by의 간격으로 through "이하"의 범위에서 반복 연산을 수행한다.

참고: [Stride](https://developer.apple.com/documentation/swift/memorylayout/2429192-stride), [stride(from:to:by:)](https://developer.apple.com/documentation/swift/1641347-stride), [stride(from:through:by:)](https://developer.apple.com/documentation/swift/1641185-stride), [Swift 문서, Strideable 프로토콜 및 stride 사용법](https://0urtrees.tistory.com/144)

### 2021.03.09.TUE TIL

LeetCode 문제 풀다가 투 포인터 (Two pointer) 알고리즘이라는 걸 알게 됐습니다.
이중 루프를 돌아야 하나 그럼 복잡도가 n제곱인데... 하면서 발을 동동 구르고 있었는데
투 포인터라는 아이디어가 있더라구요!

- 두 개의 포인터를 사용하는 알고리즘. 여기서 포인터는 C/C++의 포인터가 아니라, 어느 위치를 가르키는 개념적인 포인터다.

- 문제 조건이 연속/선행적으로 무언가를 해야할때 사용된다. 대부분이 아래 3가지 경우에 속한다.

**Collision** - One array, move from two sides to middle.
**Forward** - One array, both move forward.
**Parallel** - Two arrays, each array has been assigned with a pointer
- 슬라이딩 윈도우와 개념이 비슷하다.

<img src="https://blog.kakaocdn.net/dn/1GfnX/btqEK8Tg8Wf/55QuJ9YYKk97mwqcr3h9zK/img.png" alt="img" width="50%;" />

1번 경우인 Collision에 속하는 문제. 두 수의 합이 40과 같은지를 찾는다. 한 수가 40보다 크면 포인터를 중앙으로 옮기고, 40보다 작아지면 다른 포인터를 옮겨보는 방식.

참고:[투포인터 알고리즘](https://github.com/WooVictory/Ready-For-Tech-Interview/blob/master/Algorithm/%ED%88%AC%ED%8F%AC%EC%9D%B8%ED%84%B0%20%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98.md),  [[ 알고리즘 ] 투 포인터 알고리즘](https://developingbear.tistory.com/153)

### 2021.03.10.WED TIL

요즘 알고리즘 풀면서 Map, FlatMap, CompactMap 을 자주 쓰고 자주 접하는데 flatmap과 compactMap 에 대한 차이를 정확히 찾아봤습니다.

* map: `map`은 배열 내부의 값을 하나씩 `mapping` 합니다.
  각 요소에 대한 값을 `변경`하고자 할때 사용하고, 그 결과들을 `배열의 상태로 반환`합니다.
* flatMap 과 compactMap
**Swift 4.1부터는 flatMap이 compactMap로 변경되지만, flatMap이 없어지는 것이 아닙니다.** 4.1 버전 이후로는 쓰임이 구별됩니다.

  기존의 `flatMap`의 경우에는 배열을 `1.flatten하게` 만들어 주며 `2.nil을 제거`, `3. 옵셔널 바인딩`해주는 역할이였습니다. 위의 소스를 작성해보시면 이런 경고창이 뜨실겁니다.

  > *‘flatMap’ is deprecated: Please use compactMap(**:) for the case where closure returns an optional value
  > Use 'compactMap(**:)’ instead*
  > 

  -> 즉, Swift 4.1부터는 `1차원 배열`에서 `nil을 제거`하고 `옵셔널 바인딩`을 하고싶으실때는 `compactMap`을 사용하시면 됩니다.
  
  ➕  flatMapt과 compactMap은 nil을 제거하지않고 1차원 배열일때만 nil제거합니다.

  * **flatMap**: flatMap은 2차원배열을 1차원배열로 flatten 하게 만들어주는 반면, compactMap은 1차원 배열로 만들지 않습니다. 2차원 배열을 1차원으로 flatten하게 만드실때 flatMap을 사용
  * **compactMap**: 1차원 배열에서 nil을 제거하고 옵셔널 바인딩을 하고싶으실때는 compactMap을 사용

```swift
let array2: [[Int?]] = [[1, 2, 3], [nil, 5], [6, nil], [nil, nil]]
let flatMapTest2 = array2.flatMap { $0 }.compactMap{ $0 }

// result: 
// flatMapTest2 : [1, 2, 3, 5, 6]
```

참고: [[Swift] 고차함수(2) - map, flatMap, compactMap](https://jinshine.github.io/2018/12/14/Swift/22.%EA%B3%A0%EC%B0%A8%ED%95%A8%EC%88%98(2)%20-%20map,%20flatMap,%20compactMap/), [Map, FlatMap and CompactMap](https://www.swiftbysundell.com/basics/map-flatmap-and-compactmap/)


### 2021.03.11.THU TIL
알고리즘 풀면서 알게된 string에서 공백(whitespace) 없애는 함수

[trimmingCharacters(in:)](https://developer.apple.com/documentation/foundation/nsstring/1415462-trimmingcharacters)
: Returns a new string made by removing from both ends of the receiver characters contained in a given character set.
**Discussion**: Use whitespaces or whitespacesAndNewlines to remove whitespace around strings.