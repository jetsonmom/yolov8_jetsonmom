# yolov8_jetsonmom 참  https://www.youtube.com/watch?v=pAEkHsNkul0,   https://velog.io/@kys5037k/jetson-nano-Python-3.8-ver-%EC%84%A4%EC%B9%98
image detection

jetpack 4.6.1
python 3.8.12

1. update & upgrade
   sudo apt update
   sudo apt upgrad
2. 필요한 패키지 설치
   sudo apt install build-essential libssl-dev zlib1g-dev libncurses5-dev libncursesw5-dev libreadline-dev libsqlite3-dev libgdbm-dev libdb5.3-dev libbz2-dev libexpat1-dev liblzma-dev libffi-dev libc6-dev
3. python3.8 소스코드 받기
   cd /
   wget https://www.python.org/ftp/python/3.8.12/Python-3.8.12.tar.xz
4  압축 풀기
   tar -xf Python-3.8.12.tar.xz
   cd Python-3.8.12
5. Build
   ./configure --enable-optimizations
   make -j4

6. 마무리
   sudo make altinstall
   python3.8 --version

7. 가상환경 (중요!!)
   python3.8 -m venv myenv                                     
   source myenv/bin/activate
