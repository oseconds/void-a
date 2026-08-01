# 2023.06.09 Directional Speaker Mechanism

초지향성 스피커 방향 제어 방식 구체화

초지향성 스피커는 방향성이 강하기 때문에
관객 위치에 맞춰 스피커가 향하는 구조를 생각하고 있었음

기존에는 관객 방향을 향한다는 개념적인 구상만 있었음

이를 실제 구현 방식으로 구체화하면서
관객의 위치에 따라 거리와 높이가 달라질 경우
단순한 회전이 아니라 3차원 방향 제어가 필요하다고 판단

여러 개의 서보모터를 이용해 각 축의 회전값을 제어하는
3축 방향 제어 구조로 개발 방향 결정

참고

- Control Multiple Servomotors with TouchDesigner and Arduino | Steven Benton
https://stevenmbenton.com/control-multiple-servos-with-touchdesigner/

TouchDesigner에서 계산한 위치 데이터를 기반으로
Arduino를 통해 여러 서보모터를 제어하는 방식 탐색

관객 위치에 따라 초지향성 스피커의 방향을 조절하는
물리적 구조를 구체화