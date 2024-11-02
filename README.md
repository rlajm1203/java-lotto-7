# java-lotto-precourse

## 기능 요구사항(간단 로또 발매기)
### 로또 발매
- 로또 번호 숫자 범위 1~45
- 1개의 로또 번호 발행 시, 중복되지 않는 6개의 숫자
- 로또 구입 금액을 입력하면 구입 금액에 해당하는 만큼 로또를 발행한다.
- 로또 1장의 가격은 1000원
- 당첨 번호와 보너스 번호를 입력 받는다.
- 사용자가 구매한 로또 번호와 당첨 번호를 비교하여 당첨 내역 및 수익률을 출력하고 로또 게임 종료

### 번호 추첨
- 중복되지 않는 숫자 6개 + 보너스 번호 1개
- 당첨은 1등 ~ 5등
  - 1등 : 6개 번호 일치
  - 2등 : 5개 번호 일치 + 보너스 번호 일치
  - 3등 : 5개 번호 일치
  - 4등 : 4개 번호 일치
  - 5등 : 3개 번호 일치
- 사용자가 잘못된 값을 입력한 경우 IllegalArgumentException을 발생
  - [ERROR] 로 시작하는 메세지 출력 후 그 부분부터 다시 입력 받는다.
  - Exception이 아닌, IllegalArgumentException, IllegalStateException 등과 같은 명확한 유형 처리

## 프로그래밍 요구사항
- 함수(또는 메소드)의 길이가 15라인을 넘어가지 않도록 구현한다.
  - 함수(또는 메소드)가 한 가지 일만 잘 하도록 구현한다.
- else 예약어를 쓰지 않는다.
  - else의 대용 switch/case도 쓰지 않는다.
  - 힌트 : if 조건절에서 return 하면 else를 쓰지 않아도 된다.
- Enum을 사용해서 구현한다.
- 구현한 기능에 대한 단위 테스트를 작성한다.
  - UI 로직에 대한 단위 테스트는 작성하지 않는다.