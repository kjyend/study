# Resource 추상화

java.net.URL을 추상화 한 것 이다. 

<h2>java.net.URL</h2>

웹상에 존재하는 자원에 접근할 때 사용하는 클래스다. 웹상의 자원이란 프로토콜, 호스트, 포트번호 등등이다.

<h3>java.net.URL을 추상화하는 이유</h3>

* 기존의 java.net.URL 클래스에서 classpath를 기준으로 resource를 가져오는것이 불가능

* 새로운 핸들러를 등록하여 특별한 URL 접미사를 만들어 사용가능 했지만 구현이 힘들고 편의성 메소드가 부족

<h2>Resource 구현체</h2>

* UrlResource : URL을 기준으로 리소스를 읽는다. 프로토콜 http, https, ftp, file, jar 지원

* CalssPathResource : classpath 기준으로 리소스를 읽는다.

* ServletContextResource : 웹 어플리케이션 루트에서 상대 경로로 리소스를 찾는다.
