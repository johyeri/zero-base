Practice
===

문제 설명
---

개미가 새로운 지역을 탐험하려고 한다.  
탐험하려는 장소는 2 차원 행렬로 주어지는데, 2차원 행렬 안의 원소는 다음과 같다.
* 0은 미탐험 지역
* 1은 벽으로 인해 갈 수 없는 지역

개미의 처음 위치는 (r, c, d) 로 주어 지는데, 각각의 의미는 다음과 같다.  
* r: r 번 행 (인덱스 0부터 시작)
* c: c 번 행 (인덱스 0부터 시작)
* d: 개미가 바라보는 방향 (0: 북쪽, 1: 동쪽, 2: 남쪽, 3: 서쪽) 

또한, 개미의 탐험 방법은 다음과 같다.  
1. 현재 위치를 탐험
2. 현재 위치에서 인접한 왼쪽의 지역이 아직 미탐험 지역이면 왼쪽으로 회전하여 한칸 전진 후 1번 진행  
   미탐험 지역이 아니면 왼쪽 방향으로 회전만 진행
3. 2에서 1번을 진행하거나 후진하지 않고 2번을 연속하여 네 번 진행하는 경우,  
   한 칸 후진한다. 이 때, 뒤쪽이 벽이라면 탐험을 종료한다.

새로운 지역에 대한 정보 map 과 개미의 처음 위치 및 방향이 주어졌을 때,  
개미가 탐험 가능한 지역의 수를 출력하는 프로그램을 작성하세요.


입력 형식
---
map 의 행과 열 크기는 각각 3 ~ 100 사이의 자연수이다.    
map 의 원소는 0과 1로 이루어져 있으며, 외곽 지역은 모두 1로 이루어져 있다.

출력 형식
---
개미가 탐험한 지역의 수를 반환하세요.



입출력 예시
---
| map                                                                                                     | Result |
|---------------------------------------------------------------------------------------------------------|--------|
| {1, 1, 1, 1, 1} <br/> {1, 0, 0, 0, 1} <br/> {1, 0, 0, 0, 1} <br/> {1, 0, 0, 0, 1} <br/> {1, 1, 1, 1, 1} | 9      |
