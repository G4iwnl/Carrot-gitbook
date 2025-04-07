# SSH 접속 ( PC로 )

PuTTY 다운로드

* [https://www.chiark.greenend.org.uk/\~sgtatham/putty/latest.html](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)
* 64-bit x86 `항목 다운로드 및 설치`

## PuTTY 실행 및 설정

* 상단의 Conversions -> import key&#x20;

<figure><img src="../.gitbook/assets/image (20).png" alt=""><figcaption><p><a href="https://flickerinsider.tistory.com/11">https://flickerinsider.tistory.com/11</a></p></figcaption></figure>

* [전에 생성했던 id\_rsa (ssh key 개인키 파일)](../basic-settings/ssh.md#ssh) 선택
* Save private key를 클릭
* 암호 설정 경고문이 뜨면, 예(y) 클릭.
* 적당한 파일명으로 저장&#x20;



* 메뉴 중 Connection – SSH – Auth – Credentials&#x20;
* Private key file for authentication에서, 위에서 생성한 ppk 파일 선택

<figure><img src="../.gitbook/assets/image (22).png" alt=""><figcaption><p><a href="https://flickerinsider.tistory.com/11">https://flickerinsider.tistory.com/11</a></p></figcaption></figure>

* 맨 위 Session 으로 이동
* Host name : 콤마 ip
* port는 22&#x20;
* Saved Sessions 접속 이름을 적당히 정하고, Save를 클릭
* 두 번째 접속부터는 저장한 세션 이름을 클릭 후 ‘Load’ 를 클릭하면 저장한 내용으로 접속이 가능
