# Transaction

데이터베이스의 상태를 변화시키기 해서 수행하는 작업의 단위. 즉 SQL을 사용해서 데이터베이스를 접근하는것을 의미
작업단위는 단순히 한문장이 아니라 많은 문자이라는 점을 알아야한다.

<h2>원자성</h2>
트랜잭션의 연산이 데이터베이스에 모두 반영되거나 반영되지 않아야 한다.
<h2>일관성</h2>
작업이 항상 일관성이 있어야한다. 
<h2>독립성</h2>
하나의 트랜잭션이 다른 트랜잭션의 연산에 끼어들 수 없다.
<h2>지속성</h2>
트랜잭션이 성공되었을 경우, 결과는 영구적으로 반영되어야 한다.

<h2>Conmmit</h2>
트랜잭션 작업이 성공했으며 데이터베이스가 일관된 상태일때, 완료된 것을 트랜잭션 관리자에게 알려주는 연산이다.
<h2>Rollback</h2>
하나의 트랜잭션 처리가 비정상적으로 종료되어 데이터베이스의 일관성이 깨질때, 행한 연산을 취소하는 연산이다.
