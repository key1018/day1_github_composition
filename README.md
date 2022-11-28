#  WSL2을 이용한 linux 환경구성 방법

## 설치 환경 구성 <br>
## 1. Chocolatey 설치 <br>
Chocolatey란? <br>
➡️ 리눅스에서의 apt, yum, homebrew과 같이 패키지를 설치/업데이트/제거 관리하는데 사용하는 Windows 프로그램 <br>
즉, <i><b>리눅스 계열의 패키지 관리자와 유사</b></i>하며 해당 서버에서 저장소에 저장된 프로그램을 바로 불러와서 사용할 수 있다. <br>
삭제 또한 명령어 한줄로 가능하며, 업데이트 관리도 매우 용이하다. <br>
[chocolatey 설치경로](https://chocolatey.org/)

<details>
<summary>apt, yum, homebrew</summary>
<div markdown="1">

- apt : Ubuntu, Debian 및 관련 Linux 배포에 deb 패키지를 설치, 업데이트, 제거 및 관리하기 위한 명령줄 유틸리티 <br>
   - 참고자료 : [apt 명령어/사용방법/예제](https://jjeongil.tistory.com/1672), [apt와 apt-get의 차이](https://coding-groot.tistory.com/90)
- yum : RPM 기반의 시스템을 위한 자동 업데이터이자 소프트웨어와 같은 패키지 설치/ 삭제 도구로 패키지 의존성 문제를 자동으로 처리하면서 설치, 업데이트, 삭제를 진행 <br>
   - 참고자료 : [리눅스 YUM이란?](https://dololak.tistory.com/331), [리눅스 YUM 기본 명령어](https://velog.io/@zeesoo/Linux-%EA%B8%B0%EB%B3%B8-%EB%AA%85%EB%A0%B9%EC%96%B4-yum) <br>
- homebrew : 무료 오픈 소스 소프트웨어 패키지 관리자 솔루션으로 애플의 맥OS 운영체제와 리눅스에 소프트웨어를 설치가능 <br><br>

</div>
</details>

### 1) chocolatey command 복사
![image](https://user-images.githubusercontent.com/103404357/204304472-839d40cd-7047-47f7-80a5-d67b01438490.png)

### 2) Powershell 실행 후 명령 붙여넣기
![image](https://user-images.githubusercontent.com/103404357/204313672-e6b3beba-8ce6-45b4-a9be-88f1d332c4a7.png)
<br>

## 2. Windows Terminal 관리자 권한으로 실행 <br>

### 1) windows Terminal을 통해 WSL 관련 기능 활성화
`dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart`

![image](https://user-images.githubusercontent.com/103404357/204317288-8f66e129-c808-48ee-9d7b-daba11f26c44.png)

## 3. Ubuntu 설치 <br>
Ubuntu란? <br>
➡️ 리눅스 커널에 다양한 응용프로그램을 추가해 쉽게 설치할 수 있도록 만든 리눅스 배포판 중 하나이다.


