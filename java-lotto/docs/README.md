[] 구매한 로또들이 입력될 Lottos 리스트를 전역 리스트로 선언해준다.

[] takeCost() 함수를 통해 구매 금액을 입력받는다.
   입력 받지 못했거나 또는 입력을 받았지만 숫자가 아닌 경우, 1000원으로 나누어 떨어지지 않는 경우는 모두 예외처리 한다.
   해당 예외 상화에 모두 포함되지 않는다면 구매 금액을 1000원으로 나누어 구매한 총 로또 수를 반환한다.

[] getLotto() 함수를 통해 1부터 45 사이의 수 6개를 랜덤으로 포함하는 리스트를 받는다.
   이때 Lotto 클래스로 숫자가 6개가 되지 않는 경우, 범위를 벗어난 경우 그리고 중복된 수가 있는 경우들을 예외처리
   예외처리가 되지 않고 요구하는 조건을 모두 맞췄다면, Lottos 리스트에 추가 후 출력한다.

[] 자료형이 Lotto인 answer을 createAnswer() 함수를 이용해 당첨 번호를 입력 받는다.
   입력 받은 당첨 번호가 null이 아니라면 ',' 기준으로 문자열을 쪼개 함수 내의 answer 리스트에 추가한다.
   answer 리스트에 겹치는 숫자가 있다면 예외 처리하고 출력 후 answer 리스트의 각 값들을 Integer로 변환해 temp에 추가한다.
   이후 Lotto 클래스로 temp반환

[] 당첨 번호 중 보너스 숫자는 createBonus() 함수로 입력 받는다.
   입력 받은 후 Integer로 변환해서 반환

[] winALottery() 함수를 이용해 Lottos 리스트에 있는 로또의 총 개수만큼 반복하며 Lotto class에 있는 compareLotto() 함수를 호출한다.
   이때 보너스 숫자까지를 포함해서 5개가 일치하면 5가 아닌 7을 반환한다.
   각 로또마다 몇 개씩 일치하는지 입력한 리스트를 반환한다.

[] winALottery() 함수에서 반환해준 winning 리스트를 이용해 Winning() 함수에서 1~5등 사이에 몇개나 당첨됐는지 확인한다.
   이때 1~5등 사이 조건이 맞다면 Enum 클래스에서 생성한 객체들의 각 count를 1씩 증가시켜준다.

[] printCount() 함수를 사용해 Enum 클래스로 생성한 객체들의 ment와 count를 차례로 출력해 결과값을 나타낸다.

[] rate() 함수를 이용해 등수에 맞는 상금과 각 등수의 count를 곱한다.
   수익률은 소수점 둘째 자리에서 반올림 해야하므로  총 합계에 10을 곱한 후 로또 구매 개수로 나눈다.
   main()에서 출력 시 소수점 이전 자리는 10으로 나눌 때 정수 부분으로 소수점 첫째 자리는 10으로 나눈 나머지를 출력한다.