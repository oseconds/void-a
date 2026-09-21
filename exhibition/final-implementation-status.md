# VOID-A Final Implementation Status

> This file is a 2026-09-18 retrospective archive reconstruction. It is not a contemporaneous 2023 production log.

## Scope

이 문서는 기존 날짜별 process history를 대체하지 않는다.
현재 raw archive와 media evidence를 기준으로 연구, 프로토타입,
물리적 설치 상태와 runtime 동작을 구분한다.

`Implemented in final exhibition`은 물리적 설치 또는 기록된 전원 구성을 뜻할 수 있지만,
그 자체로 tracking, audio output, servo movement가 실제 runtime에서 동작했다는 뜻은 아니다.

## Late Installation / Exhibition Evidence

다음 자료는 특정한 2023-07-02 행사의 확정 기록으로 묶지 않고,
후기 설치·전시 상태를 보여주는 evidence로 취급한다.

- `assets/void-a_footage_from_mobile/06_exhibition-documentation/1688312987148-5(1).jpg`
- `assets/void-a_footage_from_mobile/06_exhibition-documentation/1688366312045.jpg`
- `assets/void-a_footage_from_mobile/06_exhibition-documentation/1688366314295.jpg`
- `assets/void-a_footage_from_mobile/09_video-documentation/kakaotalk_1688312373255.mp4`
- `assets/void-a_footage_from_mobile/09_video-documentation/kakaotalk_1688312373255_1.mp4`
- `assets/void-a_footage_from_mobile/09_video-documentation/kakaotalk_1688312374413.mp4`
- `assets/void-a_footage_from_mobile/09_video-documentation/kakaotalk_1688366354025.mp4`

이 자료에서 다음 물리적 상태가 관찰된다.

- 두 개의 display와 스탠드 구성
- display 상부의 camera/sensor 배치
- 화면에 표시된 시각 출력
- 하부의 회로, 배선과 초음파 트랜스듀서 모듈

이 자료만으로는 특정 행사명, 공개 기간, 최종 runtime 동작, 최종 전원 연결을 확정하지 않는다.

## Implemented in final exhibition

여기서 구현은 우선 물리적 존재 또는 기록된 구성에 한정한다.
runtime behavior는 별도로 판정한다.

- display / screen configuration의 물리적 설치
- 설치된 display에서 시각 출력이 보이는 상태
- camera/sensor가 포함된 설치 구성
  - 기존 2023-06-27 문서는 이를 Azure Kinect 설치 맥락으로 기록하지만,
    이미지 자체만으로 장치 모델을 식별하지 않는다.
- ultrasonic / parametric speaker module의 물리적 설치
- 2023-06-29 기록의 DC power supply 구성
  - CH1: 16.9V / 0.11A
  - CH2: 3.4V / 0.01A
  - 이 항목은 speaker module 전원 구성의 기록이며, 최종 음향 출력의 증거는 아니다.

## Prototyped / tested but final deployment unconfirmed

- TouchDesigner viewpoint / anamorphic system의 관객 위치 기반 runtime response
- Kinect viewer tracking의 최종 runtime 동작
- viewer coordinates와 virtual camera parameter의 최종 적용
- 555/L298N modulation circuit의 최종 음향 출력
- 관객을 향하는 directional speaker physical aiming
- 3-axis servo tracking의 실제 자동 movement
- Max/MSP 기반 audio feedback network의 최종 전시 적용

물리적 camera, display, speaker module 또는 회로가 설치 사진에 보인다는 사실은
위 기능들이 전시 중 runtime에서 동작했다는 증거와 동일하지 않다.

## Researched / planned only

- 관객 데이터를 이용한 AI texture generation
- 관객의 시선 또는 위치를 이용한 generative audio의 최종 구현

`docs/04_process/2023-06-final-presentation.md`의 관련 내용은 계획·구상으로 남긴다.
2023-07-27 TouchDesigner/ControlNet capture는 VOID-A 최종 구현 증거로 사용하지 않는다.

## Unresolved from current evidence

- `lookup.4.toe`의 raw repository 내 실제 파일 위치
- Screen Xform의 실제 값과 최종 적용 상태
- 후기 설치 자료의 정확한 행사명·공개 기간·공식 provenance
- 최종 전시에서 Kinect tracking이 실제로 관객 움직임에 반응했는지
- 최종 전시에서 초지향성 speaker가 실제로 음향을 출력했는지
- 최종 전시에서 3-axis servo가 실제로 관객을 따라 움직였는지
- M015와 같은 interaction instruction signage가 VOID-A/보이다에 직접 속해 설치된 것인지

## Owner-confirmed context

다음은 media 자체에서 판독한 사실이 아니라 owner clarification으로 보존한다.

- 2023-06-29 DC power supply는 초지향성 speaker module의 최종 전시용 전원이었고 설치 테스트 중에도 사용했다.
- 후기 설치 자료에서 별도 battery로 구동한 대상은 speaker module이 아니라 3-axis servo motor였다.

이 owner context는 media에서 직접 확인되는 runtime proof와 분리한다.

## Excluded from direct evidence / provenance candidates

- `assets/void-a_footage_from_mobile/99_unclassified/20230702_191228.jpg` (inventory M067)
  - VOID-A identifier가 충분하지 않은 ambiguous media로 취급한다.
  - final-installation direct evidence 목록에서는 제외하고 contextual/provenance candidate로만 남긴다.
- 2023-07-03~04 SNS / Docs captures
  - 후기 exhibition communication 또는 project statement 후보
- 2023-07-24 speaker/electronics media
  - 기존 prototype/reference 자료의 후속 수집인지 별도 development event인지 미확정
- 2023-07-27 TouchDesigner capture
  - external/reference 또는 later-development candidate

위 provenance candidates는 timeline에 자동 추가하지 않는다.
