## JWT

* 웹에서 사용되는 JSON 형식의 토큰에 대한 표준 규격. 사용자의 인증또는 인가 정보를 서버와 클라이언트 간에 안전하게 주고 받기 위해서 사용

## 구조

<헤더>.<페이로드>.<서명>

### 헤더

JWT 에서 사용할 타입과 해시 알고리즘의 종류가 있다.

### 페이로드

토큰에서 사용할 정보 Claim 이 있다.

### 서명

사용하는 알고리즘은 헤더에서 정의한 알고리즘 방식이 있다.

---

### Access Token

클라이언트가 갖고있는 실제로 유저의 정보가 담긴 토큰

### Refresh Token

로운 Access Token을 발급해주기 위해 사용하는 토큰, 데이터베이스에 유저 정보와 같이 기록
