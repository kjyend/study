# maven

maven은 자바 프로젝트의 빌드를 자동화 해주는 빌드 툴이다. maven은 필요한 라이브러리를 특정 문서(pom.xml)에 정의하면 네트워크에서 자동으로 다운받아 준다.

<h2>LifeCycle</h2>

maven은 미리 정의하고 있는 빌드 순서가 있어서 빌드에 따라 동작한다. 이를 Lifecycle이라 한다.

* Default(Build) : 일반적인 빌드를 위한 프로세스를 위한 모델

* Clean : 빌드시 생성되었던 파일들을 삭제

* Validate : 프로젝트가 올바른지 확인하고 필요한 모든 정보를 사용할 수 있는지 확인

* Complie : 프로젝트의 소스코드를 컴파일

* Package : 실제 컴파일된 소스 코드와 리소스들을 배포를 위한 패키지로 만듬

* Verify : 통합ㅍ 테스트 결과에 대한 검사를 실행하여 품질 기준을 충족하는지 확인

* Install : 패키지를 로컬 저장소에 설치

* Site : 프로젝트 문서와 사이트 작성, 생성

* Deploy : 만들어진 package를 원격 저장소에 release

1. compile : src/main/java 아래 모든 소스 코드 컴파일

2. test : src/test/java, src/test/resources 테스트 자원 복사 및 테스트 소스 코드 컴파일

3. packaging : target디렉토리 하위에 jar,war등 컴파일과 테스트가 완료 된 후, 압축

<h2>settings.xml</h2>

maven tool 과 관련한 설정 파일이다. MAVEN_HOME/conf에 위치한다. 

<h2>pom.xml</h2>

pom(project object model)을 설정하는 부분으로 프로젝트 내 빌드 옵션을 설정하는 부분이다. 다른이름으로 저장할 수 있다. 하지만 pom.xml을 쓰기를 권장한다.

* modelVersion : maven의 모델 버전이다.

* groupId : 프로젝트를 생성한 조직의 고유 아이디이다. 일반적으로 url의 역순으로 한다.

* artifactId: 프로젝트에서 생성하는 파일이름이다.

* version : 프로젝트의 현제 버전이다. 접미사로 SNAPSHOT을 붙이면 개발단계이다.

* packaging : 패키지 유형(jar,war,ear등)이다.

* name : 프로젝트 이름

* description : 프로젝트에 대한 설명

* url : 프로젝트를 찾을 수 있는 URL

* properties : pom.xml에서 중복해서 사용되는 설정 값을 지정해놓는 부분이다. ex)${java.}

* profiles : 나누어야할 필요가 있는 설정 값은 profiles로 설정한다.

* build : 빌드에 사용할 플러그인 목록

<h2>build에서 설정할 수 있는 값</h2>

* fianlName : 빌드 결과물 이름을 설정

* resources : 리소스(각종 설정 파일)의 위치를 지정. 기본으로 src/main/resources

* testresources : 테스트 리소스의 위치를 지정. 기본으로 src/text/resources

* reprositories : 빌드할 때 접근할 저장소의 위치를 지정. 기본으로 http://repo1.maven.org/maven2

* outputDirectory : 컴파일한 결과물 위치 설정. 기본으로 target/classes

* testoutputDirectory : 테스트 소스를 컴파일한 결과물 위치 설정 기본으로 target/test-classes


