# Garbage Collection

Java에서는 프로그램 코드에서 메모리를 명시적으로 해제하지 않기 때문에 Garbage Collector가 더 이상 필요 없는 객체를 찾아 지우는 작업을 한다. 여기서 Garbage Collector는 다음의 **weak generational hypothesis**라는 가설에 기반해 동작한다.

1. 대부분 객체는 금방 접근 불가능 상태가 된다.
2. 오래된 객체에서 젊은 객체로의 참조는 아주 적게 존재한다.

## stop-the-world란

Garbage Collector를 실행하기 위해 JVM이 GC를 발생시키는 쓰레드 이외의 쓰레드를 모두 멈추고 GC 작업을 수행하는 것을 말한다. GC 작업이 끝난 후에 멈췄던 작업들이 다시 시작된다.

어떤 GC 알고리즘이라도 stop-the-world는 발생하기에 이 시간을 줄이는 것은 Garbage Collector를 튜닝하는 데에 중요한 요소가 될 수 있다.

---
[Java Garbage Collection - Naver D2](https://d2.naver.com/helloworld/1329)