# Bean scope

Bean Scope는 Bean이 1개만생성하거나 여러개를 생성하는가 결정한다.

<h2>Singleton</h2>

Container 내에 동작하는 단 하나의 객체만 생성하여 만들어진다. spring에서 별도의 설정을 하지 않을 경우 bean scope는 singleton으로 구성된다.

<h2>prototype</h2>

Bean을 IoC컨테이너로 부터 받아올 때마다 매번 새로운 객체가 생성된다. 주의할 점은 같은 곳에있는 객체를 호출하면 
객체가 새로 생겨나는것이 아니라는것이다. 

<h2>주의사항</h2>

Prototype scope 사용시 singleton scope안에 주입되는 Prototype scope를 주의해야한다. 이를 인지하지 않으면 bean생성을 할때 
새로운 객체가 아닌 같은 객체가 나오게된다. 이는 IoC 컨테이너가 Bean을 주입할때 singleton의 필드에 존재하는 Prototype에 또 주입하는 상태가 될수 있기때문이다.
이경우 singleton 안에 있는 prototype는 새로운 bean이 생성하지 않는다.

<h2>Proxymode</h2>

위처럼 singleton scope안에 Prototype scope가 있는경우 해결방안으로 Proxymode가 있다. 
이렇게 되면 Prototype의 객체를 새로운 객체가 출력가능한 proxy가 감싸는 식이된다.  
