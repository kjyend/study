# Configuration

Bean등록할것을 가시적으로 표현하는것이다. 또한 Bean을 등록할때 싱글톤을 보장해준다. 
스프링컨테이너에서 Bean을 관리할 수 있게된다. 스프링에서 CGLIB라는 바이트코드 조작 라이브러리를 사용
AppConfig를 상속받는 임의의 클래스를 만들어 빈으로 등록한다.

