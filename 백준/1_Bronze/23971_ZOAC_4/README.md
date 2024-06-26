# [23971. ZOAC 4](https://www.acmicpc.net/problem/23971)
### 문제
* 테이블이 행마다 w개씩 h행에 있고, 참가자는 세로로 n칸 또는 가로로 m칸 이상 앉아야 함
* 거리두기 수칙 지키면서 최대 몇 명 수용 가능한지 구하기

### 풀이 방법
* 자리에 앉고 앉지 못하는 지리를 표시 0-> 그 다음 자리에 앉고 못 앉는 자리 표시...
* (1+n) * (1+m) 사각형이 h*w에 최대 몇 개 들어갈 수 있는지 찾는 문제
* 나머지 이용? -> 나누어 떨어지면 X, 나누어 떨어지지 않으면 + 1 해서...
* m+1 이 w에 몇 개 까지 들어가는지 구하기 -> 나누어 떨어지면 + 0, 나누어 떨어지지 않으면 + 1
* 가로 = (w//(m+1))
* 세로 = (h//(n+1))
