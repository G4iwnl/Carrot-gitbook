# Fleet

## Fleet 이란 ?&#x20;

* View Dashcam Footage: 주행 로그를 볼 수 있으며, 다운로드를 받을  수 있다.
* View Screen Recordings: 화면녹화 로그를 볼 수 있으며, 다운로드를 받을 수 있다.
* Error Logs, Navigation: 현재작동안함
* Tools : 설정값을 백업 및 복원가능

## Fleet 접속 방법

* 휴대폰과 콤마를 같은 네트워크에 두고 당근맨의 Fleet을 클릭하거나
* 콤마 화면 우측 하단 아이피를 참고하여, 아이피 뒤에 :8082를 붙여 인터넷으로 접속

&#x20; 콤마 화면에 192.168.127.35가 표시된 경우, 인터넷 주소창에 192.168.127.35:8082 입력



## <mark style="background-color:red;">Fleet 에 접속이 되지 않을 때</mark>

* AGNOS를 업데이트 하면, Flask가 날아가게 되어 fleet에 접속이 되지 않는 현상이 발생합니다.
* [Install Flask 수행](../carrotman/basic.md#menu)을 통해 다시 fleet이 기능을 하도록 해줍니다.

## 해결방법

* 콤마와 휴대폰을 같은 네트워크에 연결
* 당근맨 실행
* MENU -> Install Flask 클릭
* MENU -> Reboot&#x20;
* 콤마 리부팅 후 Fleet 정상 작동
