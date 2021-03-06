# 회고

## 목표1 - 추상화 리팩토링
- 프로젝트를 처음부터 점검하는 시간을 가졌다. 요구 사항에 비해 불필요하게 무거운 기술을 사용하고 있지 않은지, 더 간단한 방법이 존재하는데 익숙하지 않다는 이유(Python?!)로 회피하고 있진 않은지 등등
- 배포할 때 제일 걱정되었던 부분 중 하나가 Selenium을 여러 스레드로 실행시키는 작업이었다. 프로젝트 초반에 스크랩핑 라이브러리의 후보들을 비교하여 Selenium을 선택한 것이지만 혹시 몰라서 다시 한번 비교, 테스트해보았다. 그리고 Selenium보다 더 가벼운 라이브러리를 사용할 수 있다는 사실을 발견했다.
  - [테스트 관련 이슈](https://github.com/beginin15/get-your-friday/issues/40)
  - [관련 내용 TIL](https://github.com/back-stage/WeekBack/pull/130#issuecomment-868647431)
- 애초에 추상화 리팩토링을 진행하는 이유도 스크랩핑 객체가 사용하는 라이브러리가 변경될 가능성을 고려한 것인데 그 상황이 되어버렸다. 추상화가 잘 이루어졌는지 확인할 수 있을 것 같다.
- 원래 이번 주 목표는 추상화 리팩토링이었지만 더 큰(?) 발견을 했고 추상화에 영향을 줄 수 있는 내용이므로 목표 달성으로 체크했다.

## 목표2 - 정렬 알고리즘
- 정렬 알고리즘은 면접을 위해 공부해야겠다는 생각이 들었다.
- 바킹독 강의에서 소개하는 정렬 알고리즘 순서에 맞춰서 이전에 정리한 내용도 함께 복습하면서 공부했다. 그래서 아직 강의를 다 보진 못했다.
- 한눈으로 봤을 때 코드가 매우 간단해도 머리로 완벽히 이해가 되지 않아서 답답했다. 그래도 시간에 구애받지 않고 천천히 직접 코드를 쳐보니까 대충 내용만 훑었을 때보다 만족감이 있다. 효율적인 공부는 아니었지만 의욕이 떨어지는 것보단 낫다는 생각으로 당분간 이 방법으로 진행할 예정이다.
- [정리](https://trello.com/c/hr1HA2qg)