- 스프링에서 DB를 연결할 때 스프링에서 드라이버를 요구한다.
- 그 해당 드라이버의 버전을 내 PC에서 다운로드를 받아야 된다.
- 스프링은 JDBC를 사용한다.
- JDBC는 인터페이스다.
- JDBC 인터페이스를 구현체중 하나가  MYSQL Connector다.
- MYSQL Connector자체가 JDBC  드라이버다.
- 그래서 JDBC 드라이버를 다운받아야 된다.
- 그래야만 MYSQL 버전에 맞게 커넥션을 가지고 있다.
- gradle Repository 사이트에 들어가서 다양한 라이브러리를 다운받을 수 있다.
- lib 디렉토리안에 라이브러리가 다 있으니까 라이브러리를 다운받으면 여기에 넣으면 된다.
- mysql은 기본적으로 3306포트 로 되있다.
- 데이터베이스 사용 순서
    1. 맨처음 사용자를 만들어야 된다.
    2. 그 다음 DB를 만들어야 된다.
    3. 그 다음 테이블을 만들어야 된다.
    ```
    <property name="url" value="jdbc:mysql://localhost/springbook?serverTimezone=UTC" />
    ```
/springbook → 이거는 DB이름

.classpath : 라이브러리는 우리가 안만든다. 그거를 가져오려면 뭘 가져와야 되는지를 알아야 되는데 그것이 명시되어 있는 곳이다.