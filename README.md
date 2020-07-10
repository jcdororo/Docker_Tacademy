# Docker_Tacademy

T아카데미 (https://tacademy.skplanet.com/frontMain.action) 에서 도커에대해 배운 영상을 정리한 내용입니다.

윈도우 홈버전 도커 설치방법
========================
1. Hyper-V.bat 설치하여 관리자 권한으로 실행 한 후 컴퓨터를 다시시작
2. 재부팅 후 Windows 기능 켜기/끄기 에서 Hyper-V 체크후 확인하여 활성화
3. 윈도우 버전을 우회하기 위해 레지스트리 편집기를 열고 HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion 으로 이동
4. EditionID 값을 찾아 값 데이터를(V): [Professional]로 변경
4-1. EditionID 값 변경 후에도 Docker Installer에서 버전 우회가 되지 않는다면 PRoductName 값 역시 Professional로 변경
5. 레지스트리 변경이 모두 완료되면 DOcker Installer 실행 (https://docs.docker.com/docker-for-windows/install/)
6. 설치 완료 후 4에서 변경한 데이터값을 원래대로 되돌려놓기.
7. 명령 프롬프트창(CMD)를 관리자 권한으로 실행 후 docker run hello-world 명령어를 입력하여 정상 동작하는지 확인.
