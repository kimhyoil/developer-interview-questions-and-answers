### OOP
* 객체지향 프로그래밍과 장점
  * 프로그래밍에서 필요한 데이터를 추상화시켜 상태와 행위를 가진 객체를 만들고 그 객체들 간의 유기적인 상호작용을 통해 로직을 구성하는 프로그래밍 방식으로 `추상화`가 쉽고 상속을 통해 코드 `재산성성`을 높일 수 있으며 객체 단위 코드가 나눠져 있기 때문에 `디버깅과 유지보수`에 용이
* 객체지향 프로그래밍의 특징
  * `추상화`: 필요한 정보만을 표현함으로써 공통의 속성이나 기능을 묶어 이름을 붙이는 것
  * `캡슐화`: 속성과 기능을 정의하는 멤버 변수와 메소드를 클래스라는 캡슐에 넣는 것
  * `상속`: 부모 클래스의 속성과 기능을 그대로 이어 받아 사용할 수 있게 하고 기능의 일부분을 변경해야 할 경우, 상속 받은 자식 클래스에서 해당 기능만 다시 수정(정의)하여 사용할 수 있게 하는 것
  * `다형성`: 하나의 변수명, 함수명 등이 상황에 따라서 다른 의미로 해석될 수 있는 것
* 다형성의 구체 사례
  * 부모 타입으로 자식 객체를 참조하여 부모 타입에 대한 메소드들을 쓸 수 있음
  * 부모 타입으로 자식 타입의 객체를 참조할 때는 묵시적으로 형변환, 부모 타입의 객체를 자식 타입으로 참조하게 할때는 명시적으로 형변환할 수 있고 그 객체가 원래 자식 객체였는지 부모 객체였는지에 따라 사용 가능한 필드나 메소드가 정해짐
* 객체지향 설계의 5원칙
  * `SRP(Single Responsibility Principle)`: 단일 책임 원칙, 클래스는 단 하나의 책임을 가져야 하며 클래스를 변경하는 이유는 단 하나의 이유이어야 한다.
  * `OCP(Open-Closed Principle)`: 개방-폐쇄 원칙, 확장에는 열려 있어야 하고 변경에는 닫혀 있어야 한다.
  * `LSP(Liskov Substitution Principle)`: 리스코프 치환 원칙, 상위 타입의 객체를 하위 타입의 객체로 치환해도 상위 타입을 사용하는 프로그램은 정상적으로 동작해야 한다.
  * `ISP(Interface Segregation Principle)`: 인터페이스 분리 원칙, 인터페이스는 그 인터페이스를 사용하는 클라이언트를 기준으로 분리해야 한다.
  * `DIP(Dependency Inversion Principle)`: 의존 역전 원칙, 고수준 모듈은 저수준 모듈의 구현에 의존해서는 안된다.
* 클래스와 인스턴스의 차이
  * 클래스는 객체를 만들기 위한 템플릿, 객체는 클래스라는 템플릿을 토대로 `메모리에 할당한 실체`
* Immutable
  * 생성 후 변경 불가한 객체로 변경을 하려면 복사 이후 변경해야함
* Call by Value vs Call by Reference
  * Call by Value와 Call by Reference는 `값을 복사를 하여 처리를 하느냐, 아니면 직접 참조를 하느냐 차이`로 Call by value는 인자로 받은 값을 복사하여 처리하고 Call by reference는 인자로 받은 값의 주소를 참조하여 직접 값에 영향을 줌
* 디자인 패턴
  * 소프트웨어 코드 작성 시에 생기는 `공통적인 문제를 해결하는데 도움이 되는 코드 패턴`
* 디자인 패턴 중 싱글톤 패턴
  * 전체 프로그램에서 단 1개의 객체를 생생하고 공유하는 코드 패턴으로 한번의 객체 생성으로 재사용이 가능하기 때문에 메모리 낭비를 방지하고 객체가 전역성을 띄기 때문에 공유가 용이
* 디자인 패턴 중 MVC 패턴
  * Model, View, Controller라고 하는 컴포넌트로 분리하여 `비지니스 처리 로직`과 사용자 `인터페이스 요소`를 분리시켜 서로 영향없이 개발하기 수월
* 디자인 패턴 중 팩터리 패턴
  * 팩토리 패턴은 클래스의 `인스턴스를 만드는 것을 서브클래스에서 결정하는 패턴`으로 팩토리 메서드 패턴과 추상 팩토리 패턴으로 구체화됨
  * 팩토리 메서드 패턴: 객체를 생성하기 위한 인터페이스를 정의하는데, 어떤 클래스의 인스턴스를 만들지는 서브클래스에서 결정
  * 추상 팩토리 패턴: 인터페이스를 이용하여 서로 연관된, 또는 의존하는 객체를 구상 클래스를 지정하지 않고도 생성
* MVC 패턴을 강화시키는 방법
  * 
  