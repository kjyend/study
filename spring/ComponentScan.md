# ComponentScan

ComponentScan은 Component 및 streotype이 부여된 Class들을 자동으로 Scan하여 Bean으로 등록하는 역할이다.
이전 xml파일을 이용하여 지정했던것을 java파일을 이용하여 bean을 scan하기 위해 생겼다.
<h2>ComponentScan의 범위</h2>

* basePackges -직접 패키지 경로에 위치를 입력한다. ex)com.study.spring

* basePackgeClasses -class를 입력한다. class가 위치한 곳에서부터 모든 어노테이션이 부여된 class를 빈으로 등록한다. ex)springstudy.class

<h2>Configuration</h2>

스프링 IoC 컨테이너에게 해당 클래스가 Bean 설정 파일이라는 것을 알려주는 역할이다.
