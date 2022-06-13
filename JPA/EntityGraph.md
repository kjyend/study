# EntityGraph

entity의 특정한 속성을 같이 Loding 하도록 표시하는 어노테이션

<h2>특징</h2>

* attributePaths: Loding 설정을 변경하고 싶은 속성의 이름을 배열로 명시한다.

* type: @EntityGraph를 어떤 방식으로 적용할 것인지 설정한다.

* FATCH 속성값은 attributePaths에 명시한 속성은 EAGER로 처리하고 나머지는 LAZY로 처리.
