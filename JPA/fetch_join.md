# fetch join

SQL의 조인 종류가 아닌 JPQL에서 성능 최적화를 위해 제공하는 기능. entity를 한번에 가져오는데 목적이있기에 지연로딩(LAZY)이 아닌 즉시로딩(EAGER) 전략을 사용한다.
n+1문제의 해결방안 중 하나이다. 

<h2>distinct</h2>

단순하게 fetch join하면 중복되는 row가 있다. 그 중복되는 row를 제거할수 있는게 distinct이다.
