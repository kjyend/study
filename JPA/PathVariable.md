# @PathVariable

URL에서 각 구분자에 들어오는 값을 처리할때 사용한다. 

@GetMapping, @PostMapping, @PutMapping 상관없다. 

ex)
@GetMapping("/user/{number}")

public String findByName(@PathVariable("name") String name){}

ex) http://localhost:8080/aaa/bbb
