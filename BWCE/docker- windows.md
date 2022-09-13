# Window에 Docker 설치

## 1. Hyper-V 활성화 

### 1.1 가상화 환경 설정

작업 관리자를 열어서 `가상화`가 사용중 인지 확인합니다.

만약 사용중이 아니라면 사용하시는 PC의 BIOS 환경에 들어가서 가상화 옵션을 활성화 시키셔야 합니다.
BIOS의 경우 Virtualization Technology 및 VT-d(있는 경우) 옵션을 활성화 합니다.

![img](https://blog.kakaocdn.net/dn/bnE6Ib/btqD0jhR2ol/dMEPBUVFHMOTCw3gIomrk0/img.png)

### 1.2 Window Hyper-V 활성화
제어판 > 프로그램 설치 및 제거 > Window 기능 켜기/끄기 클릭 > Hyper-V 체크 확인 후 리부팅

![img](https://blog.kakaocdn.net/dn/qtUdX/btqD2dgKmrG/Lna2JrCK9QtSkElPZ4xjf1/img.png)

## 2. Docker Desktop 설치

### 2.1. Docker Desktop 다운 및 설치

[https://docs.docker.com/docker-for-windows/install/](https://docs.docker.com/docker-for-windows/install/)

### 2.2. PC 재기동 및 Docker Desktop 실행

![img](https://blog.kakaocdn.net/dn/bdjK7w/btqD3d1rnn1/5V28NmDqb1slQpzkkoAy5K/img.png)

![img](https://blog.kakaocdn.net/dn/DOi3J/btqD1pPtc8X/0KK08Hrk6GqJaEjeJeZdW0/img.png)

### 2.3 WLS2 (Linux kernel) 설치

Windows 버전에 따라 Docker 실행시 아래 메시지가 나온다면 해당 링크를 따라 WLS2를 설치 후 PC를 재부팅 합니다.

![img](https://blog.kakaocdn.net/dn/bVMJnC/btqQR5ROHuq/4yU3fnCTa0MFkoCk74l6lK/img.png)




