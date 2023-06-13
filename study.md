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



