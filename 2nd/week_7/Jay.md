# 회고
## 목표1 - 이력서 프로젝트
- 역시나 달성하지 못했지만 의욕을 되찾을 수 있는 한 주였다. 
- 프로젝트에서 가장 마지막으로 하던 작업이 객체 지향적인 코드로 리팩토링하는 것이었는데, 꽤나 골치아팠던 걸로 기억한다. 그 당시와 마찬가지로 많은 고민을 했지만 돌파구를 찾을 수 있었다. 특정 범위 안에서만 변경하려다보니 변경해야 하는 부분이 부담스럽게 많아졌는데, 생각을 넓혀보니 그냥 서비스 자체를 인터페이스로 두고 구현체를 갈아끼우면 훨씬 적은 변경으로 리팩토링을 할 수 있었던 문제였다. 너무 쉽게 해결할 수 있는 문제였고 심지어 한번 해봤던 방법인데 시야가 좁아져서 이렇게나 많은 고민을 했다니...무서운 일이라고 생각했다. 
- 고민했던 부분을 이슈에 남기려고 열심히 정리중이다. 정리하는데 꽤 시간이 오래 걸린다.

<img width="992" alt="스크린샷 2021-04-18 오후 11 45 17" src="https://user-images.githubusercontent.com/33659848/115149676-24f24200-a0a0-11eb-99e3-acd1791cf5da.png">

- 단위 테스트의 FIRST 원칙을 기준으로 나의 테스트 코드를 살펴봤는데, 단위 테스트라고 작성했던 코드들이 대부분 외부 라이브러리(Selenium)에 의존하고 있었다. 그래서 테스트 코드도 완전 리모델링(?)하고 있는 중이다.