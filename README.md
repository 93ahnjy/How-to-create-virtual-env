# ubuntu 16.04에서 가상환경 만들기


### 1. Anaconda3 
http://sldofvge12.blogspot.com/2018/04/ubuntu-tensorflow-gpu-anaconda-pycharm.html
<br>추가로 source ~/.bashrc 하면 컴퓨터 reset 필요없이 바로 적용 가능<br>

------------------------------------------------------------------------------------
<br><br>

### 2. 가상환경 기본 사용법

https://niceman.tistory.com/85
<br>참고로 블로그와는 조금 다른게 'source'를 붙여야 하는 경우도 있다.<br>

-----------------------------------------------------------------------------
<br><br>


### 3. 가상환경 pycharm에 옮기기
setting --> project interpreter --> 톱니 --> add local --> /home/사용자/anaconda3/envs 에서 맞는 python 선택

-----------------------------------------------------------------------------
<br><br>

### 4. cudatoolkit 설치
https://anaconda.org/anaconda/cudatoolkit
<br>cuda9.0, cudnn7.3, numpy, tensorflow-gpu까지 싹다 깔린다.

-----------------------------------------------------------------------------

### 5. pytorch 설치
https://anaconda.org/search?q=platform%3Alinux-64+pytorch
<br> 여기서 원하는 버전으로 깔면 된다. cudatoolkit이랑 버전 안맞는 것은 자동으로 딴 놈으로 downgrade

-----------------------------------------------------------------------------
