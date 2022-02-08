# @Modifying

@Query으로 작성된 수정, 삭제 쿼리 메소드를 사용할때 사용된다. 데이터 변경에 사용되는 INSERT, UPDATE, DELETE쿼리에서 사용된다.
주로 여러건의 연산을 하나로 하는 벌크 연산에 사용된다. @Query에 벌크 연산 쿼리를 작성하고, @Modifying을 붙이면된다.
DB에서는 변경될수 있으나 영속성 컨텍스트에서는 변경이 안될 수 있다. 이때 clearAutomatically를 true로 변경한다면 벌크 연산 후 clear하기에 문제가 해결이 가능하다.
