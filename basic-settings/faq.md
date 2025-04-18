# FAQ

## Q. 레인모드, 레인리스 모드를 어떻게 전환하나요?

* 차량 핸들 리모콘의 LFA 버튼을 길게 눌러 레인모드, 레인리스 모드를 전환할 수 있습니다.
  * 콤마 화면 맨 아래 중간 부분을 보면 현재 모드 상태를 확인할 수 있습니다.

<figure><img src="../.gitbook/assets/image (5).png" alt=""><figcaption><p>LFA 버튼</p></figcaption></figure>

## Q. 차선중앙유지가 만족스럽지 않아요.

* Laneless(레인리스)를 사용하는경우 모델이 차선을 잡아줌
* 전적으로 모델이 하는것이기때문에 별도의 튜닝이 없음
* [조향튜닝](../tuning/steering.md)에 문제가 있는경우에는 튜닝을 해야함 ([steerMax](../tuning/steering.md#steermax), [TorqueAccelFactor, FrictionFactor](../tuning/steering.md#torqueaccelfactor-frictionfactor))
* 커브의 경우 또다른 튜닝이 필요함(SAD)
  * 생각한 것보다 핸들을 빠르게 돌리기 시작하면, SAD값이 너무 큰 상태
  * 생각한 것보다 핸들을 느리게 돌리기 시작하면, SAD값이 너무 작은 상태
* 레인모드인 경우 또다른 튜닝이 필요
  * 레인모드의 시간지연보상의 경우, SAD와 같은 성질을 가짐

## Q. 신호정지가 잘 안돼요.

* 전적으로 모델의 판단을 사용함
* 모델에 따라서 잘될때가 있고 안될때가 있음
* 사용하기 싫은경우 고속 모드로 전환해서 사용해야함
  * 모드 전환은, 차량 핸들 리모콘의 차량간격 버튼을 길게 눌러 조절 가능
* 시속80키로를 초과하면 신호 인식이 비활성화 됨

## Q. 차선중앙유지가 안돼요.

* Laneless(레인리스)를 사용하는경우 모델이 차선을 잡아줍니다.
* Laneless(레인리스)의 경우, 전적으로 모델이 하는 것이기 때문에 별도의 튜닝이 없음
* 단, 조향튜닝에 문제가 있는경우에는 튜닝을 해야함 (steerMax, AccelFactor, friction)
* 커브의 경우 또 다른 튜닝이 필요함(SAD)
* 레인모드인 경우 또 다른 튜닝이 필요

## Q. 앞차와의 간격이 너무 멀게 주행함....

* ComfortBrake: 이값이 낮으면 멀게주행, 감속할때 서서히 감속하겠다는 것임.. 230\~240 권장
* 앞차간격: 1\~4단계로 설정하며, 줄일수록 차량간격이 좁아짐.
* 연비모드: ComfortBrake값을 10% 줄여서 운행함.
* 안전모드: ComfortBrake값을 20% 줄여서 운행함.
* Radar Reaction factor: 값이 크면 앞차의 반응에 둔감.. (거리와는 관련이 적지만)

## Q. 모델이란?

* 콤마는 콤마가 학습시킨 모델을 이용합니다.
* 모델은 조향제어, 차선인식, 전방차량인식, 신호감지등의 역할을 합니다.

## Q. 캘리브레이션을 하는 이유

* 오파장착위치 자동 계산.
* 차량이 바뀌거나, 장착위치가 바뀌면 캘리를 해야함.
* 모델이 바뀌었을때는 할 이유가 없음..
* 캘리가 틀어진 경우에는 자동으로 판단하여 다시 캘리브레이션을 함.
* 하지만, 오파작동이 갑자기 이상할 때는 한번쯤 시도해 볼만 함.

## Q. [롱컨 개조를 하는 이유.](../longcontrol/whylong.md)

## Q. 엑셀톡이란?

* 엑셀톡은 엑셀을 매우 짧게 (0.6초) 톡 밟고 떼는 것을 말합니다.
* 당근파일럿에서는 엑셀톡을 사용해 속도를 증가시킬 수 있습니다.

## 용어설명

* 롱컨: Longitudinal Control, 크루즈컨트롤과 같은 뜻
* [롱컨개조](broken-reference/): 차량의 크루즈컨트롤을 오픈파일럿의 롱컨으로 제어하기 위해 배선을 개조하는 작업
* 인게이지: 오파를 작동하기 위한 제어의 활성화하는 작업
* [레이더트랙](../functions/radartrack.md): 레이더모듈의 가공되지 않은 레이더 데이터정보들을 말함
* NOO : Navigate On Openpilot, 네비게이션 경로에 따라서 자동차선변경 및 턴을 지원함, **현재는 사라진기능**
* ATC: Auto Turn Control, 당근의 기능으로 NOO와 비슷하게 차로변경 및 턴을 지원함. **아직 완벽하지는 않음**.
* VTSC: Vision Turn control, 모델이 측정한 경로의 곡률을 토대로 속도를 제어하는 기능
* 앵글이, 앵글컨트롤 : LFA2 를 일컫는 말입니다. 기존에 토크제어라고 불리던 LFA1과는 조향 방식이 다릅니다.
