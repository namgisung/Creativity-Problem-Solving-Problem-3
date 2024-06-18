# Creative-problem-solving-ideas

**최대구간합 문제임**

 * 코드 설명

사용한 알고리즘 dp(동적계획법): 큰일을 작은일로 쪼개고 그 중에서 반복되는 것이 있으면 그거를 처음에 실행할때 저장하고 그 다음에 반복되면 저장한 값을 쓰서 중복계산을 피하는 방식임

처음에 S의 위치를 찾고 1행에 있는 값을 또다른 2차원 리스트 1행에 저장한다.

1행에 있는 값(원래 리스트)과 이전 값(새로운 리스트)과 더한 값을 그 위치(새로운 리스트)에 저장한다

1열도 똑같이 한다

나머지 칸들은 그 위치(새로운 리스트)에서 행-1인 값과 본인 원래 갑(원래 리스트)을 더하고 열-1인 값(새로운 리스트)과 본인 원래 값(원래 리스트)을 더하여 비교한다
그 비교한 것중에서 큰것을 저장한다(새로운 리스트에)

그러고나서 새로운 리스트에 가장 오른쪽 아래쪽에 있는 값이 최대값이다.
