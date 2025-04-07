# HDA1 차량의 배선 개조

## <mark style="background-color:purple;">준비물</mark>

[레이더 커넥터 암/수](https://ko.aliexpress.com/item/1005005116795325.html?spm=a2g0o.order_list.order_list_main.38.5213140fEabSjz\&gatewayAdapt=glo2kor), 무탈피 커넥터

HDA1 차량은 범퍼의 SCC모듈의 신호를 실내로 가져와야합니다.

따라서, 범퍼를 탈거해야합니다.



## 개조시작

* 차량 배선도 ( [Hyundai GSW](https://gsw.hyundai.com/hmc/login.tiles), [KIA GSW ](https://gsw.kia.com/kmc/login.tiles)) 를 참고하여, C-CAN Low와 C-CAN High의 위치를 확인합니다.
* 위 판매링크에서 구매한 암/수 커넥터와 GSW를 비교하여, 커넥터의 C-CAN High, C-CAN Low 선을 랜선이나 20AWG 선으로 연장합니다.
  * 암/수 커넥터를 구매하지 않고 진행하실 분은, 차량의 순정 배선을 절단하고 작업하셔도 됩니다.



* 범퍼를 탈거합니다.

<figure><img src="../.gitbook/assets/image (12).png" alt="" width="563"><figcaption><p>Santa FE TM 범퍼 탈거 - 출처 : 당근마스터님</p></figcaption></figure>

* SCC모듈의 배선을 감싸고 있는, 검은색 테이프를 벗겨냅니다.

<figure><img src="../.gitbook/assets/image (13).png" alt=""><figcaption><p>배선도 - 출처 : 당근마스터님</p></figcaption></figure>

* 위 배선도를 참고하여, 콤마의 하네스의 22번 핀에 C-CAN High, 24번 핀에 C-CAN Low를 연결합니다.
  * 무탈피 커넥터를 이용해 작업하면 매우 편리합니다.





## 배선개조 완료 후 콤마 롱컨 설정

* 토글 -> 오픈파일럿 가감속 제어(알파) 켜기
* carrot -> can HYUNDAI : CAMERA SCC 켜기
* carrot -> 시작 -> Read Cruise Speed from PCM 0으로 설정
