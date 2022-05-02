# 예외

java.lang.Exception 클래스의 서브 클래스들은 Error와 달리 애플리케이션 코드에서 예외가 발생하였을 경우에 사용된다.

<h2>에러</h2>

java.lang.Error 클래스의 서브 클래스들이다. 애플리케이션 코드에서 잡아서는 안되며, 잡아서 대응할 수 있는 방법도 없다.

<h2>체크 예외</h2>

RuntimeException 클래스를 상속하지 않은 Exception 클래스들이다. 예외를 처리하는 코드를 함께 작성해야 한다.

<h2>언체크 예외</h2>

RuntimeException 클래스를 상속한 Exception 클래스들이다. 에러를 처리하지 않아도 컴파일 에러가 발생하지 않는다.

<h2>예외 처리 코드 Try-Catch-Finally/throws</h2>

<h3>Try-Catch-Finally</h3>

*  Try : 예외가 발생할만한 구문

*  Catch : Exception이 발생하면 실행되는 구문

*  Finally : 반드시 실행되는 구문

Exception 발생 : Try > Catch > Finally

Exception 미발생 : Try > Finally

<h3> throws </h3>
에외 발생 시 예외 처리를 직접하지 않고 호출한 곳으로 넘긴다. 즉 예외가 발생했을 때 내가 직접 처리하지 않고 자동으로 예외를 다시 호출한곳으로 던저서 해결한다.
