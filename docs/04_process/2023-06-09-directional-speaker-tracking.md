# 2023.06.09 Directional Speaker Tracking

초지향성 스피커의 방향 제어 방식 고민

기존에는 초지향성 스피커를 특정 위치에 고정하는 방식을 생각했지만
관객과 작품의 관계를 더 명확하게 만들기 위해
스피커 자체가 관객 방향을 바라보는 구조를 고민

서로 응시하고 있는 관객에게만 소리가 전달되도록
스피커 방향을 실시간으로 제어하는 방식 탐색

TouchDesigner와 Arduino를 이용해
서보모터를 제어하는 방법 확인

참고

- Control Multiple Servomotors with TouchDesigner and Arduino | Steven Benton
https://stevenmbenton.com/control-multiple-servos-with-touchdesigner/

관객 위치 데이터를 기반으로
스피커의 방향을 회전시키는 구조 가능성 확인

시각적인 응시뿐 아니라
소리도 관객을 향하는 형태로 확장