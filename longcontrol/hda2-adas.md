# HDA2 차량의 배선 개조 (ADAS)

<mark style="background-color:purple;">준비물</mark>

[MG656971-5](https://smartstore.naver.com/nobleseat/products/8283802097?nl-query=mg656971\&nl-ts-pid=i25wJsqVOswsstsKYmZssssstLC-217972\&NaPm=ct%3Dm4tjb1y0%7Cci%3Da48a8d1cbbc46bdb22c3275bb19a84efa7423f6b%7Ctr%3Dsls%7Csn%3D2916848%7Chk%3De1ac7d01612b8fcc25da022f16d70e342e377ff8), [MG646151-5](https://smartstore.naver.com/jautoment), 기존 콤마 18핀/ 26핀하네스, c to c 3.1 gen2 케이블(2m 권장)

or

[잭by잭 완성품 구매(제이엠테크엔)](https://smartstore.naver.com/jmtechn/products/11248346315)



HDA2 차량은 HDA1 차량과 다르게 실내 (adas 모듈)에서 작업합니다.

## 배선 제작 기본 원리

* 기존 콤마 하네스의 Camera쪽은 Bypass
* adas의 ecan만 하네스의 bus2에 연결

![](<../.gitbook/assets/image (34) (1).png>)![](<../.gitbook/assets/image (35).png>)

* 사진 출처 : 포르티시모님, 로웰님 ( Discord )



제작이 힘들다면..?  [잭by잭 완성품 구매(제이엠테크엔)](https://smartstore.naver.com/jmtechn/products/11248346315)

## 차량에서,

* GSW ( [Hyundai GSW](https://gsw.hyundai.com/hmc/login.tiles), [KIA GSW ](https://gsw.kia.com/kmc/login.tiles)) 를 참고하여, adas 모듈 위치를 확인합니다.
* ADAS 모듈에서, 기존 커넥터를 제거하고 새로 만든 배선을 연결합니다.
* 하네스 박스를 적당한 위치에 잘 고정하고, c to c 3.1 gen2 cable을 이용해 콤마에 연결합니다.

## 배선개조 완료 후 콤마 롱컨 설정

* 토글 -> 오픈파일럿 가감속 제어(알파) 켜기
* carrot -> can HYUNDAI : CAMERA SCC 켜기
* carrot -> 시작 -> Read Cruise Speed from PCM 0으로 설정
* carrot -> 시작 -> canfd hda2 켜기

## 참고 - 작동원리

* ADAS에서 출력되는 ECAN의 데이터를 BUS2로 연결하면
* 오파가 작동될때, BUS2와 BUS0가 분리됨.
* BUS2에 수신되는 ECAN데이터를 적당히 가공해서 BUS0로 다시 송출함.
* BUS2, BUS0은 모두 ECAN임.
