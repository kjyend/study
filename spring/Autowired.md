# Autowired

IoC컨테이너 안에 존재하는 Bean을 자동으로 주입하는것이다. 원래라면 xml이나 @Bean을 통해서 설정을 해주어야 했다면 
Autowired를 통해서 객체의 의존성을 가지는 부분에 쉽게 의존성 주입을 받을 수 있다. 

<h2> 해당타입의 빈이 없는 경우</h2>

생성자에 대해서 Autowired가 있는 상태에서 객체에 setter을 해 주고 Autowired를 false로 바꾸어 주어야한다.
왜냐하면 Autowired에 있는 required()때문이다. Default값이 true로 되어있는데 이 경우 해당 의존성은 "꼭 필요한 대상이므로
주입을 반드시 받아야한다"이기에 false로 바꿔 주어야한다.

<h2> 해당타입의 빈이 여러 개인 경우</h2>

* @Primary 

* @Qualifier

* 모든 빈을 주입받기
