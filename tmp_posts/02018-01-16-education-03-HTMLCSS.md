---
title : [기술교육] HTML/CSS
layout: post
---

HTTP 헤더, HTTP 페이로드는 TCP 헤더 위에서 동작한다.

WWW = URL + HTTP + HTML(리소스 자체 기술)
    = 웹 브라우저가 웹서버의 HTML로 기술된 리소스를 URL 를 통해 요청하여 HTTP 프로토콜을 사용하여 받아서 표현하는 것

nc(Netcat) : TCP 서버/클라이언트 같이 사용 가능

GET (엔터티 바디 없음) : 리소스를 요청하기 위한 메서드
POST (엔터티 바디 있음) : 서버에 입력 데이타를 전송하기 위한 메서드, 주로 HTML 폼을 사용하기 위하여 많이 사용됨

내가 보낸 데이터 확인할 때. 서버에서 디버그 포인터 잡고 하는데 그 대신 httpbin.org 사이트 사용해도 ok

curl 명령어 : 리눅스에서 curl 이라는 http 메시지를 쉘상에서 요청하여 결과를 확인하는 명령어.
	      curl 명령어는 http를 이용하여 경로의 데이터를 가져옴
		$curl [옵션][URL...]

301 Moved Permanently(주소 바뀜)
영구적으로 바뀌면 브라우저가 캐시를 해야됨

Referer 헤더 : 어디서부터 왔는지 알 수 있는 주소(ex. 하이퍼링크로 이동시 이동 전 페이지를 전달)

Stateless : 매번 GET해서 이번것밖에 ㅁ르는 경우
이전 커넥션에 대해서 알고

Secure: https 커넥션인 경우에만 Cookie 로 전달
HttpOnly: javascript 에서 접근하지 못하도록 설정

서버쪽에서 세션(Session) 판단, 정렬

HTTP over SSL/TLS (HTTP가 SSL/TLS 위에 있음
ex) IP over Ethernet (IP가 이더넷 위에있음)

SSL/TLS : 암호화된 데이터를 전송하고받는 프로토콜

인증서(Certificate)가 공개키 안에 있음

---
# 기타 
ICMP 프로토콜 
>주로 핑(PING, Packet INternet Grouper) 테스트할 때 사용.

크롬 개발자 도구 -> Security -> application -> view certificate