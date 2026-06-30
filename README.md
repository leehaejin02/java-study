# Java Study

자바 학습 기록 저장소

## 목차

* 1일차 (개발환경 구축 및 학습 계획 수립)
* 2일차 (Todo 프로그램 구현 및 반복문 학습)
* 3일차 (클래스, 객체, 생성자, this 키워드 학습)
* 4일차 (toString(), List, 객체지향 방식 학습)
* 5일차 (D1~D4 복습 및 객체지향 기초 예습)
* 6일차 (D1~D5 복습 및 Todo 프로그램 직접 구현)
    
---

# 1일차 (2026-06-23)

## 오늘 한 일

* JDK 21 설치
* IntelliJ IDEA Community 설치
* Git 설치
* GitHub Repository(java-study) 생성
* JDK, IntelliJ, Git의 역할과 관계 학습
* Java 컴파일 및 실행 과정 학습
* 향후 LLM 활용 방향 및 학습 목표 정리

## 배운 점

### JDK (Java Development Kit)

* Java 프로그램을 개발하고 실행하기 위한 도구 모음
* javac(컴파일러), JVM(Java Virtual Machine), java 실행 명령어 등을 포함
* Java 코드를 컴파일하고 실행하는 역할 수행

### IntelliJ IDEA

* Java 코드를 작성하고 실행할 수 있는 IDE(통합 개발 환경)
* 자동완성, 디버깅, 프로젝트 관리 기능 제공
* 내부적으로 JDK를 사용하여 컴파일 및 실행 수행

### Git

* 소스코드 변경 이력을 관리하는 버전 관리 도구
* 코드 수정 내역을 저장하고 이전 버전으로 복구 가능
* GitHub와 연동하여 온라인으로 프로젝트 관리 가능

### Java 실행 과정

* Java 코드를 작성한다. (.java)
* javac가 Java 코드를 Bytecode(.class)로 컴파일한다.
* JVM이 .class 파일을 읽어 실행한다.
* JVM이 운영체제에 맞는 기계어로 변환하여 CPU가 실행한다.
* JVM 덕분에 하나의 Java 프로그램을 다양한 운영체제에서 실행할 수 있다.

### 개발환경 구성 요소 관계

* IntelliJ → 코드 작성
* JDK → 컴파일 및 실행
* Git → 버전 관리
* GitHub → 온라인 저장 및 공유

### 목표

* Java 기초 체력 향상
* 객체지향 프로그래밍 이해
* 스스로 프로젝트 구현 가능 수준 도달
* 폐쇄망 환경에서도 개발 가능한 역량 확보
* LLM을 보조 도구로 활용하는 개발 습관 형성

## 느낀 점

* 개발환경 구축을 완료하여 Java 학습을 시작할 준비를 마쳤다.
* 지금까지는 LLM 의존도가 높았지만 앞으로는 스스로 구현하는 비중을 늘릴 계획이다.
* 2개월 동안 Java 기초 역량을 집중적으로 학습하여 혼자서도 개발할 수 있는 수준을 목표로 한다.

---

# 2일차 (2026-06-24)

## 오늘 한 일

* IntelliJ IDEA에서 Java 프로젝트 생성
* 문자열 배열을 이용한 Todo 프로그램 구현
* split()을 사용하여 상태(todo, done)와 할 일을 분리
* Scanner를 이용한 사용자 입력 처리
* ArrayList를 이용한 데이터 저장
* while문을 이용한 반복 입력 기능 구현
* 숫자 5 입력 시 프로그램 종료 기능 구현

## 배운 점

### 문자열 처리

* split()을 사용하여 문자열을 원하는 기준으로 분리할 수 있다.
* 문자열을 분리한 후 상태값과 할 일을 각각 처리할 수 있다.

### ArrayList

* 데이터를 동적으로 저장할 수 있다.
* add(), get(), size() 메서드를 사용하여 데이터를 관리할 수 있다.

### 반복문

* while문을 사용하여 프로그램을 반복 실행할 수 있다.
* 종료 조건에 따라 반복을 제어할 수 있다.

### Return Type

* 메서드의 기능뿐만 아니라 반환 타입(Return Type)도 함께 이해해야 한다.
* 반환 타입에 따라 변수 저장, 출력, 조건문 사용 여부가 달라진다.

예시

```java
split()      -> String[]
startsWith() -> boolean
substring()  -> String
next()       -> String
size()       -> int
```

## 멘토 피드백

* 메서드의 기능뿐 아니라 Return Type까지 정확히 이해해야 한다.
* while(true) 보다는 while(조건식) 형태로 종료 조건을 명확하게 작성해야 한다.

## 느낀 점

* 사용자 입력을 받아 데이터를 저장하고 출력하는 프로그램을 직접 구현할 수 있었다.
* ArrayList와 Scanner의 기본 사용법을 익힐 수 있었다.
* 반복문의 종료 조건을 명확하게 작성하는 습관이 중요하다는 것을 배웠다.
* 앞으로는 메서드의 기능뿐 아니라 반환 타입까지 함께 확인하며 학습할 예정이다.

---

# 3일차 (2026-06-25)

## 오늘 한 일

* 이슈(Issue) 데이터를 변수로 관리하는 방식 실습
* 이슈 개수가 증가할 때 발생하는 문제점 분석
* 클래스(Class) 생성 및 활용
* 객체(Object) 생성 실습
* 생성자(Constructor) 개념 학습
* this 키워드 개념 학습
* 메서드(Method)를 이용한 데이터 출력 기능 구현

## 배운 점

### 클래스(Class)

* 클래스는 객체를 생성하기 위한 설계도이다.
* 관련된 데이터와 기능을 하나로 묶어 관리할 수 있다.
* 같은 형태의 데이터를 반복적으로 관리할 때 사용한다.

예시

```java
class Issue {
    int id;
    String title;
    String status;
}
```

### 객체(Object)

* 객체는 클래스를 기반으로 생성된 실제 데이터이다.
* 하나의 클래스로 여러 개의 객체를 생성할 수 있다.

예시

```java
Issue issue1 = new Issue(...);
Issue issue2 = new Issue(...);
Issue issue3 = new Issue(...);
```

### 생성자(Constructor)

* 객체가 생성될 때 자동으로 실행된다.
* 객체의 필드에 초기값을 설정하는 역할을 한다.

예시

```java
Issue(int id, String title, String status) {
    this.id = id;
    this.title = title;
    this.status = status;
}
```

### this 키워드

* 현재 객체 자기 자신을 가리킨다.
* 필드명과 매개변수명이 같을 때 구분하기 위해 사용한다.

예시

```java
this.id = id;
```

* 왼쪽 this.id → 객체의 필드
* 오른쪽 id → 생성자의 매개변수

### 메서드(Method)

* 객체가 수행할 수 있는 기능을 정의한다.
* 동일한 기능을 여러 번 사용할 수 있도록 재사용성을 높여준다.

예시

```java
public void printScore() {
    System.out.println("id= " + id);
    System.out.println("title= " + title);
    System.out.println("status= " + status);
}
```

## 멘토 피드백

* 변수만 사용하면 데이터가 증가할수록 관리가 어려워진다.
* 관련된 데이터를 하나의 클래스로 묶어서 관리하는 것이 중요하다.
* 객체 생성 과정과 생성자의 역할을 정확히 이해해야 한다.
* this 키워드가 필드와 매개변수를 구분하는 이유를 이해해야 한다.

## 느낀 점

* 처음에는 클래스와 객체의 차이가 헷갈렸지만, 설계도와 실제 객체의 관계로 이해할 수 있었다.
* 생성자는 객체 생성 시 초기값을 설정하는 역할이라는 것을 알게 되었다.
* this.id = id 코드의 의미를 이해하면서 필드와 매개변수의 차이를 구분할 수 있게 되었다.
* 변수만 사용하는 방식보다 클래스를 사용하는 방식이 데이터 관리에 훨씬 유리하다는 것을 느꼈다.

---

# 4일차 (2026-06-26)

## 오늘 한 일

* `toString()` 메서드와 오버라이드(Override) 학습
* `List<Issue>`를 이용한 여러 객체 관리
* 일반 `for`문과 향상된 `for`문으로 객체 출력
* `Issue` 클래스에 `start()` 메서드 구현
* 객체가 자신의 데이터를 표현하고 상태를 관리하는 객체지향 방식 학습

## 오늘 미션

### 미션 1. Issue 출력해보기

목표

* `Issue` 객체를 원하는 형식으로 출력하기
* Main에서 출력 형식을 직접 만드는 것이 아니라 `Issue` 클래스의 `toString()`을 활용하기

학습한 내용

* `toString()` 오버라이드
* `@Override`
* `System.out.println(issue)` 호출 시 `toString()` 자동 실행
* 객체가 자신의 정보를 문자열로 표현하도록 구현

---

### 미션 2. 이슈 여러 개를 List에 담기

목표

* 여러 개의 `Issue` 객체를 `List<Issue>`에 저장하기
* 반복문으로 모든 이슈 출력하기

학습한 내용

* `List<Issue>` 사용
* `add()`, `get()`, `size()` 메서드
* Java 21의 `getFirst()` 메서드
* 일반 `for`문과 향상된 `for`문 사용

---

### 미션 3. 상태 변경해보기

목표

* `issue.start();`를 호출하면 상태가 변경되도록 구현하기

학습한 내용

* `Issue` 클래스에 `start()` 메서드 구현
* Main에서 `status`를 직접 변경하지 않고 `issue.start()` 호출
* 객체가 자신의 상태를 직접 관리하는 방식 이해

## 배운 점

### toString()

* `toString()`은 객체의 정보를 문자열(String)로 반환하는 메서드이다.
* `System.out.println(issue);`를 호출하면 `toString()`이 자동으로 실행된다.
* `toString()`을 오버라이드하지 않으면 기본적으로 `클래스명@해시값` 형식으로 출력된다.

예시

```java
@Override
public String toString() {
    return "[" + id + "] " + status + " - " + title;
}
```

### 오버라이드(Override)

* 부모 클래스의 메서드를 자식 클래스에서 다시 정의하는 것을 오버라이드라고 한다.
* `Issue` 클래스에서는 `Object` 클래스의 `toString()` 메서드를 오버라이드하여 원하는 출력 형식을 만들었다.

### List

* `List`는 여러 개의 객체를 저장할 수 있는 컬렉션이다.
* `List<Issue>`의 `Issue`는 리스트에 저장할 객체의 자료형을 의미한다.
* `add()`로 객체를 추가하고 `get()`으로 원하는 객체를 가져올 수 있다.
* `size()`는 저장된 객체의 개수를 반환한다.
* Java 21부터는 `getFirst()`를 이용하여 첫 번째 요소를 가져올 수 있다.

### 일반 for문과 향상된 for문

일반 `for`문

```java
for (int i = 0; i < issues.size(); i++) {
    System.out.println(issues.get(i).title);
}
```

향상된 `for`문

```java
for (Issue issue : issues) {
    System.out.println(issue.title);
}
```

* 일반 `for`문은 인덱스를 사용할 수 있다.
* 향상된 `for`문은 객체를 하나씩 꺼내 사용할 때 간결하게 작성할 수 있다.
* `Issue`는 자료형이고 `issue`는 반복마다 하나의 객체를 저장하는 변수이다.

### 객체지향 방식

직접 변경

```java
issue.status = "IN_PROGRESS";
```

메서드 호출

```java
issue.start();
```

* Main에서 데이터를 직접 변경하면 객체의 내부 데이터를 외부에서 수정하게 된다.
* `issue.start()`를 호출하면 Main은 작업 시작만 요청하고 실제 상태 변경은 `Issue` 객체가 수행한다.
* 상태 변경 규칙이 바뀌더라도 `Issue` 클래스의 `start()` 메서드만 수정하면 되므로 유지보수가 쉬워진다.
* 객체가 자신의 데이터와 기능을 함께 관리하는 것이 객체지향 프로그래밍의 기본적인 설계 방식이다.

## 느낀 점

* 오늘 학습을 통해 `toString()`은 단순히 문자열을 반환하는 메서드가 아니라 객체가 자신의 정보를 표현하는 역할이라는 것을 이해하였다.
* `List<Issue>`를 사용하여 여러 개의 객체를 관리하고 반복문으로 순회하는 방법을 익힐 수 있었다.
* `status`를 Main에서 직접 변경하는 것이 아니라 `Issue` 객체의 `start()` 메서드를 호출하여 상태를 변경하면서 객체가 자신의 데이터를 직접 관리하는 객체지향적인 설계 방식을 이해하게 되었다.
* 문법을 익히는 것뿐만 아니라 "객체에게 일을 시킨다."는 객체지향적인 사고방식을 배우는 시간이었다.

---

# 5일차 (2026-06-29)

## 오늘 한 일

* D1~D4 학습 내용 복습
* Java 개발 환경(JDK, JRE, JVM, IntelliJ, Git) 개념 복습
* Todo 프로그램을 처음부터 다시 구현하며 복습
* `Array`와 `ArrayList`, `List`의 차이 학습
* `List<Todo>`를 활용한 객체 저장 및 관리 복습
* 클래스(Class), 객체(Object), 생성자(Constructor), `this` 키워드 개념 복습
* `toString()` 메서드와 객체 출력 방식 복습
* `private`, Getter, Setter의 필요성 예습

## 배운 점

### Java 실행 과정 복습

* `javac`는 Java 소스코드를 Bytecode(`.class`)로 컴파일한다.
* JVM이 Bytecode를 운영체제에 맞게 실행한다.
* `new` 키워드는 객체를 생성할 때 사용한다.

예시

```java
Todo todo = new Todo(1, "자바공부", false);
```

---

### 배열(Array)과 리스트(List)

배열

```java
String[] arr = new String[10];
```

* 크기가 고정된다.
* `arr.length`로 크기를 확인한다.

리스트

```java
List<String> list = new ArrayList<>();
```

* 크기가 자동으로 증가한다.
* `add()`, `get()`, `remove()`, `size()` 등의 메서드를 사용할 수 있다.

객체 저장

```java
List<Todo> todos = new ArrayList<>();
```

* 문자열이 아닌 `Todo` 객체를 저장할 수 있다.

---

### 클래스와 객체

* 클래스는 객체를 만들기 위한 설계도이다.
* `new`를 사용하면 클래스를 기반으로 객체가 생성된다.
* 하나의 클래스로 여러 개의 객체를 생성할 수 있다.

예시

```java
Todo todo1 = new Todo(1, "자바공부", false);
Todo todo2 = new Todo(2, "운동", false);
```

---

### 생성자와 this

* 생성자는 객체 생성 시 자동으로 실행된다.
* 객체의 필드를 초기화하는 역할을 한다.
* `this`는 현재 객체 자신의 필드를 의미한다.

예시

```java
Todo(int id, String title, boolean done) {
    this.id = id;
    this.title = title;
    this.done = done;
}
```

---

### List와 객체

* `List<Todo>`에는 문자열이 아니라 `Todo` 객체가 저장된다.
* `add()`로 객체를 저장하고 반복문으로 객체를 순회할 수 있다.

예시

```java
for (Todo todo : todos) {
    System.out.println(todo);
}
```

---

### toString()

* `System.out.println(todo)`를 호출하면 내부적으로 `todo.toString()`이 실행된다.
* `toString()`을 오버라이드하면 객체를 원하는 형식으로 출력할 수 있다.

예시

```java
@Override
public String toString() {
    return id + " | " + title + " | " + done;
}
```

---

### 접근 제어자와 Getter/Setter (예습)

* `private`을 사용하면 외부에서 필드에 직접 접근할 수 없다.
* Getter는 값을 읽기 위한 메서드이다.
* Setter는 값을 변경하기 위한 메서드이다.
* 읽기만 허용하고 싶은 경우 Getter만 만들고 Setter는 만들지 않을 수도 있다.

예시

```java
private int id;

public int getId() {
    return id;
}
```

## 느낀 점

* D1~D4 내용을 처음부터 다시 구현하면서 잊어버렸던 내용을 하나씩 떠올릴 수 있었다.
* 처음에는 클래스와 객체가 헷갈렸지만, 설계도와 실제 객체의 관계를 다시 정리하면서 이해가 더욱 명확해졌다.
* `List<Todo>`가 문자열이 아니라 객체를 저장한다는 개념과 `new`를 통한 객체 생성 과정을 연결해서 이해할 수 있었다.
* `toString()`이 객체를 문자열로 표현하는 역할이라는 점을 다시 확인했고, 앞으로 배울 `private`, Getter, Setter가 객체지향 설계에서 왜 필요한지도 미리 이해할 수 있었다.

---

# 6일차 (2026-06-30)

## 오늘 한 일

* D1~D5 학습 내용 복습
* 클래스(Class), 객체(Object), 생성자(Constructor), `this` 개념 설명 연습
* `Todo` 클래스 직접 구현
* `toString()` 오버라이드 복습
* `List<Todo>`를 이용한 객체 관리 복습
* `Scanner`를 이용한 메뉴 선택 기능 구현
* Todo 등록 기능 구현
* Todo 목록 조회 기능 구현
* Todo 삭제 기능 구현
* 일반 `for`문과 향상된 `for`문의 사용 목적 비교
* 사용자 입력 번호와 리스트 인덱스의 차이 학습

## 배운 점

### Todo 클래스 구현

* `Todo` 클래스를 직접 작성하며 필드, 생성자, `toString()`을 구현하였다.
* 생성자는 객체 생성 시 필드를 초기화하는 역할을 한다.
* `this`를 사용하여 필드와 매개변수를 구분하였다.

예시

```java
public class Todo {

    String title;
    boolean done;

    Todo(String title, boolean done) {
        this.title = title;
        this.done = done;
    }

    @Override
    public String toString() {
        return title + " : " + done;
    }
}
```

---

### List를 이용한 객체 관리

* `List<Todo>`를 생성하여 여러 개의 Todo 객체를 저장하였다.
* `add()`를 이용해 객체를 추가하고 반복문으로 목록을 출력하였다.

예시

```java
List<Todo> todos = new ArrayList<>();

todos.add(new Todo("자바공부", false));
```

---

### Scanner를 이용한 메뉴 구현

* `while`문을 이용하여 프로그램이 종료될 때까지 반복하도록 구현하였다.
* `Scanner`로 사용자의 메뉴 선택을 입력받아 기능을 분기하였다.

예시

```java
while (true) {

    System.out.println("""
            1. 등록
            2. 목록
            3. 삭제
            4. 종료
            """);

    int menu = scanner.nextInt();

    ...
}
```

---

### 일반 for문과 향상된 for문

향상된 `for`문

```java
for (Todo todo : todos) {
    System.out.println(todo);
}
```

* 객체를 하나씩 순회할 때 코드가 간결하다.
* 인덱스를 사용할 수 없다.

일반 `for`문

```java
for (int i = 0; i < todos.size(); i++) {
    System.out.println((i + 1) + ". " + todos.get(i));
}
```

* 인덱스를 사용할 수 있다.
* 번호 출력, 수정, 삭제 기능 구현에 적합하다.

---

### 리스트 인덱스와 사용자 번호

* 리스트의 인덱스는 0부터 시작한다.
* 사용자에게는 1번부터 보여주는 것이 자연스럽다.
* 따라서 사용자 입력 번호를 리스트 인덱스로 변환해야 한다.

예시

```java
int num = scanner.nextInt();
todos.remove(num - 1);
```

---

### 객체 출력과 `toString()`

* `System.out.println(todo)`를 호출하면 내부적으로 `toString()`이 실행된다.
* 객체의 출력 형식은 `toString()`에서 관리하는 것이 객체지향적인 방식이다.

예시

```java
System.out.println(todo);
```

## 느낀 점

* 멘토의 도움 없이 Todo 프로그램을 처음부터 다시 구현하면서 지금까지 배운 내용을 스스로 떠올리는 연습을 할 수 있었다.
* 단순히 문법을 암기하는 것보다 객체를 생성하고 `List`에 저장하며 프로그램을 직접 구현하는 과정에서 개념이 더욱 명확해졌다.
* 일반 `for`문과 향상된 `for`문의 차이를 실제 기능 구현에 적용해 보면서 각각의 사용 목적을 이해할 수 있었다.
* 삭제 기능을 구현하는 과정에서 사용자에게 보여주는 번호와 리스트의 인덱스가 다르다는 점을 직접 경험하며 인덱스 개념을 확실히 익힐 수 있었다.
* 앞으로도 정답을 바로 확인하기보다 먼저 스스로 구현하고 고민한 뒤 부족한 부분을 보완하는 방식으로 학습을 이어가고 싶다.

---


