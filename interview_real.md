
<div id="top"><h1>실제로 받았던 질문과 예상 모법답안 정리</h1></div>
<div>
    <h3>기술면접 질문</h3>
    <div><a href="#stack_q1">&nbsp;1. Hashmap 과 Hashtable의 차이점이 뭔가요?</a></div>
    <div><a href="#stack_q2">&nbsp;2. Spring을 사용하는 이유는 무엇인가요?</a></div>
    <div><a href="#stack_q3">&nbsp;3. 회사 채용공고에 기재된 개발언어에 대해 생각나는대로 말해주세요.</a></div>
    <div><a href="#stack_q4">&nbsp;4. TPS가 뭔지 아는대로 설명해주세요.</a></div>
    <div><a href="#stack_q5">&nbsp;5. 가장 자신있는 스킬 한가지를 말해주세요.</a></div>
    <div><a href="#stack_q6">&nbsp;6. Angular와 React의 차이점이 뭔지 아는대로 설명해주세요.</a></div>
    <div><a href="#stack_q7">&nbsp;7. 젠킨스로 서버 배포하는 것에 대해 아시나요?</a></div>
    <div><a href="#stack_q8">&nbsp;8. 사용자 정의 에러처리를 해보았나요?</a></div>
    <div><a href="#stack_q9">&nbsp;9. 본인의 러닝커브는 어떻게 되나요?</a></div>
    <div><a href="#stack_q10">&nbsp;10. 새로운 지식을 배울 때 주로 어디에서 공부하나요?</a></div>
</div>
<div>
    <h3>업무관련 질문</h3>
    <div><a href="#work_q1">&nbsp;1. 저희 회사는 칸반에 스프린트로 업무 프로세스를 관리합니다. 칸반에 대해 아는 바가 있다면 말씀해주세요.</a></div>
    <div><a href="#work_q2">&nbsp;2. 회사에 있었으면 하는 복지가 있나요?</a></div>
    <div><a href="#work_q3">&nbsp;3. 회사 업무내용에 대해 궁금한 점이 있나요?</a></div>
    <div><a href="#work_q4">&nbsp;4. 하나의 업무만이 아닌 때론 CS관련 업무를 진행할 수도 있습니다. 괜찮으신가요?</a></div>
    <div><a href="#work_q5">&nbsp;5. 다녔던 직장에서 코드리뷰를 해보셨나요?</a></div>
</div>
<div>
    <h3>개인 질문&nbsp;</h3>
    <div>&nbsp;개발로 전향하게된 이유가 무엇인가요?</div>
    <div>&nbsp;이력사항 중 공백기가 있습니다. 그 기간에는 무엇을 하셨나요?</div>
    <div>&nbsp;기억에 남는 대외활동이나 알바같은 사회활동 두 가지를 말해줄 수 있나요?</div>
    <div>&nbsp;이 회사에 지원하게된 이유는 무엇인가요?</div>
    <div>&nbsp;나중에 회사가 다른 지역으로 이사를 갈 수도 있습니다. 괜찮으신가요?</div>
</div>

<!-- ==================== ==================== 자료구조 질문 ==================== ==================== -->
<div><br><br></div><hr id="stack_q1">
<div>
    <h3>1. Hashmap 과 Hashtable의 차이점이 뭔가요?&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>HashMap은 동기화되지 않습니다. 스레드가 안전하지 않으며 적절한 동기화 코드없이 많은 스레드간 공유가 힘들지만 Hashtable은 동기화가 가능합니다. 스레드가 안전하고 많은 스레드와 공유 할 수 있습니다. HashMap은 하나의 null 키와 여러 null 값을 허용하지만 Hashtable은 null 키나 값을 허용하지 않습니다. 스레드 동기화가 필요하지 않은 경우 일반적으로 HashMap이 HashTable보다 선호됩니다.</p>
    <a href="https://simuing.tistory.com/260">https://simuing.tistory.com/260</a>
</div>

<div><br><br></div><hr id="stack_q2">
<div>
    <h3>2. Spring을 사용하는 이유는 무엇인가요?&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>
        
    스프링 주요특징
    1. POJO 기반의 구성
    2. 의존성 주입(DI)을 통한 객체 간의 관계 구성
    3. AOP(Aspect-Oriented-Programminig)지원
    4. 편리한 MVC 구조
    5. WAS에 종속적이지 않은 개발 환경

    스프링 버전별 암기사항
    1. Spring 2.5 : Annotation 도입
    2. Spring 3.0 : 별도 설정 없이 Java 클래스만으로 설정 파일을 대신할 수 있게 지원
    3. Spring 4.0 : 모바일/웹 환경에서 많이 사용되는 REST 방식의 컨트롤러 지원
    
    </p>
</div>

<div><br><br></div><hr id="stack_q3">
<div>
    <h3>3. 회사 채용공고에 기재된 개발언어에 대해 생각나는대로 말해주세요.&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>백엔드 포지션에는 ~~이 있었고 프론트엔드 포지션에는 ~~이 있었던 걸로 기억납니다.</p>
</div>

<div><br><br></div><hr id="stack_q4">
<div>
    <h3>4. TPS가 뭔지 아는대로 설명해주세요.&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>초당 트랜잭션 (TPS)은 초당 실행 된 트랜잭션 수입니다. 즉, 특정 테스트 기간 동안 실행 된 트랜잭션 수를 기반으로 계산 한 다음 1 초 동안 계산할 수 있습니다.</br>예를 들어, vuser가 1 분마다 6 개의 트랜잭션을 실행하면 TPS는 6 개의 트랜잭션 / 60 초 = 0.10 TPS입니다.</p>
    <a href="https://theperformanceengineer.com/2013/09/11/loadrunner-how-to-calculate-transaction-per-second-tps/">https://theperformanceengineer.com/2013/09/11/loadrunner-how-to-calculate-transaction-per-second-tps/</a>
</div>

<div><br><br></div><hr id="stack_q5">
<div>
    <h3>5. 가장 자신있는 스킬 한가지를 말해주세요.&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>개발 언어 스킬로는 javascript이며 개인 스킬로는 일에 대한 적응력이 뛰어납니다.</p>
</div>

<div><br><br></div><hr id="stack_q6">
<div>
    <h3>6. Angular와 React의 차이점이 뭔지 아는대로 설명해주세요.&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>앵귤러는 프레임워크이고 리액트는 라이브러리입니다.</p>
</div>

<div><br><br></div><hr id="stack_q7">
<div>
    <h3>7. 젠킨스로 서버 배포하는 것에 대해 아시나요?&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>젠킨스( Jenkins )는 빌드, 테스트, 배포 등의 지속적인 통합을 자동화 해주는 툴입니다. (작성중)</p>
</div>

<div><br><br></div><hr id="stack_q8">
<div>
    <h3>8. 사용자 정의 에러처리를 해보았나요?&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>네. 실무에서 사용해보진 않았고 예제를 통해 실습한 적이 있습니다.<br/>사용자 정의 에러처리는 Exception 클래스를 상속받아 생성자 선언을 포함시킨 후 사용자 정의에 따른 예외처리를 할 수 있습니다.</p>
</div>

<div><br><br></div><hr id="stack_q9">
<div>
    <h3>9. 본인의 러닝커브는 어떻게 되나요?&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>습득할 지식에 따라 다를 것 같습니다. jQuery같은 경우는 며칠도 안걸릴 것이고 회사의 프레임워크를 배우는데에는 한달정도 소요되는 편입니다.</p>
</div>

<div><br><br></div><hr id="stack_q10">
<div>
    <h3>10. 새로운 지식을 배울 때 주로 어디에서 공부하나요?&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>인터넷 검색을 통해 파악한 뒤 기초를 공부합니다. 그리고 깊이 있게 공부할 땐 책을 구입해서 병행합니다.</p>
</div>


<!-- ==================== ==================== 업무관련 질문 ==================== ==================== -->
<div><br><br></div><hr id="work_q1">
<div>
    <h3>1. 저희 회사는 칸반에 스프린트로 업무 프로세스를 관리합니다. 칸반에 대해 아는 바가 있다면 말씀해주세요.&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p></p>
</div>

<div><br><br></div><hr id="work_q2">
<div>
    <h3>2. 회사에 있었으면 하는 복지가 있나요?&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>도서 지원이 있었으면 좋겠습니다. 개인 도서로 구입하는 형태가 아닌 회사에 책장이 있어 빌려 읽는 방식으로 진행할 수 있었으면 좋겠습니다.</p>
</div>

<div><br><br></div><hr id="work_q3">
<div>
    <h3>3. 회사 업무내용에 대해 궁금한 점이 있나요?&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>채용공고나 앱스토어에 올라온 어플 샘플에 의하면 ~~하는 일을 할 것 같은데 맞는지 궁금합니다.</p>
</div>

<div><br><br></div><hr id="work_q4">
<div>
    <h3>4. 하나의 업무만이 아닌 때론 CS관련 업무를 진행할 수도 있습니다. 괜찮으신가요?&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>네. 어린 아이들부터 어른들까지 저를 좋아하는 편이라 할 수 있습니다.<br/>
        (simuing_기분이 상하지 않도록 대응할 수 있다는 의미로 답하였습니다.)</p>
</div>

<div><br><br></div><hr id="work_q5">
<div>
    <h3>5. 다녔던 직장에서 코드리뷰를 해보셨나요?&nbsp;&nbsp;<a href="#top">↑</a></h3>
    <p>네. 회사차원에서 진행한 적은 없지만 동료끼리 자체적으로 코드리뷰를 진행한 적이 있습니다.</p>
</div>
