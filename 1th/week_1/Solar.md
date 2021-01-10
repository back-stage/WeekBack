# 목표

## 목표1
### 스프링 REST API 강의 듣기
* [x] [스프링 기반 REST API 개발](https://www.inflearn.com/course/spring_rest-api/dashboard)

# 회고
스터디 시작 전에 듣고 싶었던 강의여서 수요일부터 급하게 듣기 시작하였는데 TDD로 진행하는 수업이라 만족스럽다. JUnit4를 사용하는게 아쉽지만 이건 나중에 JUnit5로 바꿔야겠다. 
![image](https://user-images.githubusercontent.com/35985636/104125003-67b4c780-5397-11eb-9adf-a644e301ef0a.png)

주초에는 예전에 못들었던 스프링 부트 개념과 활용 강의 뒷부분을 마저 들었다.
이번 스터디에도 시큐리티 적용과제가 있는데 간단한 스프링 시큐리티를 적용해보면 좋을 것 같다.
![image](https://user-images.githubusercontent.com/35985636/104125081-d7c34d80-5397-11eb-99b4-286052064f6d.png)

코쿼 프로젝트를 하면서 이미 알고있던 내용들도 많았지만 내용을 정리하기에 좋았고 스프링에서 어떻게 돌아가는지 얕게라도 알 수 있었다. 다음 프로젝트에서 커스텀하게 사용해볼 수 있지 않을까 싶다.

REST API에 대해서 HTTP method(자원에 대한 행위 표현)와 URL(정보의 자원을 표현해야 한다.) 관점만 생각했었는데, 진짜 Restful 한 API는 
다음 두가지 조건을 만족해야한다는 사실을 배웠다.
* Self-descriptive message
  * 메시지 스스로 메시지에 대한 설명이 가능해야 한다.
  * 서버가 변해서 메시지가 변해도 클라이언트는 그 메시지를 보고 해석이 가능하다.
  * **확장 가능한 커뮤니케이션**
* HATEOAS
  * 하이퍼미디어(링크)를 통해 애플리케이션 상태 변화가 가능해야 한다.
  * **링크 정보를 동적으로 바꿀 수 있다.** 


* [그런 REST API로 괜찮은가](https://www.youtube.com/watch?v=RP_f5dMoHFc)
