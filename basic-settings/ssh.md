# SSH 키 생성 & 등록

## GIT 설치

* git 설치 ( [설치링크 ](https://git-scm.com/downloads))
* 위 링크에 접속하여,  Windows를 클릭하여 git을 설치합니다.



## SSH 키 생성

* cmd 실행
* ssh-keygen -t rsa -b 2048 -m PEM -f C:\id\_rsa

C:\id\_rsa 는 C:\ 드라이브의 위치에 id\_rsa 라는 이름의 키를 생성하는 것을 의미합니다.

상황에 따라 알맞게  위치를 입력합니다.

```
Generating public/private rsa key pair.
Enter passphrase (empty for no passphrase):

```

* 아무것도 입력하지 않고 엔터.

```
Enter same passphrase again:
```

* 아무것도 입력하지 않고 엔터.

```
Your identification has been saved in C:\id_rsa
Your public key has been saved in C:\id_rsa.pub
The key fingerprint is:
SHA256:I3Lq/Ifvt0a+7k9IAH+EYKf6OPbEzw0CzPyxwvwMY3k lim05@DESKTOP-OI7SHB6
The key's randomart image is:
+---[RSA 2048]----+
|      +....      |
|     . =..       |
|      . o .      |
|   + .   o       |
|    B + S .      |
|   o @ + o..     |
|    & E..o. .    |
|   = @.+.o+.     |
|    o.=+==*+.    |
+----[SHA256]-----+

```

* 키 생성 완료

## SSH 키 등록 ( GitHub )

* GitHub 로그인
* [https://github.com/settings/keys](https://github.com/settings/keys) 접속
*   우측 상단 **New SSH Key** 클릭

    <figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>
* Title : 임의의 이름 작성 ( 예 : Comma )
* Key Type : Authentication Key
*   Key : 앞에서 생성한 SSH 키 중에서, id\_rsa.pub 파일을 메모장으로 연 후, 안의 내용을 전부 복사해 붙여넣습니다.

    <figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>
* Add SSH Key 클릭

## SSH 키 등록 ( Comma )

* 콤마 설정 진입
* 개발자 (Developer) 클릭
* **SSH 키 사용** 활성화
* 바로아래, github id 추가 버튼 클릭
* github id 입력
  *   github id 확인방법

      * [https://github.com/](https://github.com/)  접속
      * 우측 최상단 프로필 사진 클릭
      * 닉네임이 표시됨.

      ( 하단 사진의 경우에는 G4iwnl)

      <figure><img src="../.gitbook/assets/image (9).png" alt="" width="245"><figcaption></figcaption></figure>

## SSH 키 등록 ( 당근맨 )

**사전 작업**

* 위에서 생성한 두개의 파일 ( id\_rsa, id\_rsa.pub ) 중에서, id\_rsa를 이메일, 카카오톡 등을 이용하여 휴대폰으로 전송

**당근맨에 SSH 키 등록**

* 당근맨 실행
* 좌측 상단 GIT 클릭
* SSH Key Settings
*   개인키 클릭 후 id\_rsa파일 선택

    <figure><img src="../.gitbook/assets/image (10).png" alt="" width="188"><figcaption></figcaption></figure>

