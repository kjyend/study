# RequestBody 

http요청의 본문이 그대로 전달된다.xml,json기반의 메시지를 사용할때 유용하다. 
http요청의 내용을 자바객체로 변환하여 매핑된 메소드 파라미터로 전달한다. 

<h2>post요청</h2>

RequestBody로 json데이터가 넘어오면 Jackson2HttpMessageConverter가 변환해주기에
이런 방식으로 ObjectMapper의 readValue 메서드를 사용해서 변환하기에 setter가 필요하지 않다. 
하지만 기본생성자가 있어야한다.

<h2>get요청/h2>

get은 Query Parameter로 받는다. 그래서 WebDataBinder를 사용한다.
WebDataBinder는 자바빈 방식으로 setter가 필요하다.
