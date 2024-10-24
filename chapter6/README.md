## 6. 서블릿/JSP를 활용해 동적인 웹 애플리케이션 개발하기

### 6.1	서블릿/JSP로 회원관리 기능 다시 개발하기
* https://youtu.be/0VpYSAR8x28: Github 저장소 코드를 이클립스에 가져와 메이븐 빌드하는 과정

### 6.2	세션(HttpSession) 구현하기
#### 6.2.1 세션 구현하기 실습
[세션 구현하기 실습 문서](6.2 세션 구현하기 실습.pdf)

### 6.4	MVC 프레임워크 실습 1단계
#### 6.4.1 MVC 프레임워크 1단계 구현 실습
[MVC 프레임워크 1단계 구현 실습 문서](6.4 MVC 프레임워크 1단계 구현 실습.pdf)

### 6.6	쉘 스크립트를 활용한 배포 자동화
#### 6.6.1 배포 자동화 실습
[쉘 스크립트를 활용한 배포 자동화 실습 문서](6.6 쉘 스크립트를 활용한 배포 자동화 실습.pdf)

#### 6.6.3	동영상을 참고한 배포 자동화 실습
* https://youtu.be/ZsiO27LeW34 동영상은 서버에 톰캣(tomcat) 서버를 설치 및 설정하고, 톰캣 서버가 정상적으로 시작했는지 확인하는 방법을 다룬다.
* https://youtu.be/9Rr4gMRyUtQ 동영상은 톰캣 서버에 대한 기본적인 설명과 각 디렉토리별 용도에 대해 설명한다. 이 동영상은 톰캣과 관련한 최소한의 내용만 다룬다. 따라서 다른 책이나 온라인 문서를 통해 추가학습해야 한다.
* https://youtu.be/bzM1WL4qdoA 동영상은 톰캣에 웹 애플리케이션을 배포하는 과정에 대해 다룬다. 메이븐을 통해 빌드하고 빌드한 프로젝트를 톰캣에 수동으로 배포하는 과정을 담고 있다.

자바 웹 애플리케이션을 배포하는 방법은 war 파일을 만들어 배포하는 방법과 war 파일로 묶지 않고 디렉토리 자체를 배포하는 두 가지 방법이 있다. 이 두 가지 방법 중 각자의 서비스에 적합한 방법을 선택해 사용하면 된다.

소스 코드를 빌드/배포하는 과정에서 수 많은 반복 작업이 발생한다. 반복 작업은 사람의 실수를 유발하고 이는 대규모 장애로 이어진다. 따라서 반복 작업은 컴퓨터를 통해 자동화하는 것이 가장 안전하다. 그리고 개발자는 소중한 존재이므로 이런 하찮은 반복 작업에 시간을 쓰지 않도록 노력해야 한다. 틈틈히 쉘 스크립트를 구현하는 연습을 하면 많은 반복 작업을 줄일 수 있다.

* https://youtu.be/U7tZnEiYJyE 동영상은 배포 과정에서 발생하는 반복 과정에 대한 설명, 쉘 스크립트 파일을 만들어 배포 과정을 자동화하는 방법에 대해 다룬다.

### 6.7	추가 학습 자료
#### 6.7.1	쿠키와 세션, 보안
쿠키와 세션의 동작방식의 차이점을 이해하고 제대로 사용하는 것은 안전한 웹 애플리케이션을 만들기 위한 시작 단계이다. 아직까지 쿠키와 세션의 차이점을 명확히 이해하지 못한다면 **프로가 되기 위한 웹기술 입문(고모라 유스케 저/김정환 역, 위키북스/2012)** 책의 4장을 통해 추가학습할 것을 추천한다. 많은 책에서 쿠키와 세션의 차이점에 대해 설명하고 있지만 이 책의 “4장 CGI에서 웹 애플리케이션으로”에서 쉽고 자세하게 설명하고 있다.

쿠키와 세션의 차이를 이해하고 사용하는 것은 안전한 웹을 만들기 위한 첫 걸음이었다면 보안에 대한 다음 걸음은 웹 애플리케이션에 대한 다양한 공격 방법과 이에 대한 대응 방법을 학습하는 것이다. **프로가 되기 위한 웹기술 입문(고모라 유스케 저/김정환 역, 위키북스/2012)** 책의 “7장 보안을 확보하기 위한 방법”에서 학습할 수 있다. 대표적인 공격 방법 중 SQL 인젝션, 크로스 사이트 스크립팅(XSS), 세션 하이재킹, 크로스 사이트 요청 위조(CSRF)에 대해서만이라도 이해하고 대책을 마련할 것을 추천한다.

HTTP 학습 과정에서 추천한 **HTTP & Network : 그림으로 배우는 책으로 학습(우에노 센 저/이병억 역, 영진닷컴/2015)** 책의 7장, 8장, 11장 내용도 안전한 웹 애플리케이션 개발에 대한 내용을 포함하고 있으니 같이 학습하면 좋다.

#### 6.7.2	쉘 스크립트와 배포 자동화
나는 웹 백엔드 개발자로 살아가면서 쉘 스크립트를 작성하는 경우가 생각보다 많지 않았다. 어쩌면 내 자신이 쉘 스크립트에 익숙하지 않기 때문에 사용하는 것을 꺼릴 수도 있었다. 아니 쉘 스크립트를 활용하기보다 같은 기능을 지원하는 다른 도구를 찾아 적용했다는 것이 맞을 수 있겠다. 어떤 도구를 사용하던 원하는 목적을 달성하면 된다. 즉, 개발자가 단순, 반복적으로 하는 작업을 최소한의 시간 투자로 자동화할 수 있다면 그 자체로 목적을 달성하는 것과 같다.

쉘 스크립트를 활용하면 개발자의 무수히 많은 단순, 반복적인 수동 작업을 자동화하는 것이 가능하다. 특히 웹 백엔드 개발자에게 자동화된 배포 환경을 구축하는 것은 많은 시간을 아낄 수 있는 중요한 작업이다. 이 환경을 구축하기 위해 학습해야할 주제가 메이븐, 그래들과 같은 빌드 도구와 쉘 스크립트를 활용한 배포 자동화이다.

쉘 스크립트에 대한 기본적인 학습은 **리눅스 커맨드라인 완벽 입문서(윌리엄 E. 샤츠 주니어 저/이종우, 정영신 역, 비제이퍼블릭/2013년 1월)** 책의 PART4를 통해 학습할 수 있다. 쉘 스크립트 작성 능력을 키우려면 책을 통해서는 한계가 있기 때문에 작은 것이라도 자기 주변에서 발생하는 불편한 점을 쉘 스크립트를 통해 개선해 나가는 경험을 하는 것이 가장 좋은 학습 방법이다. 지금까지 다른 사용자를 위한 소프트웨어를 개발했다면 지금부터 쉘 스크립트를 통해 자신에게 필요한 도구를 만드는 경험을 해보자.

----
# Table of Contents
### 1부. 첫 번째 양파 껍질
##### [1. 첫 번째 양파 껍질 벗기기](../chapter1)
### [2부. 두 번째 양파 껍질](../2nd-onion.md)
##### [2. 문자열 계산기 구현을 통한 테스트와 리팩토링](../chapter2)
##### [3. 개발 환경 구축 및 웹 서버 실습 요구사항](../chapter3)
##### [4. HTTP 웹 서버 구현을 통해 HTTP 이해하기](../chapter4)
##### [5. 웹 서버 리팩토링, 서블릿 컨테이너/서블릿 과의 관계](../chapter5)
##### [6. 서블릿/JSP를 활용해 동적인 웹 애플리케이션 개발하기](../chapter6)
##### [7. DB를 활용해 데이터를 영구적으로 저장하기](../chapter7)
##### [8. Ajax를 활용해 새로고침 없이 데이터 갱신하기](../chapter8)
##### [9. 두 번째 양파 껍질을 벗기기 위한 중간 점검](../chapter9)
##### [10. 새로운 MVC 프레임워크 구현을 통한 점진적 개선](../chapter10)
##### [11. 의존관계 주입(이하 DI) 을 통한 테스트하기 쉬운 코드 만들기](../chapter11)
##### [12. 확장성 있는 DI 프레임워크로 개선](../chapter12)
### 3부. 세 번째 양파 껍질
##### [13. 세 번째 양파 껍질](../chapter13)