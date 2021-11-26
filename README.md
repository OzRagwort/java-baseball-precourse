# 미션 - 숫자 야구 게임

## 🏁 구현할 기능 목록

### 상대방(Computer)
- 1부터 9까지 서로 다른 수로 이루어진 3자리의 무작위 수 생성

### 사용자(User)
- 1부터 9까지 서로 다른 수로 이루어진 3자리의 수 입력
- 게임이 끝난 후 재시작/종료를 구분하는 1과 2 중 하나의 수 입력

### 판정 및 출력
- 메시지 출력
  - `숫자를 입력해주세요 : ` : 숫자 입력 대기 메시지
  - `3개의 숫자를 모두 맞히셨습니다! 게임 종료` : 3개의 숫자를 모두 맞힐 경우 메시지
  - `게임을 새로 시작하려면 1, 종료하려면 2를 입력하세요.` : 재시작/종료 입력 대기 메시지
- 볼 카운트 판정 및 출력
  - 같은 수가 같은 자리에 있으면 스트라이크
  - 같은 수가 다른 자리에 있으면 볼 
  - 같은 수가 전혀 없으면 포볼 또는 낫싱
  - 예시 : `1볼 1스트라이크`
- 재시작/종료 입력 판정
  - 1 : 게임을 처음부터 재시작
  - 2 : 프로그램 종료

### 유효성 검증
- 상대방(Computer)이 생성한 3자리의 무작위 수 검증
  - 3자리의 자연수 인지 확인
  - 1부터 9까지의 수로만 이루어져 있는지 확인
  - 중복된 수가 없는지 확인
  - 검증 실패 시 새로운 난수 생성을 위해 검증 결과를 리턴
    `VALID_SUCCESS`, `VALID_FAILED`
- 사용자가 입력한 3자리의 수 검증
  - 3자리의 자연수 인지 확인
  - 1부터 9까지의 수로만 이루어져 있는지 확인
  - 중복된 수가 없는지 확인
  - 검증 실패 시 `IllegalArgumentException`을 발생
- 사용자가 입력한 재시작/종료 입력 검증
  - 1 또는 2가 아닌 경우 `IllegalArgumentException`을 발생

<br>

---

## 📝 License

This project is [MIT](https://github.com/woowacourse/java-baseball-precourse/blob/master/LICENSE) licensed.
