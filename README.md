
<div><h1>기술면접 대비공부</h1></div>
<div>
    <h3>JAVA SE</h3>
    <div><a href="#javase1">&nbsp;1. 사용해 본 웹 컨테이너는?</a></div>
    <div><a href="#javase2">&nbsp;2. JVM 의 메모리 구조를 설명하세요.</a></div>
    <div><a href="#javase3">&nbsp;3. 스레드의 생명주기를 설명하세요.</a></div>
    <div><a href="#javase4">&nbsp;4. 인터페이스란 무엇인가?</a></div>
    <div><a href="#javase5">&nbsp;5. 추상클래스란 무엇인가?</a></div>
    <div><a href="#javase6">&nbsp;6. 다형성이란 무엇인가?</a></div>
    <div><a href="#javase7">&nbsp;7. 컬렉션 프레임웍이란 무엇인가?</a></div>
    <div><a href="#javase8">&nbsp;8. Boxing과 unBoxing이란 무엇인가?</a></div>
    <div><a href="#javase9">&nbsp;9. 스트림의 종류를 설명하세요.</a></div>
    <div><a href="#javase10">10. JDBC란 무엇인가?</a></div>
</div>
<div>
    <h3>JAVA EE</h3>
    <div><a href="#javaee1">&nbsp;1. 커넥션풀링이란 무엇인가?</a></div>
    <div><a href="#javaee2">&nbsp;2. 모델1과 모델2의 차이점은?</a></div>
    <div><a href="#javaee3">&nbsp;3. MVC 패턴이 무엇이고 왜 사용하는가?</a></div>
    <div><a href="#javaee4">&nbsp;4. 모델2란 무엇인가?</a></div>
    <div><a href="#javaee5">&nbsp;5. WAS란 무엇이고 사용해본 제품은 어떤것이 있는가?</a></div>
    <div><a href="#javaee6">&nbsp;6. X-Internet 이란 무엇이고 사용해본 솔루션에는 어떤 것이 있는가?</a></div>
    <div><a href="#javaee7">&nbsp;7. 사용해본 데이터베이스 모델링 툴은 어떤게 있는가?</a></div>
    <div><a href="#javaee8">&nbsp;8. 서블릿의 생명주기를 설명하세요.</a></div>
    <div><a href="#javaee9">&nbsp;9. jar 와 war의 차이점은 무엇인가?</a></div>
    <div><a href="#javaee10">10. 바인드변수란 무엇인가?</a></div>
    <div><a href="#javaee11">11. 디자인패턴이란 무엇이고 개발시 적용해본 패턴에는 어떤것이 있는가?</a></div>
    <div><a href="#javaee12">12. 바인드변수란 무엇인가?</a></div>
    <div><a href="#javaee13">13. 사용할 수 있는 IDE에는 무엇이 있는가?</a></div>
    <div><a href="#javaee14">14. VCS(Version Control System)에 대해 설명하고, 이 중 사용할 수 있는 시스템은 무엇인 가?</a></div>
    <div><a href="#javaee15">15. 프레임워크란 무엇인가?</a></div>
    <div><a href="#javaee16">16. ORM 프레임웍은 무엇인가?</a></div>
    <div><a href="#javaee17">17. SQL 매핑 프레임웍은 무엇인가?</a></div>
    <div><a href="#javaee18">18. SpringMVC 란 무엇인가?</a></div>
    <div><a href="#javaee19">19. POJO 란 무엇인가?</a></div>
</div>

<!--공백--><div><br><br></div>

<div>
    <h2 id="javase1">1. 사용해 본 웹 컨테이너는?</h2>
    <h3>Tomcat 입니다.</h3>
    <p>+ 아파치 톰캣(Apache Tomcat)을 사용해보았습니다.</p>
    <p>+ Tomcat 이란 Java Servlet을 실행하고 JSP 가 포함된 웹 페이지를 렌더링하는 Apache Software Foundation의 응용 프로그램 서버입니다.
    톰캣은 웹 서버와 연동하여 실행할 수 있는 자바 환경을 제공하여 자바 서버 페이지(JSP)와 자바 서블릿이 실행할 수 있는 환경을 제공하고 있습니다. 톰캣은 관리툴을 통해 설정을 변경할 수 있지만, XML 파일을 편집하여 설정할 수도 있습니다. 그리고, 톰캣은 HTTP 서버도 자체 내장하기도 합니다.</p>
    <p>Tomcat is an application server from the Apache Software Foundation that executes Java servlets and renders Web pages that include Java Server Page coding. Described as a "reference implementation" of the Java Servlet and the Java Server Page specifications, Tomcat is the result of an open collaboration of developers and is available from the Apache Web site in both binary and source versions. Tomcat can be used as either a standalone product with its own internal Web server or together with other Web servers, including Apache, Netscape Enterprise Server, Microsoft Internet Information Server (IIS), and Microsoft Personal Web Server. Tomcat requires a Java Runtime Enterprise Environment that conforms to JRE 1.1 or later.</p>
    
    → https://www.theserverside.com/definition/Tomcat
    → https://ko.wikipedia.org/wiki/%EC%95%84%ED%8C%8C%EC%B9%98_%ED%86%B0%EC%BA%A3
</div>

<!--공백--><div><br><br></div>

<div>
    <h2 id="javase2">2. JVM 의 메모리 구조를 설명하세요.</h2>
    <h3>JVM</h3>
    <p>JVM은 실행될 클래스 파일을 메모리에 로드 후 초기화 작업을 수행합니다. 메소드와 클래스변수들을 해당 메모리 영역에 배치하고 클래스로드가 끝난 후 JVM 은 main 메소드를 찾아 지역변수, 객체변수, 참조변수를 스택에 쌓습니다. 다음 라인을 진행하면서 상황에 맞는 작업(함수 호출, 객체 할당 등)을 수행합니다.</p>
    <h3>JVM의 메모리 구조</h3>
</div>

<div><br><br></div>

<div>
    <h2 id="javase3">3. 스레드의 생명주기를 설명하세요.</h2>
    <p>하나의 프로세스 내부에서 독립적으로 실행되는 하나의 작업 단위입니다.</p>
</div>

<div><br><br></div>

<div>
    <h2 id="javase4">4. 인터페이스란 무엇인가?</h2>
    <p>+ 메소드에 대한 명세와 상수만 존재합니다. 인터페이스를 상속받은 클래스는 인터페이스에 있는 모든 메소드를 구현해야 합니다.</p>
    <p>+ 추상 클래스는 구현된 메서드를 포함할 수 있지만 인터페이스는 아닙니다. 인터페이스는 포함된 메서드를 정의하고 인터페이스가 규정하는 일반 규약을 지키기만 하면 됩니다.</p>
</div>

<div><br><br></div>

<div>
    <h2 id="javase5">5. 추상클래스란 무엇인가?</h2>
    <p>+ 하나 이상의 추상 메소드를 포함하는 클래스입니다. 추상 클래스 자체로는 클래스로써의 역할을 하지 못하며 객체를 생성할 수 없지만, 새로운 클래스를 작성하는데 있어 부모클래스로써 중요한 역할을 합니다.</p>
    <p>+ 인스턴스의 생성이 불가능하며, 해당 클래스를 extends 하여 추상 메소드를 구현해야만 사용 가능합니다.</p>
</div>

<div><br><br></div>

<div>
    <h2 id="javase6">6. 다형성이란 무엇인가?</h2>
    <h3>polymorphism</h3>
    <p></p>
</div>

<div><br><br></div>

<div>
    <h2 id="javase7">7. 컬렉션 프레임웍이란 무엇인가?</h2>
    <h3>Collection Framework</h3>
    <p></p>
</div>

<div><br><br></div>

<div>
    <h2 id="javase8">8. Boxing과 unBoxing이란 무엇인가?</h2>
    <h3>Boxing</h3>
    <p>+ </p>
    <h3>unBoxing</h3>
    <p></p>
</div>

<div><br><br></div>

<div>
    <h2 id="javase9">9. 스트림의 종류를 설명하세요.</h2>
    <h3>InputStream</h3>
    <p></p>
    <h3>OutputStream</h3>
    <p></p>
</div>

<div><br><br></div>

<div>
    <h2 id="javase10">10. JDBC란 무엇인가?</h2>
    <h3>JDBC</h3>
    <p></p>
</div>

<!--공백--><div><br><br></div>
