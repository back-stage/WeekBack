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





## TIL

* 2021.01.11.Mon
  xib로 viewController를 만든 후 코드로 불러와 화면을 띄울 때 주의할 점
  1. 이 경우 view와 매칭되는 view controller 클래스는 custom class으로 지정하지 않고 file owner로 지정해야 한다.
  2. file owner의 view와 xib 파일의 view를 연결해줘야 한다. ([stackoverflow](https://stackoverflow.com/questions/4763519/loaded-nib-but-the-view-outlet-was-not-set) 참고)

