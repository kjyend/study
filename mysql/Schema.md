# 스키마

데이터베이스의 구조와 제약 조건에 관한 전반적인 명세를 기술한 것이다.

자세히 말하면, 
객체의 특성을 나타내는 속성(Attribute)과, 속성들의 집합으로 이루어진 개체(Entity), 
개체 사이에 존재하는 관계(Relation)에 대한 정의와 이들이 유지해야 할 제약 조건을 기술한 것입니다.

<h2>특징</h2>

1. 데이터 사전에 저장되며, 다른 이름으로 메타데이터라고도 한다.
2. 현실 세계의 특정한 한 부분의 표현으로서 특정 데이터 모델을 이용해서 만들어진다.
3. 시간에 따라 불변인 특성을 갖는다.
4. 데이터의 구조적 특성을 의미하며, 인스턴스에 의해 규정된다.

<h2>스키마의 3계층</h2>
<h3>외부 스키마</h3>

1. 사용자들의 입장에서 필요로 하는 데이터베이스의 논리적 구조를 정의한 것이다.
2. 하나의 데이터베이스 시스템에는 여러개의 외부 스키마가 존재할 수 있으며 하나의 외부 스키마를 여러개의 응용 프로그램이나 사용자가 공용할 수도 있다.
3. 같은 데이터베이스에 대해서도 서로 다른 관점을 정의할 수 있도록 허용한다.
4. 일반 사용자는 SQL을 이용하여 DB를 쉽게 사용할 수 있다.

<h3>개념 스키마</h3>

1. 데이터베이스의 전체 조직에 대한 논리적인 구조로, 물리적인 구현은 고려하지 않는다.
2. 각 데이터베이스에는 한 개의 개념 스키마만 존재한다.
3. 개체 간의 관계 및 무결성 제약 조건에 대한 명세를 정의한다.
4. 데이터베이스 파일에 저장되는 데이터의 형태를 나타낸다.

<h3>내부 스키마</h3>

1. 물리적 저장장치의 입장에서 본 데이터베이스 구조로, 물리적인 저장장치와 밀접한 계층이다.
2. 개념 스키마를 디스크 기억장치에 물리적으로 구현하기 위한 방법을 기술한 것이다.
3. 저장 데이터 항목의 표현 방법, 내부 레코드의 물리적 순서 등을 나타낸다.

