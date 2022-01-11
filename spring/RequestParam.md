# RequestParam

컨트롤러에서 Parameter으로 파라미터값을 입력받는 API를 만드는 경우에 사용된다.

<h2>단일 파라미터 변환</h2>

@RequestParam("실제 값") String 설정할 변수 이름으로 표현한다.
ex) /static?name="name에 담긴 value"

RequestParam에 key값이 존재하지 않을 경우 에러가 발생 그런 경우 "required=false"를 해야한다.

<h2>Map</h2>

여러개의 Parameter일 경우에 사용한다. 대규모 파라미터를 받는데 사요하면 편리하지만 다른사람들이 유지보수하기 어려운 점이 있다.
