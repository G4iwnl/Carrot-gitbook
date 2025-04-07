# 추가 정보 - 무선 adb

## 조건

* <mark style="background-color:purple;">ssh를 이용하기 위해서는</mark> <mark style="background-color:purple;"></mark><mark style="background-color:purple;">**기기와 휴대폰이 같은 네트워크 상**</mark><mark style="background-color:purple;">에 있어야 합니다!</mark>
* 휴대폰에 ADB Shell - Debug Toolbox 앱 다운로드
* [https://play.google.com/store/apps/details?id=com.github.standardadb\&pcampaignid=web\_share](https://play.google.com/store/apps/details?id=com.github.standardadb\&pcampaignid=web_share)

## 무선 디버깅 활성화

* 개발자 옵션 진입 후 무선 디버깅 활성화

<figure><img src="../.gitbook/assets/image (23).png" alt=""><figcaption><p>개발자 옵션</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

* 페어링 코드로 기기 페어링  클릭
* 아래 사진을 참고하여 나오는 페어링 코드, IP주소 및 포트 메모(사진 찍어두기)

<figure><img src="../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

## 휴대폰 ADB Shell - Debug Toolbox앱 에서

<figure><img src="../.gitbook/assets/image (27).png" alt="" width="375"><figcaption></figcaption></figure>

예시는 이해하시기 쉽게, 위의 사진에 나오는 숫자를 이용합니다.

* adb pair ip:port 입력 ( 예시 : adb pair 192.168.0.26:35331 )
* 페어링 코드 입력 ( 예시 : 638688 )
* adb connect ip:port 입력 ( 예시 : adb connect 192.168.0.26:39935 )
* 필요한 명령어 입력 (adb shell pm grant com.ajouatom.carrotman android.permission.READ\_LOGS)
