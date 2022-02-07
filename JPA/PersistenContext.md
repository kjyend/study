# @PersistenContext(영속성 컨텍스트)

EntityManager로 entity를 컨텍스트에 저장하는것을 뜻한다. 

<h2>EntityManager</h2>
트랜잭션 단위를 수행할 때마다 생성한다. 내부 DB커넥션 풀을 이용해서 DB접근. thread간에 공유하면 안된다. 
<h2>EntityManagerFactory</h2>
JPA에서는 애플리케이션 로딩되는 시점에 DB당 하나만 생성해야한다. WAS가 종료되는 시점에 닫는다.
<h2>EntityTransaction</h2>
데이터를 변경하는 모든 작업은 반드시 트랜잭션 안에서 이루어져야 한다.
