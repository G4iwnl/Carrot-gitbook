# 당근네비 & 당근맨 설치방법

## <mark style="background-color:blue;">UPDATES</mark>

* 트흐님과 당마님의 업데이트를 통해, 당근나비 2501 & 당근맨 69 버전부터 adb로 권한을 주는 과정이 필요 없게 되었습니다.

## 준비물

데이터 전송이 되는 케이블, 사용하실 폰, Windows PC, adb, 당근맨, 당근나비 파일

[**당근맨 & 당근네비 파일 얻는법**](../#and)

## ADB 다운로드 및 준비

* https://developer.android.com/tools/releases/platform-tools?hl=ko
* Windows SDK 플랫폼 도구 다운로드 클릭.
* 약관 동의 및 다운로드
* 다운로드 한 zip 파일 압축 풀기 (아래 사진과 같이)
* 압축 푼 폴더 안에 apk 파일 2개 넣기.

<figure><img src="../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

* 스마트폰 설정 -> 휴대전화 정보 -> 소프트웨어 정보 -> 빌드번호 10회 연속 클릭
* 뒤로가기 후, 개발자 옵션 진입.
* usb 디버깅 허용.

## ADB로 앱 설치

* <mark style="background-color:blue;">휴대폰에서 apk파일로 바로 설치가 되지 않을 때 사용합니다.</mark>
* 휴대폰에서 기존의 앱을 삭제합니다.
* adb 파일을 옮겼던 폴더로 가서 주소창의 빈부분 (아래 사진 참고)을 클릭합니다.

<figure><img src="../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

* CMD 입력 후 엔터
* cmd 창 열리면, adb devices 입력해서 연결 상태 확인. ( XXXXXXXXXXXXX device ) 형식으로 표시됨.
* adb install -r CarrotMan68.apk (Performing Streamed Install, Success 문구 나오고 완료됨)

<mark style="background-color:red;">(CarrotMan68.apk 와 같은 앱 이름은 상황에 따라 알맞게 수정)</mark>

## 차량에서

* 휴대폰에서 핫스팟을 켜고, 콤마 기기에서 핫스팟에 연결합니다.
* 네비 목적지를 입력하기 전에는 APM 아이콘이 나오고, 목적지/안심주행 상태로 들어가면 APN 상태가 되어 네비 연동이 됩니다.

## FAQ

Q. 안드로이드 오토를 그대로 사용할 수 있나요?&#x20;

A. No. 플레이스토어에서 공식으로 가져온 앱이 아닌, 제 3자에 의해 수정된 앱이기에 불가능합니다.
