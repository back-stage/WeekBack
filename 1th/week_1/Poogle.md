# 목표

## 목표1 - Photo Tag 프로젝트 마무리
- [x] 전체 API 구현 및 배포
- [x] 코드 리팩토링
- [x] 코드 리뷰 신청
- [x] 문서화 작업: README 정리, 로그 시트 업데이트, 블로그 글 정리 및 업로드

# 회고
## Photo Tag 프로젝트 마무리
### 프로젝트 시작 - 마음가짐, 소개
* [개발 기록](https://suhyunsim.github.io/2020-10-12/photo-tag-project)

### 얻고자 했던 것
- [x] 전부 내 손으로 직접 구현, iOS와 원할한 소통
![Screenshot from 2021-01-10 20-15-41](https://user-images.githubusercontent.com/58318786/104121344-aab77080-5380-11eb-80a1-446b796dfd2d.png)

- [x] 코드스쿼드 과정 중 놓친 부분들을 최대한 적용
    * RDS
    * S3
    * 자동배포
    * 무중단 배포
    * open API 활용

- [x] 문서화
    * [README](https://github.com/SimLeeTag/photo-tag-backend)
    * [API sheet](https://docs.google.com/spreadsheets/d/1gHO1JHXxuU0hV4mtMjsBqaDUbOPT61zda3QIDIxAJZc/edit?usp=sharing)
    * [로그 시트](https://docs.google.com/spreadsheets/d/1ZVOKlSRF1K4oozG9hMWMO3tkUF_r6mvOVHHwoGeZuBU/edit?usp=sharing)
    * 블로그 포스팅

- [x] commit 영문 작성
![Screenshot from 2021-01-10 20-23-04](https://user-images.githubusercontent.com/58318786/104121458-b8b9c100-5381-11eb-849f-33efb62100c3.png)

### 구현 상황
![Screenshot from 2021-01-10 20-25-36](https://user-images.githubusercontent.com/58318786/104121500-151ce080-5382-11eb-96e7-387566e5331b.png)
![Screenshot from 2021-01-10 20-25-51](https://user-images.githubusercontent.com/58318786/104121501-164e0d80-5382-11eb-8602-8d0053e05c93.png)

* 노트, 태그 기본적인 CRUD 기능 api 전체 구현 후 배포
* Apple OAuth Login 
* Travis CI, Code Deploy를 활용한 자동 배포

### 추가 반영, 구현 사항
* Team Repository 문서화 작업
* 기술 문서 BE Repo wiki 업로드
* Trouble Shooting 블로그 포스팅
* 관리자 기능 - 웹 구현 예정 (~ 1월 중)
    * 전체 유저 목록
    * 유저 관리 (수정, 삭제)
* 장소, 날짜 기능 - Criteria, Query DSL 공부 후
    * Google Map 지원
    * 필터링
    * 정렬
    * 검색
* Elastic Search
* 소셜 로그인 - Google, Facebook OAuth
* 공유 기능
    * 링크 생성
    * 접근 권한 관리
* 사진 편집
    * 이미지 위 그리기

### 소감
* 생각보다 오랜 기간 작업하게 되어서 마무리가 더뎠다. 약 한 달 간의 42서울 과정이 끝난 후에 다시 코드에 익숙해지는데 꽤 시간이 걸렸고, 또 집에서 원격으로 진행하다보니 소통의 어려움이나 집중의 한계도 존재했다.
* 그럼에도 불구하고 한 프로젝트를 마무리 지었다는 것에 의의를 둔다. 처음에 의논했던 모든 api를 구현했고, 목표로 했던 내용들을 대부분 적용할 수 있었다. 프로젝트의 마감 기한이 특별히 없다 보니 추가적으로 기획하고 싶은 내용들이 자꾸만 생겼는데 그만큼 다양한 기능들을 고려해볼 수 있어서 재밌었다.
* 다만 아쉬운 것은 코드스쿼드 과정 중 진행했던 내용들의 대부분을 복습하는 느낌의 프로젝트라 특별히 새로운 기술에 대해 공부하지 않았다는 점이다. 또한 TDD로 구현하지 않은 것도 아쉽다. 아직 테스트 코드를 작성하는 것에 익숙해지지 않아 이번 프로젝트에는 적용하지 못했는데 추후 프로그래머스 스터디나 TDD 강의를 수강하고 추가적으로 작성해보고 싶다.