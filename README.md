# ubuntu 16.04에서 가상환경 만들고 pytorch 시작하기
<br><br>

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
<br>cuda9.0, cudnn7.3, numpy, tensorflow-gpu까지 싹다 깔린다.<br><br>
```conda install -c anaconda cudatoolkit```
<br> 

-----------------------------------------------------------------------------
<br><br>


### 5. pytorch 설치
https://anaconda.org/search?q=platform%3Alinux-64+pytorch
<br> 여기서 원하는 버전으로 깔면 된다. cudatoolkit이랑 버전 안맞는 것은 자동으로 딴 놈으로 downgrade<br><br>
<br>```conda install -c anaconda pytorch```<br><br>
 

https://pytorch.org/get-started/previous-versions/
<br> 이전 버전에서 conda 없이 깔려면 여기서 맞는 cuda 및 python버전의 whl 파일 설치.
<br> 그 담에는 pip3 install 'whl경로' 명령어를 쳐서 설치하면 된다. 
<br> 참고로 terminal 계정이 root냐 아니냐에 따라서 계정에 따른 실행 가능 상황이 달라질 수 있으니 조심.
<br> pychram에 바로 갱신 되는 

-----------------------------------------------------------------------------
<br><br>



### 6. torchvision 설치
https://github.com/pytorch/vision
<br> pycharm기준 가상환경에서 pip로 설치하니깐 된다. conda로는 안되었음.<br><br>
```pip install torchvision```
<br> 

-----------------------------------------------------------------------------
<br><br>



### 7. matplotlib 설치
https://anaconda.org/conda-forge/matplotlib
<br> 쓸데없는 짓이었다. 그냥 pip로 해야 됨. <br><br> 
```pip install matplotlib```
<br> 

-----------------------------------------------------------------------------
<br><br>
