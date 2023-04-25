##  ch1 프로그래밍 언어 소개

# 1.1 프로그래밍 언어란 무엇인가?

프로그래밍 언어: 기계가 읽을 수 있고 사람이 읽을 수 있는 형식으로 계산을 서술하기 위한 표기 체계

- 계산 (computation): 컴퓨터가 수행할 수 있는 작업
- 기계가 읽을 수 있는 (machine-readable): 문맥 자유 언어 (context free language)
- 사람이 읽을 수 있는 (human-readable): 추상화



#  1.2 프로그래밍 언어를 배워야 하는 이유

1. 현재 사용하고 있는 언어를 더 잘 이해하게 한다
2. 유용한 프로그래밍을 구사할 수 있는 능력을 증대시킨다
3. 프로그래밍 언어를 선택할 수 있는 능력을 증대시킨다
4. 새로운 프로그래밍 언어를 배우기 쉽게 해준다
5. 새로운 프로그래밍 언어를 설계하기 쉽게 해 준다





# 1.3 프로그래밍 언어에서의 추상화

추상화: 속성들의 일부분만을 가지고 주어진 작업이나 객체들을 필요한 정도로 묘사할 수 있는 방법을 지원하는 것

## 자료 추상화

- 기본적 추상화 (basic abstraction): 컴퓨터 내부의 자료 표현을 추상화

  `int x; float y;`

- 구조적 추상화 (structured abstract): 자료값의 집합을 추상화

  `type rarray = array[1..10] of real;`

- 단위 추상화(unit abstraction): 캡슐화

  Modula-2의 module, Ada의 package, Java의 class 등

## 제어 추상화

- 기본적 추상화: 몇 개의 기본 명령어를 모아 이해하기 쉬운 추상 구문으로 만든 것

  `x := x + y`

-  구조적 추상화: 프로그램에서 어떤 검사된 값에 따라 분할된 명령어의 그룹을 수행하도록 하는 것

  - if문, case문, switch문, 반복문
  - 프로시저 호출 (함수 호출)

- 단위 추상화: 프로시저의 집합을 추상화

  - 라이브러리, Modula-2의 module, Ada의 package, Java의 class 등
  - Java의 멀티스레드



# 1.4 계산 전형 (computational paradigms)

## 명령형 언어(imperative language) / 절차 언어(procedural language)

- C, C++, Ada, Pascal
- 폰노이만 병목형상 발생: 순차 실행 때문에
- 많은 자료의 동시 계산, 비결정적 계산, 순서에 의존하지 않는 계산 등에 비효율적

## 함수형 언어 (functional language) / 적용형 언어 (applicative language)

- LISP
- 함수의 평가(evaluation)와 함수 적용(application)을 기본으로 함

## 논리형 언어 (logical language) / 선언적 언어 (declarative language)

- 기호 논리학에 근거
- Prolog

## 객체 지향 언어 (object-oriented language)

- Java
- 객체는 클래스로 그룹화: 클래스 선언 + 클래스의 인스턴스



# 1.5 언어 정의

프로그래밍 언어의 정확한 형식 정의가 필요

- 언어 구문(syntax) 정의: 대부분 문맥 자유 문법(context free grammer)을 만족하며 BNF로 정의
- 언어 의미(semantics) 정의: 프로그래밍의 실행 시 어떤 일이 발생하는가를 서술



