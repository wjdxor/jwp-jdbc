# JDBC 라이브러리 구현
## 진행 방법
* 프레임워크 구현에 대한 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)

### 구현 할 기능 리스트
* step1
  * HTML 대신 JSON으로 데이터를 요청하고 응답 받도록 변경한다.
    * core.mvc.JsonViewTest의 모든 테스트를 pass하도록 JsonView를 구현.
    * next.controller.UserAcceptanceTest 테스트를 pass하도록 Controller 추가.
* step2
  * UserDao의 update, findAll을 구현한다.
  * UserDaoTest를 통하여 구현을 확인한다.
  * 리팩토링을 통하여 소스의 가독성을 높인다.
  * 공통 라이브러리를 만들어 SQL쿼리, 인자, 데이터 추출에 집중 할 수 있게 한다.
