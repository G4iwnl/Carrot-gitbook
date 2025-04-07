---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 레이더트랙

## Radar Tracks (레이더트랙)

*   레이더모듈(SCC모듈)에서 레이더의 raw data를 출력하도록 활성화시키는 것입니다.

    <mark style="color:red;">**만도레이더**</mark>를 사용하는 **극히 일부 차량에서만** 작동합니다.

    ​
*   **설정방법**

    콤마 설정 Carrot에 들어가 **Enable RadarTrack** 을 1로 하면 시동시, 레이더트랙을 활성화하기 위해 레이더모듈의 ECU에 config를 바꿉니다.


*   **현재까지 확인 된 지원 차량**

    2020 SONATA

    2020 PALISADE

    2019, 2020 SANTAFE

    2020 G70

    K5 HEV\
    STARIA



* **레이더 트랙이 되는 차량인지 확인하는 방법**
  * 레이더 트랙 설정을 활성화 한 후, 시동시 에러가 나지 않아야 합니다.
  * 주행중 전방의 100M이내의 차량에 대해 노란색 박스가 변하지 않고 지속되며 원할한 운전이 지속되어야 합니다.

## 레이더 트랙 롱컨

* 레이더 트랙이 지원되는 차량은, 배선개조 없이 롱컨을 사용가능합니다.
* 레이더 트랙 설정을 활성화 하고, 토글 메뉴에서 오픈파일럿 가감속 설정을 활성화 해주면 롱컨이 가능합니다.

## <mark style="background-color:red;">주의점</mark>

* 레이더 트랙 롱컨의 경우에는, 순정의 안전관련기능(AEB[^1], FCW[^2]등)을 사용할 수 없습니다.
* HDA2 차량은 레이더트랙을 사용할 수 없습니다.

[^1]: Autonomous Emergency Braking : 자동긴급제동

[^2]: Forward Collision Warning : 전방추돌경고
