### OSI 7 Layer에 대해서 설명하세요.

<details>
   <summary> Answer </summary>
   컴퓨터 간 데이터 송수신이 일어나는 과정을 7단계로 나눈 것을 OSI 7계층이라 한다.
   물리-데이터-네트워크-전송-세션-표현-응용으로 구성되어 있으며 계층 별 역할이 구분되어 있다.
   OSI 7계층을 4단계로 나누어 TCP/IP 프로토콜(데이터링크-네트워크-전송-응용)이라 부른다. 
<br />
</details>

### DNS에 대해서 설명하세요.

<details>
   <summary> Answer </summary>
<br />
IP 주소를 사람이 인지하기 쉬운 형태(영어, 한글 등)로 변환하거나 반대의 역할을 하는 서버를 말한다.
예를 들어 브라우저 url에 www.naver.com을 치면 DNS서버는 입력된 도메인에 해당하는 IP 주소를 반환한다.   

</details>

### REST 의미에 대해 설명하세요.
   
<details>
   <summary> Answer </summary>
   REpresentational State Transfer. 표현적 상태 전달. URI에 자원을 명시하고 HTTP Method를 통해 해당 자원에 대해 어떤 행위를 할 것인지 나타낸다.
<br />
   
</details>
   

### stateless와 stateful에 대해 설명하세요.  
  
<details>
   <summary> Answer </summary>
   #더 찾아볼게요... <br />
   stateless : 무상태. 서버가 클라이언트의 상태를 유지하지 않음. http 프로토콜은 stateless <br />
   stateful : 상태 유지. 서버 부하가 크다?
<br />
   
</details>


### 클라이언트가 서버에서 발행한 세션을 유지하는 프로세스를 간단하게 설명하세요

<details>
   <summary> Answer </summary>
   서버에서 세션id를 Set-cookie 헤더에 넣어 response로 보내면 클라이언트에서는 해당 쿠키값을 기억하고, 이후 request를 보낼 때 자동으로 헤더 쿠키에 값을 넣어서 보낸다.
<br />
   
</details>

### Request Message와 Response Message의 구조차이에 대해 설명하세요

<details>
   <summary> Answer </summary>
   Request Message : HTTP Method, 헤더, query string 이나 body <br />
   Response Message : HTTP status, message, body, 헤더(쿠키 등)
<br />
   
</details>

### 파일전송시 ftp와 http의 차이점에 대해 설명하세요

<details>
   <summary> Answer </summary>
   http는 작은 파일을 여러번 보낼때 유리. <br />
   ftp는 큰 단일 파일을 보낼때 유리.
<br />
   
</details>

### HTTP 응답코드에 대해서 설명하세요

<details>
   <summary> Answer </summary>
   http 응답코드는 클라이언트가 보낸 요청에 대한 응답 상태를 숫자 + 메세지로 표현한 것이다. 상태 종류에 따라 1xx, 2xx, 3xx, 4xx, 5xx로 표현된다.
   가장 유명하고 쉽게 볼 수 있는 코드는 404 Not Found 가 있다.
<br />
   
</details>

### CORS에 대해 설명하세요

<details>
   <summary> Answer </summary>
   교차 출저 리소스 공유 Cross Origin Resource Sharing 의 약자로 서로 다른 Origin 간에 리소스 요청 및 응답이 가능한 정책을 말한다.
   브라우저는 보안상 기본적으로 SOP 정책을 따르기 때문에 동일한 Origin 내에서만 리소스의 요청 및 응답이 가능하다. 
   다만 응답 헤더에 Access-Control-Allow-Origin과 요청 쪽 Origin이 포함되어 있다면 CORS가 가능하다. 
   헤더 값은 서버에서 설정하거나, 프록시 서버를 통해 설정 할 수 있다. 
<br />
   
</details>

### 웹 캐싱 과정에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   
</details>

### same-origin 과 same-site에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   
</details>

### XSS에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   
</details>


### https와 http차이에 대해 설명하세요

<details>
   <summary> Answer </summary>
   http 통신은 평문의 메세지를 주고받아 통신이 도청되면 바로 안에 내용을 알 수 있다. 
   또한 리퀘스트에 대한 진위 확인을 하지 않기 때문에 변조된 요청 및 응답인 지 알 수 없다.
   이러한 http 프로토콜에 보안 요소를 강화한 것이 https(secure)이다. https는 공개키-비밀키를 통한 암호화 및 인증서를 통해 통신을 보호한다. 
<br />
   
</details>

### 2-factor 인증에 대해 설명하세요

<details>
   <summary> Answer </summary>
   이중 인증 혹인 2단계 인증이라고도 말하며 말 그대로 2개의 다른 방법을 사용해 인증하는 것이다. 
   예를 들어 로그인의 경우, 아이디-비밀번호를 입력한 후 otp 코드를 한번 더 입력하거나 설정한 메일주소를 입력하는 방법 등이 있다. 
<br />
   
</details>

### Web으로 Server Push를 구현하는 방법에 대해 설명하세요.
<details>
   <summary> Answer </summary>
   완전한 서버푸시는 아니지만 그렇게 보이는 방법(클라이언트에서 리퀘스트 필요) - ajax polling, ajax long polling, comet <br/>
   리퀘스트 없이 서버 푸시 가능 - SPDY(http2), WebSocket <br/>
   https://stackoverflow.com/questions/11077857/what-are-long-polling-websockets-server-sent-events-sse-and-comet
  
<br />
   
</details>

### Socket.io와 WebSocket의 차이에 대해 설명하세요.
<details>
   <summary> Answer </summary>
   WebSocket은 프로토콜이며 웹소켓을 사용하기 위해서는 서버와 클라이언트가 웹소켓을 지원해야 한다. 요즘은 대부분의 브라우저가 웹소켓을 지원하지만 버전이 다를 수 있다.
   여러 서버 구현체(Jetty, GlassFish, Node.js, Netty, Grizzly 등)가 웹소켓을 지원한다. <br/>
   반면 Socket.io는 라이브러리로 브라우저 종류에 상관없이 양방향 통신이 가능하다. Socket.io를 사용하면 WebSocket을 지원하지 않은 클라이이언트의 경우 http통신으로 대체한다. <br />
   ('The client will try to establish a WebSocket connection if possible, and will fall back on HTTP long polling if not.')
   https://d2.naver.com/helloworld/1336 <br/>
   https://socket.io/docs/v4/   
<br />
   
</details>

### XSS와 CSRF의 차이에 대해 설명하세요.
<details>
   <summary> Answer </summary>
<br />
</details>

### 해싱과 암호화의 차이에 대해 설명하세요.
<details>
   <summary> Answer </summary>
<br />
</details>
