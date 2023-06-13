### 에러 모음   
<br>
<br>
<br>

- https://start.spring.io/ 로 프로젝트 구성함   
- Gradle-Groovy / Java / Spring Boot 2.7.12 버전 / Java 11버전 사용   
(스프링부트 3.0 이상을 쓰면 자바 17로 해야된다길래 2.7.12버전으로 함)
- 인텔리제이 설치하고 main메서드 run하자마자 에러남
- 에러내용

```java
Execution failed for task ':HelloSpringApplication.main()'.
> Process 'command 'C:/Program Files/Java/jdk-11.0.16.1/bin/java.exe'' finished with non-zero exit value 1

* Try:
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights.
```

<br>
해결방법

1. [File > Settings] 메뉴 클릭(단축키: ctrl + alt + s)
2. [Build, Execution, Deployment > Build Tools > Gradle] 메뉴로 이동
3. Build and run using을 IntelliJ IDEA로 변경
4. Run tests using을 IntelliJ IDEA로 변경
5. Gradle JVM을 jdk11로 변경(없다면 설치)
<br>
<br>

--------------------------------------


<br>
<br>

- 이번엔 8080포트를 이미 사용중이라고 에러 발생. 이건 아마 오라클 포트라? 그런듯
- 에러 내용

```java
Description:

Web server failed to start. Port 8080 was already in use.

Action:

Identify and stop the process that's listening on port 8080 or configure this application to listen on another port.


Process finished with exit code 1
```

<br>
해결방법   

1. 인텔리제이 포트 번호를 바꾸든지   
2. 8080포트를 죽이든지 taskkill 


* 포트 번호 바꾸는 법    
  1. Run - Edit Configurations...로 들어간다.   
  2. Environment variables에 server.port='원하는 포트번호'로 수정한다.   


<br>
<br>

--------------------------------------


<br>
<br>
