### OSI 7 Layer에 대해서 설명하세요.

<details>
   <summary> Answer </summary>
<br />
   컴퓨터 네트워크 프로토콜을 기능에 따라 계층별로 나눈 것으로 물리 계층, 데이터 링크 계층, 네트워크 계층, 전송 계층, 세션 계층, 표현 계층, 응용 계층으로 이루어진다.
   계층을 나눔으로써 네트워크가 일어나는 과정들을 명확하게 알아볼 수 있고, 각 계층의 내부를 자유롭게 설계할 수 있다.
   네트워크 통신 과정에서 응용 계층부터 차례로 헤더가 붙으며 캡슐화되고 반대로 물리 계층부터 차례로 사용한 헤더를 떼어내며 역캡슐화한다.
</details>

### DNS에 대해서 설명하세요.

<details>
   <summary> Answer </summary>
<br />
   도메인 네임과 IP 주소를 서로 변환해주는 시스템이다.
   Local DNS Server와 Root DNS Server, TLD Server 등을 거치며 변환된다.
</details>

### REST 의미에 대해 설명하세요.
   
<details>
   <summary> Answer </summary>
<br />
   심플한 인터페이스를 설계하기 위한 아키텍처이다. HTTP와 잘 어울리고, 유연성이 높은 방식이다. 그래서 특히 MSA에서는 대부분 REST API를 도입한다.
   Uniform Interface, Stateless, Cacheable, Self-descriptiveness, Layered System, Server-Client 구조 등을 특징으로 꼽을 수 있다.
   HTTP 상의 REST API는 URI로 자원을 나타내고, Method로 자원에 대한 행위를 표현한다.
</details>
   

### stateless와 stateful에 대해 설명하세요.  
  
<details>
   <summary> Answer </summary>
<br />
   상태와 관계 없이 같은 요청에 대해 같은 응답을 유지하면 stateless한 것이고, 상태에 따라 다른 동작을 하면 stateful한 것이다.
   응답하는 쪽(Server)에서 요청하는 쪽(Client)의 정보를 가지고 있으면 stateful하다고 한다.
   HTTP의 경우, 기본적으로 stateless한 프로토콜로 각 요청은 서로 분리된 트랜잭션을 가진다. 
   그래서 사용자 인증 정보 등 유지 되어야하는 정보가 있을 경우, 쿠키와 세션 등을 사용하여 stateful하게 동작할 수 있다.
</details>


### 클라이언트가 서버에서 발행한 세션을 유지하는 프로세스를 간단하게 설명하세요

<details>
   <summary> Answer </summary>
<br />
   클라이언트가 session id 없이 요청을 한 경우, 서버는 새로 session id를 발급하여 세션 정보들을 서버에 저장해두고 response에는 session id를 담아 응답한다.
   이 때, Set-cookie 헤더를 이용해 클라이언트에서 session id를 저장해놓을 수 있도록 한다.
   클라이언트는 이후 요청을 보낼 때 헤더에 session id 값을 담아 보내면, 서버에서는 session id에 해당하는 정보들을 활용할 수 있게 된다.
</details>

### HTTP의 Request Message와 Response Message의 구조차이에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   헤더와 바디로 나누어져 있는 것은 같고, 메시지 헤더가 리퀘스트 라인이나 상태 라인을 포함한다는 점이 서로 다르다.
   Request는 HTTP 버전과 메소드, URI를 담은 리퀘스트 라인을 포함하고 있다.
   Response는 HTTP 버전과 결과를 나타내는 상태 코드, 설명을 담은 상태 라인을 포함하고 있다.
</details>

### 파일전송시 ftp와 http의 차이점에 대해 설명하세요

<details>
   <summary> Answer </summary>
<br />
   FTP는 양방향 프로토콜로 한번 커넥션을 맺고 파일업/다운로드를 여러번 수행하고 커넥션을 해제할 수 있다.
   HTTP는 단방향 프로토콜로 한번의 커넥션으로 하나의 요청->응답을 통해 파일업/다운로드를 수행한다.
</details>




