# Device OOP Polymorphism Web App
자료구조 과제 2 제출용 웹앱입니다. 과제 1의 Python OOP 구조인 `DeviceADT -> Device -> AirConditioner / RobotVacuum`을 웹 화면에서 시각화하고, 각 클래스 노드를 클릭하면 오버라이딩된 `operate()` 메서드가 다른 결과를 출력하도록 구현했습니다.
## 실행 방법
1. `index.html`을 브라우저로 열면 바로 실행됩니다.
2. 왼쪽의 클래스 카드를 클릭합니다.
3. 오른쪽 `실행 결과` 영역에서 `operate()` 호출 결과를 확인합니다.
4. `다형성 전체 실행` 버튼을 누르면 `Device` 타입 배열 안의 서로 다른 하위 클래스 객체들이 같은 `operate()` 호출에 대해 서로 다른 결과를 출력합니다.
## 과제 1과의 연결
- `DeviceADT`: 추상 ADT 역할. `name`, `brand`, `introduce()`, `operate()`의 규칙을 정의합니다.
- `Device`: 공통 속성 `_name`, `_brand`와 공통 메서드 `introduce()`, 기본 `operate()`를 구현합니다.
- `AirConditioner`: `Device`를 상속하고 `operate()`를 에어컨 동작으로 오버라이딩합니다.
- `RobotVacuum`: `Device`를 상속하고 `operate()`를 로봇청소기 동작으로 오버라이딩합니다.
