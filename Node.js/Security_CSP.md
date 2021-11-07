# CSP(Content Security Policy): 콘텐츠 보안 정책

ckeditor 가 언제부턴가 제대로 동작하지 않고 있었음.

개발자도구로 확인해 봤을 때 CSP(차단됨) 이라고 나옴.

  
<br/>
  

### CSP(Content Security Policy): 콘텐츠 보안 정책

외부에서 페이지를 공격하는 것을 막기 위해, 자기자신이 아닌 다른 출처의 script을 아예 막아버리는것.


![image](https://user-images.githubusercontent.com/13077196/140635585-edf9626f-b71c-48b5-b20d-22e75c5af996.png)
Node.js helmet의 default 옵션을 사용하면  self 이외는 다 막아버림 ( 출처 : https://www.npmjs.com/package/helmet )



### 해결방법

helmet의 csp옵션을 변경해줌

``` javascript

let cspOptions = {
    useDefaults: true,
    directives: {
      "script-src": ["'self'", 'https://cdn.ckeditor.com/ckeditor5/30.0.0/classic/ckeditor.js', "'unsafe-inline'"]
    },
  }

```

"unsafe-inline"은 사실 위험해서 hash나 nonce를 사용해야 한다고 함

그런데 무슨 일인지 hash 로 하려고 했는데 잘 안먹어서 일단 이대로 반염.. ( 추후 보강 필요 )


<br/>
참고 사이트 : https://developer.mozilla.org/ko/docs/Glossary/CSP﻿
