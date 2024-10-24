### yolo 가상환경 만들기

 -yolo (You Only Look Once)는 실시간 객체 탐지 알고리즘으로, 이미지나 비디오에서 여러 객체를 한 번에 빠르게 탐지하는 방식이다. 객체의 위치와 종류를 동시에 예측하고 다른 모델보다 효율적이고 속도가 빠른 것이 특징이다.
 
##### yolo 가상환경 만들기
    uname -a
    wget https://github.com/Archiconda/build-tools/releases/download/0.2.3/Archiconda3-0.2.3-Linux-aarch64.sh
    sudo chmod 755 Archiconda3-0.2.3-Linux-aarch64.sh
    ls
##### 결과

  Archiconda3-0.2.3-Linux-aarch64.sh Pictures Desktop Public Documents Templates Downloads Videos examples.desktop yolov8_4gb Music

     ./Archiconda3-0.2.3-Linux-aarch64.sh
실행 중 선택이라 뜨면
yes---> enter ---> yes in your /home/ldh/.bashrc ? [yes|no] [no] >>> yes
이렇게 한다.

    conda env list
    conda activate base
    jetson_release 

    
### python 3.8 가상환경 만들기
***
base가 아닌 native에서 실행

    conda create -n yolo python=3.8 -y
    conda env list

    conda activate yolo
    
 - "conda activate yolo"를 실행하여 yolo 가상환경으로 진입해서 pytorch, torchvosion을 설치하는 과정이다.
 - 결과 가상에서 설치 torch, torvosion 다운로드
(yolo) dli@dli:~$
