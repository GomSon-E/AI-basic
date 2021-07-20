# 인터넷과 웹

## 인터넷 (Internet)

전 세계 컴퓨터를 하나로 합치는 거대한 통신**망**

## 웹 (Web)

인터넷에 연결된 사용자들이 정보를 공유할 수 있는 **공간**

### 웹사이트 (Web Site)

웹페이지의 집합
* E) Naver

### 웹페이지 (Web Page)

웹에 존재하는 개별의 정보
* E) Naver.shopping,
     Naver.sports,
     Naver.entertainment,
     ...

## Web의 동작방식

웹은 **클라이언트**와 **서버** 사이의 소통이다

* 클라이언트 (Client) : 정보를 요청함
* 서버 (Server) : 정보를 제공함

1. Client가 Server에 정보를 **요청** : Request
    * E) naver.com/blog : naver.com의 blog 정보를 요청
      E) naver.com/ : naver.com의 root 정보 (홈페이지)를 요청
2. Server는 이 요청받은 정보에 대한 **처리**를 진행
    * 데이터베이스로부터 정보를 가지고 오거나 렌더링을 통해 문서를 준비해야 하는 경우도 있음
3. Server가 Client에게 요청에 대해 **응답** : Response
    * E) 200 ok, 403, 500 ...

### HTTP

웹 사용자끼리의 약속

* HTTP Request : HTTP Verb
* HTTP Response : HTML ...