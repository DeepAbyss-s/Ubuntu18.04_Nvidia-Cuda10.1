# Ubuntu18.04_Nvidia-Cuda10.1

CUDA를 사용하는 이유는 매우간단하다.

GPU(그래픽카드)에 메모리를 할당하고 CPU보다 많은양의 연산량을 빠르게 처리가 가능하다.

CPU는 코어 적은 반면에 코어당 속도가 상당히 빠르다, 하지만 GPU의 경우 코어는 상당히 많지만 코어당 속도가 CPU보다 느리다.

CPU의 속도는 최대 5.0Ghz 까지 올라가지만 GPU의 속도 같은 경우에는 1.8Ghz가 거의 최대이다.
CPU의 코어는 일반적으로 4~20코어정도가 대부분이지만 GPU의 쿠다는 일반적으로 1500~4600개까지이다

쉽게 설명하자면 CPU는 인정받은 천재 몇 명 앉아서 일을 해결하는 것이고, GPU는 능력이 있는 일반인들 수천명이 앉아서 일을 해결하는 것과 비슷하다.

머신러닝의 특성상 최고성능의 GPU를 활용하면 속도와 효율을 더 높일 수 있다.


# 우분투 버전
- Ubuntu 18.04.4 LTS AMD64버전

## 참조
쿠다드라이버만 설치를 하여도 엔비디아 최신 그래픽드라이버가 설치가 됩니다.

만약 다른 드라이버를 사용해야 한다면 아래의 링크인 엔비디아 드라이버설치하는 세션으로 가셔서 진행을 하시면됩니다.
- [엔비디아 드라이버 설치](https://github.com/DeepAbyss-s/Ubuntu18.04_Nvidia-driver)

# 지원하는 그래픽카드 확인
- [엔비디아 쿠다드라이버 공식 홈페이지](https://developer.nvidia.com/cuda-gpus)

# 권장사양
현재까지 테스트는 엔비디아 사의 RTX 2080 Ti와 RTX타이탄을 주로 사용하였으며, 쿠다버전 또한 직접 테스트한 10.1 버전으로 진행합니다.

_2020년 07월 18일 기준 cuda10.1버전을 설치하여 테스트하였습니다._

# 설치방법
터미널을 실행 시킨 후 슈퍼유저 (sudo -E su)로 작업을 진행하는 것을 권장합니다.


파일을 받아둔 디렉토리로 이동하여 아래의 명령어로 실행을 시켜줍니다.

- ./nvidia_cuda10.1_setup.sh

만약 실행이 되지 않는다면 (chmod +x 파일명)명령어를 이용하여 실행권한을 주어 진행을 하시면됩니다.

그리고 실행이 정상적으로 끝났다면 재부팅을 권장합니다.

# 설치 확인
- 쿠다가 정상적으로 설치가 되셔서 재부팅까지 마쳤다면, 검색창에 **"NVIDIA X Server Settings"** 에서 정상적으로 그래픽카드가 인식이 되는지 확인을 권장드립니다.

- 터미널창에서는 **"nvidia-smi"** 명령어를 이용하여 설치된 쿠다의 버전과 그래픽카드 확인이 가능합니다.



For Ubuntu 18.04 version's Nvidia graphic Cuda 10.1

- When you setup this, then A graphic driver of the latest version will be installed.-
If you want to install another version, Move to Nvidia-driver Section and setup with it.
