
<div><h1>Java 백엔드 기술면접 대비공부</h1></div>
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
    <div><a href="#javaee11">11. 커넥션 풀이란 무엇인가?</a></div>
    <div><a href="#javaee12">12. 모델1과 모델2의 차이점은?</a></div>
    <div><a href="#javaee13">13. MVC 패턴이 무엇이고 왜 사용하는가?</a></div>
    <div><a href="#javaee14">14. 모델2란 무엇인가?</a></div>
    <div><a href="#javaee15">15. WAS란 무엇이고 사용해본 제품은 어떤것이 있는가?</a></div>
    <div><a href="#javaee16">16. X-Internet 이란 무엇이고 사용해본 솔루션에는 어떤 것이 있는가?</a></div>
    <div><a href="#javaee17">17. 사용해본 데이터베이스 모델링 툴은 어떤게 있는가?</a></div>
    <div><a href="#javaee18">18. 서블릿의 생명주기를 설명하세요.</a></div>
    <div><a href="#javaee19">19. jar 와 war의 차이점은 무엇인가?</a></div>
    <div><a href="#javaee20">20. 바인드변수란 무엇인가?</a></div>
    <div><a href="#javaee21">21. 디자인패턴이란 무엇이고 개발시 적용해본 패턴에는 어떤것이 있는가?</a></div>
    <div><a href="#javaee22">22. 사용할 수 있는 IDE에는 무엇이 있는가?</a></div>
    <div><a href="#javaee23">23. VCS(Version Control System)에 대해 설명하고, 이 중 사용할 수 있는 시스템은 무엇인 가?</a></div>
    <div><a href="#javaee24">24. 프레임워크란 무엇인가?</a></div>
    <div><a href="#javaee25">25. ORM 프레임웍은 무엇인가?</a></div>
    <div><a href="#javaee26">26. SQL 매핑 프레임웍은 무엇인가?</a></div>
    <div><a href="#javaee27">27. SpringMVC 란 무엇인가?</a></div>
    <div><a href="#javaee28">28. POJO 란 무엇인가?</a></div>
</div>

<!--공백--><div><br><br></div><hr id="javase1">
<div>
    <h2>1. 사용해 본 웹 컨테이너는?</h2>
    <p>+ Tomcat 이 있습니다.</p>
    <p>+ 아파치 톰캣(Apache Tomcat)을 사용해보았습니다.</p>
    <p>+ Tomcat 이란 Java Servlet을 실행하고 JSP 가 포함된 웹 페이지를 렌더링하는 Apache Software Foundation의 응용 프로그램 서버입니다.
    톰캣은 웹 서버와 연동하여 실행할 수 있는 자바 환경을 제공하여 자바 서버 페이지(JSP)와 자바 서블릿이 실행할 수 있는 환경을 제공하고 있습니다. 톰캣은 관리툴을 통해 설정을 변경할 수 있지만, XML 파일을 편집하여 설정할 수도 있습니다. 그리고, 톰캣은 HTTP 서버도 자체 내장하기도 합니다.</p>
    <p>Tomcat is an application server from the Apache Software Foundation that executes Java servlets and renders Web pages that include Java Server Page coding. Described as a "reference implementation" of the Java Servlet and the Java Server Page specifications, Tomcat is the result of an open collaboration of developers and is available from the Apache Web site in both binary and source versions. Tomcat can be used as either a standalone product with its own internal Web server or together with other Web servers, including Apache, Netscape Enterprise Server, Microsoft Internet Information Server (IIS), and Microsoft Personal Web Server. Tomcat requires a Java Runtime Enterprise Environment that conforms to JRE 1.1 or later.</p>
    → https://www.theserverside.com/definition/Tomcat
    → https://ko.wikipedia.org/wiki/%EC%95%84%ED%8C%8C%EC%B9%98_%ED%86%B0%EC%BA%A3
</div>

<!--공백--><div><br><br></div><hr id="javase2">
<div>
    <h2>2. JVM 의 메모리 구조를 설명하세요.</h2>
    <h3>자바가상머신(Java Virtual Machine, JVM)</h3>
    <p>JVM은 실행될 클래스 파일을 메모리에 로드 후 초기화 작업을 수행합니다. 메소드와 클래스변수들을 해당 메모리 영역에 배치하고 클래스로드가 끝난 후 JVM 은 main 메소드를 찾아 지역변수, 객체변수, 참조변수를 스택에 쌓습니다. 다음 라인을 진행하면서 상황에 맞는 작업(함수 호출, 객체 할당 등)을 수행합니다.</p>
    <h3>JVM의 메모리 구조</h3>
    <p>+ 프로그램을 실행하기 위한 데이터 및 명령어를 저장하는 공간을 말합니다. 즉 응용프로그램이 실행되면 JVM은 이 메모리를 사용하게 됩니다.</p>
    <ul>
    <dl>JAVA Source : 사용자가 작성한 JAVA 코드</dl>
    <dl>JAVA Compiler : JAVA 코드를 Byte Code로 변환시켜주는 기능</dl>
    <dl>Class Loader : Class 파일을 메모리(Runtime Data Area)에 적재하는 기능</dl>
    <dl>Execution Engine : Byte Code를 실행 가능하게 해석해주는 기능</dl>
    <dl>Runtime Data Area : 프로그램을 수행하기 위해 OS에서 할당 받은 메모리 공간</dl>
    </ul>
    <h3>왜 JVM 메모리 구조를 알아야 하는가?</h3>
    <p>+ 같은 기능의 프로그램이더라도 메모리 관리에 따라 성능이 좌우됩니다. 메모리 관리가 되지 않은 경우 속도저하 현상이나 튕김 현상 등이 일어날 수 있어 한정된 메모리를 효율적으로 사용하기 위해 JVM의 메모리 구조를 아는 것이 중요합니다.</p>
    → http://www.incodom.kr/%EC%9E%90%EB%B0%94%EA%B0%80%EC%83%81%EB%A8%B8%EC%8B%A0%28Java_Virtual_Machine%2C_JVM%29/%EB%A9%94%EB%AA%A8%EB%A6%AC%EA%B5%AC%EC%A1%B0
</div>

<!--공백--><div><br><br></div><hr id="javase3">
<div>
    <h2>3. 스레드의 생명주기를 설명하세요.</h2>
    <p>하나의 프로세스 내부에서 독립적으로 실행되는 하나의 작업 단위입니다.</p>
</div>

<!--공백--><div><br><br></div><hr id="javase4">
<div>
    <h2>4. 인터페이스란 무엇인가?</h2>
    <p>+ 메소드에 대한 명세와 상수만 존재합니다. 인터페이스를 상속받은 클래스는 인터페이스에 있는 모든 메소드를 구현해야 합니다.</p>
    <p>+ 추상 클래스는 구현된 메서드를 포함할 수 있지만 인터페이스는 아닙니다. 인터페이스는 포함된 메서드를 정의하고 인터페이스가 규정하는 일반 규약을 지키기만 하면 됩니다.</p>
</div>

<!--공백--><div><br><br></div><hr id="javase5">
<div>
    <h2>5. 추상클래스란 무엇인가?</h2>
    <p>+ 하나 이상의 추상 메소드를 포함하는 클래스입니다. 추상 클래스 자체로는 클래스로써의 역할을 하지 못하며 객체를 생성할 수 없지만, 새로운 클래스를 작성하는데 있어 부모클래스로써 중요한 역할을 합니다.</p>
    <p>+ 인스턴스의 생성이 불가능하며, 해당 클래스를 extends 하여 추상 메소드를 구현해야만 사용 가능합니다.</p>
</div>

<!--공백--><div><br><br></div><hr id="javase6">
<div>
    <h2>6. 다형성이란 무엇인가?</h2>
    <h3>다형성(polymorphism)</h3>
    <p>+ 객체지향 프로그래밍의 특징 중 하나인 다형성은 같은 모양의 코드가 다른 행위를 하는 것을 나타냅니다. 자바에서 다형성의 개념을 녹여낸 방법은 오버라이딩과 오버로딩 두 가지가 있습니다.</p>
    <p>+ [고급]오버라이딩은 대상이 되는 함수를 런타임 시점에 정의하고 오버로딩은 컴파일 시점에 정의합니다.</p>
    <h3>오버라이딩(Overriding)</h3>
    <p>오버라이딩은 슈퍼클래스를 상속받은 서브 클래스에서 슈퍼 클래스의 (추상) 메소드를 같은 이름, 같은 반환값, 같은 인자로 메소드 내의 로직들을 새롭게 정의하는 것을 말합니다.</p>
    <h3>오버로딩(Overloading)</h3>
    <p>오버로딩은 하나의 클래스에서 같은 이름의 메소드를 여러 개 가질 수 있게 합니다. 단 메소드의 인자들은 달라야합니다.</p>
    → https://brunch.co.kr/@kd4/4
</div>

<!--공백--><div><br><br></div><hr id="javase7">
<div>
    <h2>7. 컬렉션 프레임워크란 무엇인가?</h2>
    <p>+ 배열은 연관 데이터를 관리하기 위한 수단으로써 한번 정해진 배열의 크기를 변경할 수 없다는 불편함이 있습니다. 이 때 컬렉션 프레임워크를 사용하면 유동적인 크기의 배열을 만들 수 있게됩니다.</p>
    <p>[기존배열] String[] arrayObj = new String[2] //생성 후 배열크기 변경불가</p>
    <p>[컬렉션프레임워크] ArrayList&#60;String&#62; array = new ArrayList&#60;String&#62;(); //배열 크기 상관없이 생성 가능</p>
</div>

<!--공백--><div><br><br></div><hr id="javase8">
<div>
    <h2>8. Boxing과 unBoxing이란 무엇인가?</h2>
    <p>+ 박싱(Boxing)이란 기본형을 참조형으로 변환하고, 언박싱(unBoxing)이란 참조형을 기본형으로 변환합니다. JDK 1.5부터는 이것을 자동으로 해주는 오토박싱(AutoBoxing)기능이 추가되었습니다.</p>
</div>

<!--공백--><div><br><br></div><hr id="javase9">
<div>
    <h2>9. 스트림의 종류를 설명하세요.</h2>
    <p>+ 스트림이란 프로그램과 I/O 객체를 연결하여 데이터를 송수신 하는 길을 말합니다. InputStream은 데이터를 읽어 들이는 객체이고, OutputStream은 데이터를 써서 보내는 객체입니다.</p>
    <p>+ 데이터를 어떤 방식으로 전달하느냐에 따라 스트림은 바이트 스트림(Byte Stream)과 문자 스트림(Character Stream)으로 나뉩니다. 바이트 스트림은 binary 데이터를 입출력하는 스트림으로써 이미지, 동영상 등을 송수신할 때 주로 사용합니다. 문자 스트림은 말 그대로 text 데이터를 입출력하는데 사용하는 스트림으로써 html 문서, 텍스트 파일을 송수신할 때 사용합니다.</p>
    <h3>문자 단위 구성도</h3>
    <h4>입력 문자스트림 : Reader</h4>
    <h4>출력 문자스트림 : Writer</h4>
    <h4>입력 바이트 스트림 : InputStram</h4>
    <h4>출력 바이트 스트림 : OutputStram</h4>
    → http://victorydntmd.tistory.com/134
</div>

<!--공백--><div><br><br></div><hr id="javase10">
<div>
    <h2>10. JDBC란 무엇인가?</h2>
    <p>+ JDBC(Java Database Connectivity)란 데이터베이스에 접근하여 SQL문을 실행하기 위한 자바 라이브러리를 말합니다.</p>
    <p>+ 데이터베이스 벤더*들이 이러한 라이브러리를 각자 만든다면, 자바 프로그래머는 각 벤더가 만든 라이브러리 사용법을 익혀야 합니다.
JDBC는 선에서 만든, RDBMS에 접근하여 SQL문을 실행하기 위한, 자바 라이브러리를 말합니다. JDBC에는 구현클래스가 거의 없고 대부분이 인터페이스입니다. (그래서 표준이란 표현을 씀) 인터페이스를 구현한 클래스는 각 벤더가 만들어야 합니다.</p>
    <p>*벤더(vendor) : 제품 판매인 또는 판매업체 - 판매한 제품에 대해 책임을 지는 곳을 가리킵니다.(물품을 공급한곳) 벤더는 제품을 제조한 곳일 수도 있고. 다른 회사 제품을 판매만 하는 곳일 수도 있습니다.</p>
    → http://www.java-school.net/jdbc/JDBC-Intro
</div>

    

<!--공백--><div><br><br></div><hr id="javaee11">
<div>
    <h2>11. 커넥션 풀(Connection Pool, DBCP)이란 무엇인가?</h2>
    <p>+ 데이터베이스와 연결된 커넥션을 미리 만들어 풀(pool) 속에 저장해 두고 있다가 필요할 때 커넥션을 풀에서 쓰고 다시 풀에 반환하는 기법을 말합니다.</p>
    <p>+ 커넥션 풀이란 미리 커넥션 객체를 생성하고 해당 커넥션 객체를 관리하는것을 의미합니다.</p>
    <p>+ 웹 프로그램에서는 데이터베이스의 환경설정과 연결 관리 등을 따로 XML파일이나 속성 파일을 사용해서 관리하고, 이렇게 설정된 정보를 이름을 사용하여 획득하는 방법을 사용합니다.</p>
    <h3>커넥션풀(DBCP)의 특징</h3>
    <p>- 풀 속에 미리 커넥션이 생성되어 있기 때문에 커넥션을 생성하는 데 드는 연결 시간이 소비되지 않는다.<br>
    - 커넥션을 계속해서 재사용하기 때문에 생성되는 커넥션 수가 많지 않다.<br>
    - 커넥션 풀을 사용하면 커넥션을 생성하고 닫는 시간이 소모되지 않기 때문에 그만큼 어플리케이션의 실행 속도가 빨라지며, 또한 한 번에 생성될 수 있는 커넥션 수를 제어하기 때문에 동시 접속자 수가 몰려도 웹 어플리케이션이 쉽게 다운되지 않는다.</p>
    → http://devbox.tistory.com/entry/JSP-%EC%BB%A4%EB%84%A5%EC%85%98-%ED%92%80-1
</div>

<!--공백--><div><br><br></div><hr id="javaee12">
<div>
    <h2>12. 모델1과 모델2의 차이점은?</h2>
    <p>+ 모델1은 뷰와 로직을 모두 JSP페이지 하나에서 처리하는 방식이며 개발속도가 빠르지만 유지보수와 확장에 대한 어려움이 있습니다. 모델2는 모델1과 달리 JSP페이지, Servlet, 로직을 위한 클래스를 나뉘어 브라우저 요청을 처리하는 방식으로, 초기 구조설계에 많은 시간을 투자해야한다는 단점이 있으나 유지보수와 확장이 용이하다는 장점이 있습니다.</p>
    <p>MVC패턴(모델2) - <b>M</b>odel:javaBean, <b>V</b>iew:jsp, <b>C</b>ontroller:servlet</p>
</div>

<!--공백--><div><br><br></div><hr id="javaee13">
<div>
    <h2>13. MVC 패턴이 무엇이고 왜 사용하는가?</h2>
    <p>+ MVC란 Model View Controller의 약자로 에플리케이션을 세가지의 역할로 구분한 개발 방법론입니다. 사용자가 Controller를 조작하면 Controller는 Model을 통해서 데이터를 가져오고 그 정보를 바탕으로 시각적인 표현을 담당하는 View를 제어해서 사용자에게 전달하게 됩니다.</p>
</div>

<!--공백--><div><br><br></div><hr id="javaee14">
<div>
    <h2>14. 모델2란 무엇인가?</h2>
    <p>+ </p>
</div>

<!--공백--><div><br><br></div><hr id="javaee15">
<div>
    <h2>15. WAS란 무엇이고 사용해본 제품은 어떤것이 있는가?</h2>
    <p>+ WAS는 웹 프로그램을 실행할 수 있는 기초적인 환경을 제공하며 톰캣(Tomcat)을 사용해본 적이 있습니다.</p>
</div>

<!--공백--><div><br><br></div><hr id="javaee16">
<div>
    <h2>16. X-Internet 이란 무엇이고 사용해본 솔루션에는 어떤 것이 있는가?</h2>
    <p>+ </p>
</div>

<!--공백--><div><br><br></div><hr id="javaee17">
<div>
    <h2>17. 사용해본 데이터베이스 모델링 툴은 어떤게 있는가?</h2>
    <p>+ exERD와 draw.io가 있습니다.</p>
</div>

<!--공백--><div><br><br></div><hr id="javaee18">
<div>
    <h2>18. 서블릿의 생명주기를 설명하세요.</h2>
    <p>+ </p>
</div>

<!--공백--><div><br><br></div><hr id="javaee19">
<div>
    <h2>19. jar 와 war의 차이점은 무엇인가?</h2>
    <p>+ 엔터프라이즈 Java Bean (클래스 파일) 및 EJB 배치 디스크립터를 포함하는 EJB 모듈은 .jar 확장을 갖는 JAR 파일로 압축됩니다. 서블릿 클래스 파일, JSP 파일, 지원 파일, GIF 및 HTML 파일을 포함하는 웹 모듈은 확장자가 .war인 JAR 파일로 패키지됩니다. </p>
</div>

<!--공백--><div><br><br></div><hr id="javaee20">
<div>
    <h2>20. 바인드변수란 무엇인가?</h2>
    <p>+ </p>
</div>

<!--공백--><div><br><br></div><hr id="javaee21">
<div>
    <h2>21. 디자인패턴이란 무엇이고 개발시 적용해본 패턴에는 어떤것이 있는가?</h2>
    <p>+ 디자인 패턴이란 건축으로치면 공법에 해당하는 것으로 소프트웨어의 개발 방법을 공식화 한 것입니다. 소수의 뛰어난 엔지니어가 해결한 문제를 다수의 엔지니어들이 처리 할 수 있도록 한 규칙이면서, 구현자들 간의 커뮤니케이션의 효율성을 높이는 기법입니다.<br>
    교육이수 과정의 파이널 프로젝트로 MVC패턴을 적용한 적이 있습니다.</p>
</div>

<!--공백--><div><br><br></div><hr id="javaee22">
<div>
    <h2>22. 사용할 수 있는 IDE에는 무엇이 있는가?</h2>
    <p>+ 이클립스를 사용할 수 있습니다.</p>
</div>

<!--공백--><div><br><br></div><hr id="javaee23">
<div>
    <h2>23. VCS(Version Control System)에 대해 설명하고, 이 중 사용할 수 있는 시스템은 무엇인가?</h2>
    <p>+ </p>
</div>

<!--공백--><div><br><br></div><hr id="javaee24">
<div>
    <h2>24. 프레임워크란 무엇인가?</h2>
    <p>+ 틀, 뼈대, 약속이라고 볼 수 있습니다.</p>
</div>

<!--공백--><div><br><br></div><hr id="javaee25">
<div>
    <h2>25. ORM 프레임웍은 무엇인가?</h2>
    <p>+ </p>
</div>

<!--공백--><div><br><br></div><hr id="javaee26">
<div>
    <h2>26. SQL 매핑 프레임웍은 무엇인가?</h2>
    <p>+ </p>
</div>

<!--공백--><div><br><br></div><hr id="javaee27">
<div>
    <h2>27. SpringMVC 란 무엇인가?</h2>
    <p>+ </p>
</div>


<!--공백--><div><br><br></div><hr id="javaee28">
<div>
    <h2>28. POJO 란 무엇인가?</h2>
    <p>+ Plain Old Java Object 의 약자로 오래된 방식의 간단한 자바 오브젝트라는 말로서 Java EE 등의 중량 프레임워크들을 사용하게 되면서 해당 프레임워크에 종속된 "무거운" 객체를 만들게 된 것에 반발해서 사용되게 된 용어입니다. getter 와 setter 로 구성된 클래스 입니다.</p>
    → https://ko.wikipedia.org/wiki/Plain_Old_Java_Object
    → https://www.quora.com/What-is-POJO-in-Java
</div>

