# RestAPI

### REST

[MDN 정의 ] REST(Representational State Transfer)는 효율적, 안정적이며 확장가능한 분산시스템을 가져올 수 있는소프트웨어 아키텍처 디자인 제약의 모음을 나타냅니다. 그리고 그 제약들을 준수했을 때 그 시스템은 RESTful하다고 일컬어집니다. 

REST 라는 것은 특정한 기술이 아니라 data 아키텍쳐/ design 방법론 임.

정해진 method set을 받아서 동작하며 standard 한 구조적 데이터 (JSON/XML)형태로 output을 반환함.

<br/>

### REST API 가 하는 일

Restapi는 도서관의 사서와 같은 역할을 한다고 생각하면 됨. Application의 client가 어떤 데이터를 어떤 형태로 가져올 것인지 주문하면 Rest API가 요청에 맞춰서 수행함

Database - Rest API - Application




<br/>

### Rest API 가 필요한 이유.

웹사이트 내에서 새로운 page로 이동할 때마다 모든 html,css,js 를 전부 가져오는건 비효율적임.

모든 page가 상태(state) 를 대표(represent)하고 있는 View의 형태로 되어있고. 이 Representational state 가 data object 와 연결되는것임.

즉, web page에 필요한 모든 파일을 새로 가져오는 것이 아니라 데이터만 update 할 수 있음


web의 Single Page Applcation 뿐 아니라 태블릿, 모바일 등 모든 디바이스들이 같은 api resource를 사용함.(consistant)


<br/>

### Restful

RESTful은 일반적으로 REST라는 아키텍처를 구현하는 웹 서비스를 나타내기 위해 사용되는 용어.


#### Reference

 LinkedIn Learning - Learning REST APIs
