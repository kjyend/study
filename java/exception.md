# 예외처리에 대한 공부

예외로 인해 시스템 동작이 멈추는 것을 미리 에측해 제어하는 것을 예외처리라고하다. 


<h2>예외 처리 코드 Try-Catch-Finally/throws</h2>

<h3>Try-Catch-Finally</h3>
dnflrk f

*  Try : 예외가 발생할만한 구문

*  Catch : Exception이 발생하면 실행되는 구문

*  Finally : 반드시 실행되는 구문

Exception 발생 : Try > Catch > Finally
Exception 미발생 : Try > Finally

<h3> throws </h3>
에외 발생 시 예외 처리를 직접하지 않고 호출한 곳으로 넘긴다. 즉 예외가 발생했을 때 내가 직접 처리하지 않고 자동으로 예외를 다시 호출한곳으로 던저서 해결한다.
