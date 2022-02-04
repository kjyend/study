# NoArgsContructor

파라미터가 없는 기본 생성자를 생성합니다. 필드들이 final로 생성되어 있는 경우 에러 발생.
force=true를 사용하면 null,0등 기본 값으로 초기화 하지만
@NonNull같이 제약 조건이 설정되어 있는 경우, 생성자내 null-check로직이 생성 불가
