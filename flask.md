# Flask

## Flask?

Python 기반 마이크로 웹 프레임워크
* 마이크로 = 작지만 있을 건 다 있다! -> 매우 가볍고 작은 프로젝트에서 효율을 내는 특징을 가지고 있음

## 가상환경 (Virtual Environment)

각 프로젝트의 목적에 따른 모듈만 있는 환경을 구축해서 관리할 수 있도록 함

### 1. 파이썬 가상환경 모듈 설치하기

`pip install virtualenv`

### 2. 현재 디렉토리에 새 가상환경 만들기

`virtualenv <가상환경 이름>`
* 통상적으로는 **venv**로 가상환경 이름을 많이 씀

### 3. 가상환경에 진입하기

Mac
* `source venv/bin/activate`
Window
* `./venv/Scripts/activate.bat`
* `call venv/bin/activate`
* `venv\Scripts\activate`

## Flask 설치하기

`pip install flask`

## Flask 시작하기

`flask run`

# Flask with REST API

## API?

프로그램들이 서로 **상호작용**하는 것을 도와주는 **매개체**

## REST (Representational State Transfer)?

웹 서버가 요청을 응답하는 방법론 중 하나 (*특정한 기술의 이름이 아님*)
* 데이터가 아닌, **자원(Resource)**의 관점으로 접근

## REST API?

**HTTP URI**를 통해 자원을 명시하고 **HTTP Method**를 통해 해당 자원에 대한 CRUD를 진행

### HTTP URI

웹 상에서 자원을 요청할 때, 대상의 식별자 (Identifier)  
* E) URL ( ~ Locate)

### HTTP Method

어떤 자원을 요청하는 방법

|HTTP MEthod|Resource (HTTP URI)|
|:---:|:---:|
|GET|/order|
|POST|/order|
|PUT|/order|
|DELETE|/order|
|* 같은 URI 다른 ACTOIN|

## REST API의 Stateless (무상태성)

Client의 Context를 서버에서 유지하지 않는다
* 각각의 Request를 독립적으로 간주

### REST API의 Stateless Example

1. `POST/shoes`는 자원에 새로운 **정보를 생성**
2. `GET/shoes`는 DB에 shoes가 있는지 확인 후 **해당 자원 반환**

* *(서버 입장에서) 아이템을 GET하기 위해서 POST를 진행할 필요가 없음, POST 여부에 관계없이 GET 실행*

## REST API Example

* jsonify : Python의 dict 타입을 Javascript에서 사용되는 데이터 저장 방식인 json으로 바꿔주는 module

* request : HTTP request를 다룰 수 있는 module

## Postman?

일반적인 웹 브라우저는 POST를 하기에 적절하지 않기 때문에, 별도의 프로그램인 **Postman**을 통해 API를 테스트할 수 있음