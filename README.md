# 스터디 규칙
1. 매주 스터디한 내용은 `Readme.MD`에 등록 (by 스터디장)
2. 매주 과제 출제, 스터디원들은 해당주차 과제가 `issues` 탭에 등록되오니 해당 issues란 `comment`로 등록
3. 나머지 1시간에 스터디원들의 발표주제는 `과제한 내용` or `공유하고 싶은 내용`으로 `선택`
4. 발표자는 2명, 스터디날짜 때 `추첨`으로 뽑힘 -> 누가 걸릴지 모르므로 각자 최선을...


# 스터디 일정

* `1주차(08/20)`
  - 자바 챌린지 스터디를 만든 idea 소개
  - 취지 -> 서로 스터디하면서 시너지를 낼 수 있는 환경설정, 기술 "공유" 세미나

  - POJO -> OOP 형식의 유지보수가능하게 돕는 자바 클래스, 데이터 그릇(Entity, Dto, VO 등)
    으로 활용, 우리 스터디에도 자바 프로그램의 in/out 흐름 파라미터로 사용!

  - Setting 환경: https://github.com/mooh2jj/javaChallenageProg.git
    - SpringBoot REST API로 Dto로 데이터값 POST방식(postman)으로 확인
    - 순수 자바 프로젝트로 진행해도 무관

  - 자바 성적 산출 프로그램 예시
    1) 비즈니스 로직 조건문 if 
    2) 도메인 주도 패턴 - 데이터처리로직 -> 관련 Domain Dto에 메서드로 이동
    3) stream API 로 데이터값 파싱

  - 향후계획: java챌린지스터디 -> Spring(Boot) REST API를 다루는 spring챌린지스터디 계획

<br>

* `2주차(8/27)`

  - Builder 패턴
    - 점증적 생성자 패턴 vs 빌더패턴
    - 빌더패턴 이슈 => `NoArgs, AllArgs의 문제` => AllArgsConstructors는 모든 필드에 대한 생성자 생성함. 
      하지만 인스턴스 맴버변수 순서의 영향을 받아 컴파일 오류가 아닌 런타임 오류가 생겨 치명적인 오류임! 
    - 결국에 NoArs와 Builder는 생성자에 넣는 방식으로 사용

  - String vs StringBuilder, StringBuffer 
    - 메모리 성능 차이 =>  "+=" vs "append()" 
    - 불변객체 String => Constant pool(상수풀) 메모리에 할당.
      - String 생성방식 ""(리터럴방식) vs new String(); (new 연산자 방식)
    - StringBuffer vs StringBuilder  (멀티스레드 동기화 블록 o, x)

  - String 메서드 
    - equals()	// equals() vs "=="
    - spilt() && join()
    - replaceAll() => `정규표현식` => 활용범위가 넓음. 리눅스에서도 많이 사용

