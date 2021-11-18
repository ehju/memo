# HTTP Protocol

HTTP(HyperText Transfer Protocol)

웹 상에서 정보를 주고 받을 수 있는 프로토콜

API 와  서버의 통신은 주로 HTTP 를 통해 이루어진다.



## HTTP methods

### GET
서버에 리소스를 요청한다. (READ)

### POST
새로운 리소스를 작성한다.(CREATE)

### PUT
리소스 정보를 수정한다.(UPDATE)

### PATCH
리소스 정보의 일부를? 수정한다.(UPDATE)

( POST PUT PATCH 를 구분하지 않는 API도 있다.)

### DELETE
서버에 저장된 리소스를 삭제한다. (DELETE)

### OPTIONS
서버에서 어떤 method 를 지원하는지 알 수 있다.


### HEAD
응답의 HEAD 부분만을 가져온다



##  HTTP status messages

1×× Information
2xx Success
3xx Redirection
4xx Client Error
5xx Server Error

