# 자바, JVM, JDK 그리고 JRE

## JVM(Java Virtual Machine)

1. 특정 밴더가 구현한 구현체, **바이트 코드**를 실행할 수 있다.
2. 바이트 코드(.class 파일)를 OS에 특화된 코드로 변환(인터프리터 & JIT 컴파일러)하여 실행한다.

    ```shell
    $ java helloworld.java
    $ javap -c helloworld
    ```

3. 특정 플랫폼에 종속적이다.

## JRE(Java Runtime Environment)

1. JVM과 라이브러리를 제공한다.
2. 자바 애플리케이션을 **실행**할 수 있도록 구성된 배포판이다.
3. 자바 컴파일러는 들어있지 않다.

## JDK(Java Development Kit)

1. JRE와 개발에 필요한 툴을 제공한다.
2. 소스 코드를 작성할 때 사용하는 자바 언어는 플랫폼에 독립적이다. (JVM이 플랫폼에 종속적)
3. 오라클은 자바 11부터는 JDK만 제공한다.
4. 자바 9 부터는 제공되는 모듈로 커스텀 JRE를 만들 수 있다.

## 자바

1. 프로그래밍 언어이다.
2. JDK에 들어있는 자바 컴파일러(`javac`)를 사용해 바이트 코드로 컴파일할 수 있다.

## JVM 언어

1. 바이트 코드(.class 파일)나 자바 파일(.java 파일)을 만들 수 있는 언어라면 JVM으로 실행할 수 있다.
2. Kotlin, Scala, Jython..
