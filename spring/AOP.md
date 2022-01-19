# AOP

관점 지향 프로그래밍이라고 한다. Aspect로 모듈화시키고 사용하는것이다.

* Aspect : Aspect 안에 모듈화 시킨 것

* Advice : 실질적으로 어떤 일을 해야하는것

* Pointcut : 어디에 적용해야 하는지에 대한 정보

* Target : Aspect에 적용 되는 대상 

* Join point : Advice가 적용될 위치, 끼어들 수 있는 지점 등 다양한 시점에 적용가능하다.

<h2>AOP 특징</h2>

* 스프링 빈에만 AOP를 적용 가능

* 스프링 IoC와 연동하여 엔터프라이즈 애플리케이션들에서 문제에 대한 해결책을 지원하는 목적

<h2>Aspect의 실행 시점 지정 어노테이션</h2>

* @Before : 타겟 메소드가 호출되기전 어드바이스 기능 수행

* @After : 타겟 메소드의 결과 관계 없이 타겟 메소드가 완료되면 기능 수행

* @AfterReturning : 타겟 메소드가 결과값을 성공하여 반환 후 기능 수행

* @AfterThrowing : 타겟 메소드가 수행 중 예외를 던지면 기능 수행

* @Around : 타겟 메소드 호출전과 후에 기능 수행