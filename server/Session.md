# session

방문자가 웹 서버에 접속해 있는 상태를 세션이라고 한다.

세션을 끝나는 시점은 사용자가 브라우저를 종료하여 서버와의 연결을 끝내는 시점이다.

<h2>특징</h2>

* 각 클라이언트 고유 ID를 부여한다. 
* 서버는 세선 ID로 클라이언트를 구분한다.
* 브라우저를 닫거나, 서버에서 세션을 삭제 했을때만 삭제되므로, 쿠키보다 보안이 좋다.
* 접속 시간에 제한을 두어 일정 시간 응답이 없다면 세션 패기가 가능하다.
* 저장 데이터에 제한이 없다.

<h2>동작 순서</h2>

1. 클라이언트가 페이지를 요청한다.

2. 서버는 접근한 클라이언트의 Request-Header필드인 Cookie를 확인하여, 클라이언트가 해당 session-id를 보냈는지 확인한다.

3. session-id가 존재하지 않는다면, 서버는 session-id를 생성해 클라이언트에게 돌려준다.

4. 서버에서 클라이언트로 돌려준 session-id를 쿠키를 사용해 서버에 저장한다. 쿠키 이름: JSESSIONID

5. 이후 다시 서버에 요청 할때 요청과 쿠키(JSESSIONID)와 함께 session-id 값을 서버에 전달한다.

6. 서버는 전달받은 쿠키에 있는 session-ID를 활용하여 해당 요청을 처리하고 응답
