# Project Timeline

`void-a / 보이다`의 2023년 작업 흐름 정리

이 문서는 날짜별 process log를 대체하기 위한 문서가 아니라
초기 개념 탐색부터 실제 전시까지 작업이 어떤 방향으로 변화했는지 빠르게 확인하기 위한 상위 timeline

세부 실험과 당시 판단은 각 날짜별 기록에 그대로 보존

---

## March 2023 — Initial Research

### 2023-03-16 — Early Philosophy Exploration

시선과 존재에 대한 작업 방향을 잡기 위해 여러 철학적 개념 조사

* Sartre의 타자의 시선과 대상화
* Heidegger의 존재와 현존재
* Spinoza의 conatus
* Augustine / Aristotle의 시간과 현재
* 이후 Lacan의 gaze와 `objet petit a` 쪽으로 관심이 이동

이 단계에서는 하나의 이론을 작품에 적용하기보다
내가 생각하고 있던 보는 것 / 보여지는 것 / 존재의 관계를 설명할 수 있는 언어 탐색

초기 연구 전체가 최종 작품의 이론으로 남은 것은 아님

### 2023-03-20 — Gaze as Objet a

Notion에서 `상호지향적 응시 (Gaze as Objet a)` 정리

르네상스 원근법과 고정된 관찰자
Lacan의 Look / Gaze
타자의 시선
objet petit a
보는 주체가 다시 보여지는 대상으로 놓이는 관계 등을 집중적으로 조사

이 시기의 개념 연구가 이후 `void-a`라는 이름과 작품의 gaze 구조에 직접 연결

### 2023-03-21 — Initial Proposal

초기 기획안 작성

당시에는 gaze 외에도

* simulacra
* mirror stage
* digital solidification
* 관객의 순간과 좌표를 가상 공간에 남기는 방식

등 여러 아이디어가 동시에 들어가 있었음

`0th axis`를 가상 작업 공간과 실제 전시 공간을 연결하는 축으로 설정

관객의 위치를 추적하고
그 시점에 맞는 가상 오브젝트를 실제 display 안에 존재하는 것처럼 보여주는 방향도 이때부터 등장

`digital solidification`은 이후 `다음 작업으로` 분리

### 2023-03-25 — Perception and Spatial Illusion Research

철학적인 개념을 실제 공간 경험으로 옮길 방법 탐색

AR painting
phenomenology
anamorphic space
object-seeing 관련 논문 조사

TouchDesigner의 Sweet Spot Previz와 MUTEK workshop 자료도 확인

이 시기부터

gaze
→ viewpoint
→ anamorphosis
→ real-time trompe-l'œil

이라는 기술적 연결이 생기기 시작

아직 처음부터 sweet spot을 작품의 눈으로 생각했던 것은 아님

anamorphic / viewpoint-dependent system을 조사하다가
나중에 고정된 관찰점을 작품의 시선으로 뒤집어 해석하게 됨

### 2023-03-26 — Parametric Speaker Feasibility

초지향성 스피커 DIY 사례와 회로 조사

초지향성 스피커 자체는 이전부터 작품 요소로 생각하고 있었고
이날은 실제로 직접 제작할 수 있는지 확인하는 단계

몇 가지 DIY 프로젝트와 회로를 확인한 뒤
직접 제작해볼 수 있겠다고 판단

음향 방향은 이후 moving sweet spot에서 파생된 것이 아니라
시각 시스템과 처음부터 병렬로 진행한 별도의 gaze 실험

---

## April 2023 — From Concept to Prototype

### 2023-04-04 — Kinect Tracking Research

관객의 실제 위치를 얻는 방법 구체화

Kinect의 인식 거리와 depth tracking 조사

초기에는 Unity + HTC Vive tracking도 검토했지만
HMD를 사용하는 VR 작품을 만들기 위한 것은 아니었음

tracker를 관객이 직접 들거나 부착하는 방식보다
관객에게 tracking interface가 드러나지 않는 구조가 작품 경험에 더 적합하다고 판단

Kinect + TouchDesigner 방향으로 이동

### 2023-04-07 — Main Object Previz

작품 안에서 관객을 바라보는 존재의 형태 탐색

눈은 단순히 gaze를 설명하는 상징보다
작품 자체가 하나의 생명체 / 주체처럼 느껴지도록 만드는 요소로 보는 쪽이 더 중요했음

Midjourney로

* cube display
* sphere-like object
* eye / creature 형태

등을 빠르게 시각화

2023년 당시 생성형 이미지를 최종 결과물보다
형태와 분위기를 빠르게 확인하는 previz 도구로 활용

### 2023-04-18 — Form and Symbol Exploration

눈이라는 형태가 너무 직접적인지 다시 고민

현실적인 eyeball이나 surveillance 이미지로 고정되지 않으면서도
관객이 하나의 존재와 시선을 인식할 수 있는 방법 탐색

입자들이 모인 구
간접적인 눈의 기호
파레이돌리아처럼 관객이 스스로 얼굴이나 시선을 발견하는 방식 등을 생각

눈을 제거하는 방향이라기보다
눈을 얼마나 직접적으로 보여줄지 조정하는 과정

### 2023-04-22 — TouchDesigner Trompe-l'œil Test

TouchDesigner에서 viewpoint-dependent trompe-l'œil 구현 시작

virtual camera 위치가 바뀌면
실제 display에서 보이는 perspective도 함께 변하도록 구성

anamorphic system의 fixed sweet spot을
움직이는 viewpoint로 바꾸는 핵심 시각 구조 테스트

### 2023-04-26 — Workstation Setup

실시간 그래픽과 이후 VRAM을 많이 사용하는 작업을 고려해 workstation 구성

* Intel i5-13600KF
* RTX 3060 12GB × 2
* RAM 64GB
* NVMe 2TB

RTX 3060은 당시 VRAM 대비 비용을 고려한 선택

### 2023-04-27 — Viewpoint Prototype

TouchDesigner prototype에서
virtual camera position에 따른 perspective 변화 확인

이 시점에는 실제 관객 tracking까지 완성된 것은 아님

먼저

`virtual camera position → viewpoint-dependent projection`

부분이 실제 display에서 성립하는지 테스트

관객 위치를 자동으로 얻어 camera에 연결하는 부분은 이후 작업으로 남음

`.toe` prototype 파일 보존

### 2023-04-28 — Mid Presentation

중간 발표

이전 작업 `if you gaze`, `Panopticon`과 연결해
계속 다뤄온 시선의 문제를 설명

Lacan의 Look / Gaze
anamorphosis
주체와 타자의 시선 등을 비교적 직접적으로 사용

당시 visual prototype은 구현되어 있었지만
실제 viewer position tracking은 아직 완전히 연결되지 않은 상태

이후에는 철학적 설명을 그대로 전면에 두기보다
관객이 실제로 무엇을 느끼는가에 집중하는 쪽으로 작품 설명이 이동

---

## May 2023 — Simplifying the Experience

### 2023-05-08 — Directional Sound Research

초지향성 스피커와 별개로
공간에서 소리의 방향성을 만드는 여러 방법 조사

Rear Delay Array / Back-to-Back 방식과
delay를 이용한 후방 cancellation 등의 원리 확인

최종 구현 여부와 별개로 directional sound를 이해하기 위한 연구 과정

### 2023-05-12 — Gaze Concept Revision

중간 발표 이후 작품의 설명 방식을 다시 정리

철학적 개념을 직접적으로 많이 보여주는 방식보다

관객이 먼저 작품에 모습을 보여주고
작품의 시선을 다시 경험하는 관계

쪽으로 단순화

Lacan의 이론을 버린 것은 아니지만
관객이 이론을 이해해야만 작품이 성립하는 구조에서는 벗어나려 함

---

## June 2023 — Building the System

### 2023-06-06 — Max/MSP Feedback Network

실시간으로 계속 변화하는 sound system 연구

Max/MSP Feedback Network 참고

미리 완성된 audio track을 재생하기보다
작품 상태에 따라 계속 변화하는 generative sound 가능성 탐색

최종 전시에서 어느 범위까지 적용되었는지는 별도 implementation boundary에서 구분 필요

### 2023-06-09 — Directional Speaker Mechanism

초지향성 스피커가 관객 방향을 실제로 향하도록 만드는 방법 구체화

이전부터 방향성을 가진 스피커를 생각하고 있었지만
이날부터 viewer position을 기준으로 실제 기계적 방향을 계산하는 구조 조사

TouchDesigner → microcontroller → multiple servo 방향 제어 참고

단순한 좌우 회전보다
관객의 높이 / 거리 / 공간상의 위치까지 대응할 수 있는 다축 구조를 생각

실제 최종 deployment 범위는 별도 확인 필요

### 2023-06-09 — Parametric Speaker Prototype

초지향성 스피커 실제 제작 시작

* ultrasonic transducer array
* 555 관련 회로
* driver
* 전원부
* STM32 등

여러 구성을 사용하며 초기 prototype 제작

이후 실제 회로는 테스트를 거치며 계속 변경

### 2023-06-13 — Parametric Speaker Assembly

초음파 transducer array와 회로 제작 계속

perfboard 납땜
전원 회로
driver
transducer array 등을 실제 hardware로 조립

이 단계의 부품 구성이 최종 전시 구성과 완전히 동일한 것은 아님

### 2023-06-15 — Pareidolia and Exhibition Narrative

작품의 출발점을 관객에게 어떻게 설명할지 고민

실제 생각의 배경에는
파레이돌리아와 시선에 대한 지각 경험이 있었음

하지만 이를 그대로 설명하기보다

책상 위 이어폰이 한번 얼굴처럼 보이기 시작한 뒤
계속 자신을 바라보는 것처럼 느껴졌다는 일상적인 이야기로 번역

이 일화는 실제 최초 사건을 그대로 기록한 것이라기보다
파레이돌리아와 보이지 않는 시선의 감각을 관객에게 전달하기 위해 만든 exhibition narrative

### June 2023 — Final Presentation

정확한 날짜 확인 필요

최종 발표에서는 작품의 핵심 질문이 상당히 단순해짐

사람은 직접 상대방을 보지 않아도 시선을 느낄 수 있는데
왜 camera-based media art에서는 작품이 자신을 보고 있다고 느끼지 않는가

고정된 anamorphic sweet spot을 작품의 viewpoint로 보고
그 위치를 관객에게 따라가게 만들면
작품의 시선에도 방향을 줄 수 있지 않을까

Kinect를 이용해 viewer position을 계산하고
그 위치에 맞춰 virtual viewpoint를 변화시키는 구조 설명

초지향성 스피커 역시 보이지 않는 방향성을 만드는 또 다른 축으로 제시

당시 발표 시점의 계획과 이후 실제 전시 구현 상태는 구분해서 기록 필요

### 2023-06-19 — Circuit Verification

초지향성 스피커 회로의 원리와 reference circuit 재검토

NE555
audio modulation
driver
ultrasonic transducer 연결 구조 등을 확인

reference schematic과 실제 제작 회로를 비교하면서 구성 정리

### 2023-06-20 — Circuit Design

제작 중인 회로를 Fritzing과 Tinkercad에서 다시 정리

`ultrasonicspeaker.fzz` 제작

이미 납땜을 시작한 뒤였기 때문에
제작 전에 설계한 회로라기보다 실제 작업을 진행하면서 연결 상태를 다시 확인하기 위한 과정

### 2023-06-21 — Parametric Speaker Modulation Test

6월 21일 시작해 자정을 넘긴 일부 6월 22일 사진까지 하나의 테스트 session으로 정리

실제 audio modulation과 출력 테스트

reference schematic의 resistor 값을 그대로 사용하는 것이 아니라
실제 입력 전력
audio source
driver
transducer array 조건에 맞춰 resistor 값을 반복적으로 변경

방향성을 유지하면서 사용할 수 있는 출력 범위를 찾는 과정

L298N을 ultrasonic output driver로 사용한 테스트도 이 시기에 진행

### 2023-06-23 — RC Filter and Audio Input Tuning

desktop headphone output을 실제 audio input으로 사용

일반적인 line input 조건과 다를 수 있어서
PC 출력 조건과 cable
impedance
resistor / capacitor 조합 등을 함께 확인

RC cutoff와 modulation 상태를 보면서 회로 조정

개별 부품 값 하나보다
audio source → circuit → power → output 전체 조건을 같이 맞추는 방향

### 2023-06-23 — Azure Kinect Reservation

실제 전시 환경 tracking 테스트를 위해 Azure Kinect 대여 예약

6월 26일부터 30일까지 사용

같은 예약 내역에 존재하는 다른 equipment code는 현재 의미 확인 필요

### 2023-06-24 — 555 Simulation and Real-world Comparison

555 Timer Calculator와 Tinkercad를 이용해 modulation 조건 반복 확인

40kHz 근처 carrier 조건
resistor / capacitor 조합
power condition 등을 바꿔가며 simulation

처음에는 battery나 PC USB 등을 이용해 전원을 공급하다가
전원 조건 자체도 modulation에 영향을 준다는 것을 확인하면서 bench power supply 사용으로 이동

simulation waveform 변화와
실제 speaker에서 들리는 결과를 비교하면서 값을 조정

simulation → 실제 출력 → 다시 simulation

형태로 반복

### 2023-06-24 — Kinect-based Direction Control Research

Kinect 좌표를 이용해 directional speaker의 방향을 계산하는 방법 조사

* Kinect Airsoft Turret
* TouchDesigner Look At axis 제한
* servo control examples

viewer position을 실제 mechanical orientation으로 변환하는 방법 탐색

연구 / prototype과 최종 전시 구현 범위는 별도 구분 필요

### 2023-06-27 — Exhibition-space Setup

실제 전시 공간에서 display와 tracking system 설치

2개의 display
PC
Azure Kinect 등을 실제 공간 조건에 맞게 배치

Kinect 설치 위치
높이
angle
tracking range 등을 현장에서 확인

이때부터 laboratory test보다 실제 전시장 조건에서 조정하는 단계

### 2023-06-29 — On-site Calibration

실제 전시장 기준으로 Kinect와 visual system 조정

`lookup.4.toe` 파일과 Screen Xform 관련 자료 보존

viewer tracking
display geometry
viewpoint transformation 사이의 현장 보정 작업이 있었던 것으로 확인

다만 정확히 어떤 parameter를 어디까지 조정했는지는
source evidence와 당시 기억을 더 확인해 세부 범위를 확정할 필요 있음

### 2023-06-29 — Final Power Setup

bench power supply를 사용해 speaker circuit의 실제 동작 조건 조정

최종 기록 사진 기준

* CH1 — 16.9V / 0.11A
* CH2 — 3.4V / 0.01A

초기 prototype 과정에서 STM32와 HW-131 등을 사용했던 구성은 이후 변경

최종 전시 hardware의 정확한 전원 연결 구조는
사진과 남아 있는 회로 evidence를 기준으로 별도 정리

---

## July 2023 — Exhibition

### 2023-07-02 — Final Installation Documentation

실제 전시 설치 상태에 대한 사진과 작품 설명 자료 존재

이 자료는 날짜별 제작 process의 연장이라기보다
완성된 설치 상태를 기록하는 exhibition documentation으로 분리

확인되는 요소

* `보이다` 작품 설명
* TEAM 0th axis / 오영서 표기
* actual exhibition space
* display system
* camera / tracking system
* ultrasonic transducer speaker module
* 최종 설치 hardware

speaker array는 최종 설치 사진에서 4 × 5
총 20개의 ultrasonic transducer로 구성

speaker module 전원은 main visual system과 분리해 별도 battery로 공급

세부 설치 구조는 source evidence가 확인되는 범위까지만 기록하고
사진만으로 확정할 수 없는 controller나 signal path는 추정하지 않음

---

# Development Flow

전체 흐름을 압축하면

**시선과 존재에 대한 초기 탐색**

↓

**Lacan의 gaze / objet a를 중심으로 한 개념 연구**

↓

**관객이 작품의 시선을 어떻게 느낄 수 있는가**

↓

**perception / anamorphosis / viewpoint-dependent image 연구**

↓

**고정된 sweet spot을 작품의 viewpoint로 다시 해석**

↓

**viewer tracking + moving viewpoint prototype**

동시에

**보이지 않는 방향성을 가진 sound**

↓

**parametric speaker feasibility**

↓

**speaker hardware / modulation / power test**

두 방향이 병렬로 진행

↓

**Kinect 기반 tracking과 실제 전시장 calibration**

↓

**visual system + directional sound system의 전시 설치**

---

# Archive Note

이 timeline에서는 작업을 최종 결과에 맞춰 역으로 정리하지 않음

초기에 중요했지만 이후 폐기된 아이디어
prototype까지만 진행한 기술
최종 전시 여부가 확인되지 않는 기능도 당시 위치에 그대로 남김

특히

* digital solidification
* 일부 실시간 AI generation 구상
* generative sound
* servo-based speaker tracking

등은 최종 구현 여부를 timeline만으로 확정하지 않음

실제 전시 구현 상태는 별도의 `Final Implementation Boundary` 문서에서

* implemented in exhibition
* prototyped / tested but final deployment unconfirmed
* planned / researched only
* unresolved

로 구분
