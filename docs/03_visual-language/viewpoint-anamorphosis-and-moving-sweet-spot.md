# Viewpoint, Anamorphosis, and the Moving Sweet Spot

## Before Anamorphosis

작업 초반부터 중요했던 것은 시선과 관객의 관계였지만
처음부터 anamorphosis나 sweet spot을 작품의 눈으로 생각했던 것은 아님

처음에는

작품이 관객을 보고 있다는 느낌을 어떻게 만들 수 있을까
관객이 단순히 인터랙션을 발생시키는 사람이 아니라
작품의 시선 안에 들어왔다는 느낌을 받을 수 있을까

이런 질문이 먼저 있었음

초기에는 Lacan의 gaze를 비롯해 시선과 지각에 관한 여러 개념을 조사했고
작품의 형태나 관객 데이터를 사용하는 방식도 여러 방향으로 생각

이 시점에는 아직 구체적인 시각 시스템이 정해져 있지 않았음

## Finding Anamorphosis

3월 말부터 perception과 공간 illusion에 관한 자료를 찾으면서
anamorphosis와 viewpoint-dependent image에 관심이 생김

특정한 위치에서 봤을 때만 이미지가 정상적으로 보이고
관찰자의 위치가 달라지면 형태가 크게 왜곡되는 구조

일반적인 이미지와 달리
이미지 자체가 관찰자의 위치를 강하게 요구한다는 점이 흥미로웠음

TouchDesigner의 Sweet Spot Previz 같은 자료도 이 과정에서 확인

여기서 처음에는 기술적인 방법으로 접근

실제 공간 안의 관객 위치를 기준으로
perspective를 실시간으로 바꾸면
고정된 화면에서도 입체적인 가상 공간이 존재하는 것처럼 만들 수 있겠다고 생각

## The Fixed Sweet Spot

anamorphic image에는 이미 특정한 관찰 위치가 존재

그 위치에 있을 때만 공간과 형태가 의도한 방식으로 성립

처음에는 이것을 단순히 viewer position이라고 봤는데
자료를 계속 보면서 이 고정된 위치를 다른 방식으로 볼 수 있겠다는 생각이 생김

이미지가 관객에게 요구하는 하나의 정확한 위치

그렇다면 이 위치를 관객의 눈이라고만 볼 필요가 있을까

오히려 작품이 관객을 바라보는 위치라고 생각할 수도 있지 않을까

여기서 sweet spot과 작품의 gaze가 연결됨

이건 작업 시작부터 가지고 있던 아이디어가 아니라
anamorphosis와 trompe-l'œil 구조를 조사하다가 나중에 나온 해석

## Reversing the Viewpoint

기존 anamorphic display에서는 관객이 작품이 정해놓은 위치를 찾아가야 함

관객이 sweet spot 안에 들어오면 이미지가 정상적으로 보이고
벗어나면 illusion이 깨짐

여기서 이 관계를 반대로 뒤집어봄

관객이 sweet spot을 찾아가는 대신
sweet spot이 관객을 따라가면?

관객의 위치를 계속 추적해서
virtual camera를 그 위치에 맞게 움직이면

관객이 어디에 있든
이미지는 계속 그 사람에게 맞는 perspective를 유지할 수 있음

결과적으로

내가 작품을 보기 위해 정해진 위치로 이동하는 것이 아니라
작품의 시점이 계속 나를 찾아오는 구조

이때부터 sweet spot을
작품이 바라보는 위치
작품의 시선이 향하는 지점처럼 생각하게 됨

## From Viewer Position to Artwork Gaze

기술적으로 보면

viewer position
→ virtual camera position
→ perspective transformation

이라는 비교적 단순한 구조

근데 작품 안에서는 이 구조를 다르게 읽고 싶었음

viewer position이라는 값을 단순한 interaction parameter로 사용하기보다
작품의 시선이 어디를 향하고 있는지를 결정하는 좌표로 사용

관객이 왼쪽으로 움직이면
그래픽이 왼쪽으로 반응하는 것이 아니라

작품이 관객을 계속 바라보기 위해
자신의 시점을 이동하는 것처럼 느껴지는 방향

같은 tracking 기술이라도
관객이 작품을 조작하는 구조와
작품이 관객을 추적하는 구조 사이에는 경험적으로 꽤 큰 차이가 있다고 생각

## Manual Viewpoint Test

실제 구현에서는 tracking보다 먼저 viewpoint rendering 자체를 테스트

TouchDesigner에서 virtual camera 위치를 직접 움직이며
카메라가 이동할 때 화면에 투영된 가상 공간이 제대로 변하는지 확인

이 단계에서는 실제 관객 위치가 아직 자동으로 연결되지 않았음

카메라 위치를 수동으로 움직여
여러 관찰 위치에서 perspective가 어떻게 변하는지 먼저 테스트

그래서 초기 prototype은

관객 tracking까지 완성된 시스템이라기보다
moving viewpoint의 시각적 원리가 실제 display에서 성립하는지 확인하는 단계

이 부분이 성공한 뒤
실제 관객 위치를 얻기 위한 Kinect tracking을 연결하는 방향으로 진행

## Invisible Tracking

관객 위치를 얻는 방법으로 처음에는 Vive tracker 같은 방식도 고려

하지만 관객이 tracker나 별도의 물체를 들고 있어야 한다면
자신이 시스템을 조작하고 있다는 느낌이 너무 강해질 수 있음

이번 작업에서는 반대로

내가 무엇을 조작하지 않았는데도
작품이 내 위치를 알고 있는 상황

이쪽이 더 중요했음

그래서 tracking 장치 자체가 관객 경험의 중심에 드러나지 않는 방향을 선호

Kinect나 depth camera로 관객 위치를 읽고
그 좌표를 virtual camera에 연결하는 방식으로 이동

## Artwork Viewpoint

이 과정을 거치면서 viewpoint는 단순한 렌더링 파라미터 이상의 의미를 가지게 됨

일반적인 perspective에서는
관객의 눈이 세계를 구성하는 기준점

`보이다`에서는 이 관계를 약간 뒤집고 싶었음

화면 속 가상 공간이 관객을 위해 존재하는 것처럼 보이지만
동시에 그 공간의 시점 자체가 관객을 계속 따라다님

관객이 보고 있는 동안
작품 역시 관객을 기준으로 자신의 시점을 계속 이동

이 움직이는 viewpoint가
작품이 관객에게 보내는 시선의 방향처럼 기능

## Relation to the Eye-creature

화면 속 눈을 가진 오브젝트와
viewpoint-dependent rendering도 따로 떨어진 요소로 생각하지 않았음

오브젝트는 작품이 하나의 존재처럼 느껴지게 만드는 시각적인 주체

moving sweet spot은
그 존재가 관객을 바라보고 있다는 관계를 공간 전체에 적용하는 구조

눈만 관객을 따라 움직이는 것이 아니라
오브젝트가 존재하는 가상 공간 자체의 시점이 관객에게 맞춰짐

그래서 시선은 캐릭터의 눈동자 움직임 하나로 표현되는 것이 아니라
화면 전체의 perspective를 통해서도 만들어지도록 생각

## Direction

처음에는 gaze라는 개념에서 시작했고
그다음에 anamorphosis라는 기술과 지각 현상을 발견했고
이후 그 안에 존재하는 fixed viewpoint를 작품의 시선으로 다시 해석

즉

gaze를 설명하기 위해 anamorphosis를 처음부터 선택한 것이 아니라

anamorphosis를 연구하면서
기존에 가지고 있던 gaze에 대한 질문과 연결되는 지점을 발견

그 지점이 이후 작품의 주요 시각 시스템으로 발전
