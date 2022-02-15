# Scope

빈의 범위를 설정하는 어노테이션이다. 보통 스프링이 구동 될때 싱글톤이 생성하는데 이때 @Scope를 통해서 범위를 설정할 수 있다.

<h2>singleton</h2>
스프리 IoC 컨테이너당 하나의 빈만 사용
<h2>prototype</h2>
요청이 있을 때, 새로운 빈을 사용
<h2>request</h2>
HTTP request 라이프 사이클 마다 하나의 빈을 사용
<h2>session</h2>
HTTP session 마다 하나의 빈을 사용
<h2>application</h2>
ServletContext 동안 하나의 빈만 사용
<h2>globalSession</h2>
전체 모든 세션을 하나의 빈으로 사용
