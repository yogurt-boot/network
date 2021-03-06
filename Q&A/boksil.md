### OSI 7 Layer에 대해서 설명하세요.

<details>
   <summary> Answer </summary>
<br />
   송신호스트에서 수신호스트로 데이터를 전송할 때,
   송신호스트는 수신호스트가 열려있는지 확인하고, 호스트의 ip주소에 도달하기 위한 경로를 찾고, 데이터에 오류가 있는지 확인한 후 이상이 없으면 전기신호로 데이터를 전송한다.
   이 과정에서 전송하려는 데이터 패킷에 헤더가 겹겹이 쌓이고 수신하는 쪽은 역순으로 패킷에 쌓여있는 헤더를 디캡슐레이션 하여 원래의 데이터를 수신받는다. 
   이렇게 네트워크 통신이 일어나는 과정을 7개의 계층으로 나누어 설명한 것을 OSI 7 Layer라고 한다.   
</details>

### DNS에 대해서 설명하세요.

<details>
   <summary> Answer </summary>
<br />
   호출하려는 도메인의 이름을 ip주소로 바꿔주는 시스템
   혹은 ip주소를 도메인 이름으로 바꿔주는 시스템

</details>


### REST 의미에 대해 설명하세요.
   
<details>
   <summary> Answer </summary>
<br />
   
</details>
   

### stateless와 stateful에 대해 설명하세요.  
  
<details>
   <summary> Answer </summary>
<br />
   
</details>


### 클라이언트가 서버에서 발행한 세션을 유지하는 프로세스를 간단하게 설명하세요

<details>
   <summary> Answer </summary>
<br />
   
</details>

### Request Message와 Response Message의 구조차이에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   
</details>

### 파일전송시 ftp와 http의 차이점에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   
</details>

### HTTP 응답코드에 대해서 설명하세요

<details>
   <summary> Answer </summary>
<br />
   클라이언트가 서버로 리퀘스트를 보낼 때 그 결과의 상태에 대한 코드값.
   200번대는 리퀘스트를 정상적으로 수행했음을 의미하고 500번대는 서버에서 리퀘스트 처리에 대해 실패했음을 의미하고
   400번대는 서버가 리퀘스트를 이해할 수 없음을 의미
</details>

### CORS에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   다른 출처에 대한 요청을 허용하도록 HTTP헤더에 내용을 추가하는 것을 의미함
   프로토콜, 포트, 호스트 중 하나라도 다르면 다른 출처로 간주함
</details>

### 웹 캐싱 과정에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   브라우저가 과거에 요청한 적이 있는 리소스를 리퀘스트하는 경우,
   http header에 담겨있는 cache-control 정책에 따라 리소스를 캐시또는 오리진서버에서 받아옴
</details>

### same-origin 과 same-site에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   same-origin은 서브도메인, 도메인, 프로토콜, 포트가 전부 같은 것을 의미하고,
   same-site는 도메인만 같은 것을 의미한다.  
</details>

### XSS에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   스크립트를 심을 수 있는 웹페이지에 해커가 악의적인 스크립트를 삽입하여 공격하는 기법. 
   쿠키정보를 탈취하거나 다른 악의적인 사이트로 리다이렉트 시키는 등의 일을 함.
   쿠키가 탈취된 경우 sessionId를 획득하여 정상적으로 로그인한 유저처럼 행동할 수 있음.
</details>

### https와 http차이에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   
</details>

### 2-factor 인증에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   
</details>

### Web으로 Server Push를 구현하는 방법에 대해 설명하세요.
<details>
   <summary> Answer </summary>
<br />
   WebSocket프로토콜을 이용하여 구현한다. 기존 http프로토콜은 클라이언트에서 서버로 요청하는 단방향 프로토콜이지만,
   webSocket프로토콜은 클라이언트의 요청 없이도 서버에서 요청할 수 있게 지원해주며,
   통신은 tcp포트 80/443을 통해 접속하므로 추가 방화벽 오픈없이 web으로 구현할 수 있다.
</details>

### Socket.io와 WebSocket의 차이에 대해 설명하세요.
<details>
   <summary> Answer </summary>
<br />
   WebSocket은 HTML5 표준 프로토콜이고, Socket.io는 양방향 송신을 가능하게하는 library이다.
   WebSocket프로토콜을 지원하지 않는 오래된 브라우저나 클라이언트가 브라우저가 아닐경우 Socket.io를 이용하여 소켓통신을 구현한다.
</details>

### XSS와 CSRF의 차이에 대해 설명하세요.
<details>
   <summary> Answer </summary>
<br />
   xss는 클라이언트 정보탈취 등 클라이언트에 대한 공격이 목적이고,
   csrf는 인증한 클라이언트에게 서버에 대한 공격을 유도하여 서버를 공격하는 것이 목적이다.
</details>

### 해싱과 암호화의 차이에 대해 설명하세요.
<details>
   <summary> Answer </summary>
<br />
   해싱은 단방향 함수를 사용하고, 암호화는 양방향 함수를 사용한다.
   즉 해싱된값은 원문정보로 복호화 할 수 없으며, 암호화된 값은 원문정보로 복호화할 수 있다.
</details>


