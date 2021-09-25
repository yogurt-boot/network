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
   #더 찾아볼게요... <br />
   http는 작은 파일을 여러번 보낼때 유리. <br />
   ftp는 큰 단일 파일을 보낼때 유리.
<br />
   
</details>

### HTTP 응답코드에 대해서 설명하세요

<details>
   <summary> Answer </summary>
<br />
   
</details>

### CORS에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   
</details>


