### OSI 7 Layer에 대해서 설명하세요.

<details>
   <summary> Answer </summary>
<br />
   컴퓨터 네트워크 프로토콜을 기능에 따라 계층별로 나눈 것으로 물리 계층, 데이터 링크 계층, 네트워크 계층, 전송 계층, 세션 계층, 표현 계층, 응용 계층으로 이루어진다.<br />
   계층을 나눔으로써 네트워크가 일어나는 과정들을 명확하게 알아볼 수 있고, 각 계층의 내부를 자유롭게 설계할 수 있다.<br />
   네트워크 통신 과정에서 응용 계층부터 차례로 헤더가 붙으며 캡슐화되고 반대로 물리 계층부터 차례로 사용한 헤더를 떼어내며 역캡슐화한다.<br />
</details>

### DNS에 대해서 설명하세요.

<details>
   <summary> Answer </summary>
<br />
   도메인 네임과 IP 주소를 서로 변환해주는 시스템이다.<br />
   Local DNS Server와 Root DNS Server, TLD Server 등을 거치며 변환된다.<br />
</details>

### REST 의미에 대해 설명하세요.
   
<details>
   <summary> Answer </summary>
<br />
   심플한 인터페이스를 설계하기 위한 아키텍처이다. HTTP와 잘 어울리고, 유연성이 높은 방식이다. 그래서 특히 MSA에서는 대부분 REST API를 도입한다.<br />
   Uniform Interface, Stateless, Cacheable, Self-descriptiveness, Layered System, Server-Client 구조 등을 특징으로 꼽을 수 있다.<br />
   HTTP 상의 REST API는 URI로 자원을 나타내고, Method로 자원에 대한 행위를 표현한다.<br />
</details>
   

### stateless와 stateful에 대해 설명하세요.  
  
<details>
   <summary> Answer </summary>
<br />
   상태와 관계 없이 같은 요청에 대해 같은 응답을 유지하면 stateless한 것이고, 상태에 따라 다른 동작을 하면 stateful한 것이다.<br />
   응답하는 쪽(Server)에서 요청하는 쪽(Client)의 정보를 가지고 있으면 stateful하다고 한다.<br />
   HTTP의 경우, 기본적으로 stateless한 프로토콜로 각 요청은 서로 분리된 트랜잭션을 가진다. <br />
   그래서 사용자 인증 정보 등 유지 되어야하는 정보가 있을 경우, 쿠키와 세션 등을 사용하여 stateful하게 동작할 수 있다.<br />
</details>


### 클라이언트가 서버에서 발행한 세션을 유지하는 프로세스를 간단하게 설명하세요

<details>
   <summary> Answer </summary>
<br />
   클라이언트가 session id 없이 요청을 한 경우, 서버는 새로 session id를 발급하여 세션 정보들을 서버에 저장해두고 response에는 session id를 담아 응답한다.<br />
   이 때, Set-cookie 헤더를 이용해 클라이언트에서 session id를 저장해놓을 수 있도록 한다.<br />
   클라이언트는 이후 요청을 보낼 때 헤더에 session id 값을 담아 보내면, 서버에서는 session id에 해당하는 정보들을 활용할 수 있게 된다.<br />
</details>

### HTTP의 Request Message와 Response Message의 구조차이에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   헤더와 바디로 나누어져 있는 것은 같고, 메시지 헤더가 리퀘스트 라인이나 상태 라인을 포함한다는 점이 서로 다르다.<br />
   Request는 HTTP 버전과 메소드, URI를 담은 리퀘스트 라인을 포함하고 있다.<br />
   Response는 HTTP 버전과 결과를 나타내는 상태 코드, 설명을 담은 상태 라인을 포함하고 있다.<br />
</details>

### 파일전송시 ftp와 http의 차이점에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   FTP는 양방향 프로토콜로 한번 커넥션을 맺고 파일업/다운로드를 여러번 수행하고 커넥션을 해제할 수 있다.<br />
   HTTP는 단방향 프로토콜로 한번의 커넥션으로 하나의 요청->응답을 통해 파일업/다운로드를 수행한다.<br />
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

### 웹 캐싱 과정에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   웹 애플리케이션 서버 앞단에 캐싱 프록시 서버를 추가하여 새로운 리퀘스트가 들어왔을 때 캐시 서버에서 실제 서버의 응답을 캐싱해두고
다음 번에 같은 리퀘스트가 들어온 경우 웹 애플리케이션 서버에 요청을 보내지 않고 직접 캐시된 응답을 반환한다. 
</details>

### same-origin 과 same-site에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   same-origin : scheme, host, port가 모두 같음
   same-site : 서브도메인을 제외하고 TLD와 그 다음 도메인만 같으면 same-site. (example.com)

   same-site는 쿠키 설정 시 공유 기준이 된다. 
</details>

### XSS에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   사용자 입력 값에 스크립트를 넣어 해당 스크립트를 실행시키는 공격이다. 
   저장되는 입력 값에 스크립트를 삽입해 지속적으로 공격하는 방식을 Stored XSS라고 하며
   일회성으로 요청 파라미터에 스크립트를 삽입하는 방식을 Reflected XSS라고 한다. 
   Reflected XSS는 보통 브라우저에 차단 처리가 되어있다. 
   사용자 정보 탈취나 브라우저에서 악성 스크립트가 실행되도록 하는 방식이기 때문에 공격대상은 서버보다는 클라이언트가 된다. 
   CSRF는 사용자가 인증되어있는 상태를 이용해서 서버를 대상으로 공격하는 방식이다. 
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
