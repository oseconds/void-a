# 2023.06.24 Kinect Based Direction Control

## Kinect 데이터 기반 방향 제어 방식 탐색

초지향성 스피커가 관객을 향하도록 만들기 위해
관객 위치 데이터와 회전 구조를 연결하는 방법 고민

이전에는 여러 개의 서보모터를 이용해
3차원 방향 제어를 하는 구조를 생각했는데
실제 구현을 위해 Kinect 좌표를 어떻게 회전값으로 변환할지 확인

Kinect Tracking 데이터를 기반으로
XY축 서보모터를 제어하는 사례 참고

참고

- Kinect Airsoft Turret
https://github.com/AllPartsCombined/Kinect-Airsoft-Turret

TouchDesigner에서 오브젝트의 방향을 제어할 때
Look At 기능을 원하는 축으로 제한하는 방법 탐색

참고

- How to limit a parameter "Look at" to only one axis?
https://forum.derivative.ca/t/how-to-limit-a-parameter-look-at-to-only-one-axis/9393

관객 위치 좌표를 기반으로
방향 벡터를 계산하고 이를 회전값으로 변환하는 구조 고민

시각적 오브젝트뿐 아니라
물리적인 스피커 방향도 관객 위치를 따라가는 방식으로 발전