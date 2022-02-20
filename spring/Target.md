# @Target

적용할 위치를 나타내는데 사용된다. ElementType은 해당 타입선언 사용한다는 의미이다.

<h2>Retention</h2>

실제로 적용되고 유지되는 범위를 의미.

* RetentionPolicy.RUNTIME은 JVM에 의해서 계속 참조가 가능

* RetentionPolicy.CLASS은 컴파일러가 클래스를 참조할 때까지 유효

* RetentionPolicy.SOURCE은 컴파일 전까지만 유효
