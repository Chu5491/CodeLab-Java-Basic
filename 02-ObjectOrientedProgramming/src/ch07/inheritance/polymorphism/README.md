[Go Home](https://github.com/devJRL/CodeLab-JAVA-Basic#codelab-java-basic) / [Go Up](..)

# 다형성(polymorphism)

## [다형성이란?](./AnimalTest.java)

> 하나의 코드가 여러 자료형으로 구현되어 실행되는 것  
> 같은 코드에서 여러 실행결과가 나오는 것

> 정보은닉, 상속과 더불어 객체지향 프로그래밍의 가장 큰 특징 중 하나  
> 객체 지향 프로그래밍의 유연성, 재활용성, 유지보수성에 기본이 되는 특징

## 다형성을 활용하는 방법

> 여러가지 클래스를 묶어서 하나의 타입으로 관리하고자할 때 용이합니다.  
> 공통된 속성을 부모클래스에서 구현합니다.  

## [다운캐스팅(DownCasting)과 instanceof](./AnimalTest.java#L83)

> **다운캐스팅** : 묵시적으로 상위 클래스 형 변환된 인스턴스가  
> 원래 자료형(하위 클래스)으로 변환되어야 할 때 명시하는 형변환  
> 하위 클래스로의 형 변환은 명시적으로 되어야 함

```java
	Customer    vip1 = new VIPCustomer();  // 묵시적 형변환 (UpCasting)
	VIPCustomer vip2 = (VIPCustomer) vip1; // 명시적 형변환 (DownCasting)
```

> 그러나, 명시적 형변환만 사용하면 오류가 발생할 수 있습니다.  
> [instanceof 연산자](./AnimalTest.java#L96)를 사용해서 안전하게 타입을 체크하여 사용합니다.