# HTTP & HTTPS

## HTTP란 무엇일까?

#### HTTP
- HyperText Transfer Protocol
- 인터넷에서 클라이언트와 서버가 자원을 주고받을 때 이용하는 통신 규약이다.
- TCP/IP위에서 동작한다.
- 텍스트, 이미지, 영상, JSON 등 거의 모든 형태의 데이터를 전송할 수 있다.

##### HTTP는 보안적으로 안전한가?
- HTTP는 암호화가 되지않은 평문 데이터를 전송하는 프로토콜이다.
- 통신에 대한 별다른 보안 조치가 없다.
	- 즉, 만약 누군가 네트워크 신호를 가로챈다면, HTTP의 내용은 그대로 노출된다.

=> 그럼 어떻게 해야 할까?
=> HTTPS의 등장!

```
HTTP일때,
📱비밀번호:1234 -> HTTP -> 💻비밀번호:1234
```

## HTTPS란 무엇일까?

#### HTTPS
- HyperText Transfer Protocol Secure
- HTTP의 보안 취약점을 개선하기 위해, SSL과 TLS을 활용한다.
	- SSL 인증서: 데이터 암호화를 통해, 도난 및 해킹을 방지한다.
	- TLS: 데이터 무결성을 제공하기 때문에, 데이터 전송 중 수정 및 손상을 방지한다.
- SEO에서도 유리하다.
<br/>

##### HTTPS가 보안이슈를 해결하는 방법
- 기존의 HTTP 프로토콜은, 전송계층의 TCP 위에서 동작한다.
- HTTPS는, 여기서 SSL이라는 보안계층이 전송계층 위에 올라간다.
> 즉, SSL위에 HTTP를 얹어서 보안 기반의 통신을 하는 것!
> = SSL 암호화 통신 by 공개키 암호화 방식 알고리즘

공개키 암호화 방식은, 공개키 자체가 위조될 수 있다는 위험이 있다.
=> 어떻게 해결할까?
=> SSL 인증서
<br/>

##### SSL 인증서와 CA
- SSL인증서는, 서버에서 주는 공개키가 신뢰할 수 잇는 것인지 확인시켜주는 인증서이다.
- 이때, '공개키가 해당 서버에서 온 것'과 관련한 인증서 발급의 주체: CA
	- Certificate Authority. 공인된 인증기관

```
HTTPS는 공개키 암호화 방식 + SSL 인증서를 통해 해킹을 방지한다.
```
<br/>

##### HTTPS를 사용하는 이유
1. 기밀성: 두 참여자간 통신을 보호해준다.
2. 무결성: 변조되지 않은 정보로 목적지에 도달하게 한다.
3. 인증: 웹사이트 진위 여부 확인이 가능하다.

<br/>

```
HTTPS일때,
📱비밀번호:1234 -> HTTP -> 💻비밀번호:A!B2
```
<br/>

#### 정리
> HTTPS는 보안측면과 SEO 측면에서 장점이 있으므로, HTTP보다 HTTPS 사용을 지향하자.