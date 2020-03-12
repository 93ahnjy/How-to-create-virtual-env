# ubuntu 16.04에서 가상환경 만들고 pytorch 시작하기
<br><br>

### 1. Anaconda3 
http://sldofvge12.blogspot.com/2018/04/ubuntu-tensorflow-gpu-anaconda-pycharm.html
<br>추가로 source ~/.bashrc 하면 컴퓨터 reset 필요없이 바로 적용 가능<br>

뭔가 다운이 잘 안되면 다음을 통해 anaconda update 진행

```
conda update -n root conda
```

또는 cache 삭제

```
conda clean --all
```
------------------------------------------------------------------------------------
<br><br>

### 2. 가상환경 기본 사용법

https://niceman.tistory.com/85
<br>참고로 블로그와는 조금 다른게 'source'를 붙여야 하는 경우도 있다.<br><br>

```
conda create --name pytorch python=3.6
source activate pytorch
```


In most cases what you want to do when you say that you want to update Anaconda is to execute the command:
```
conda update --all
```



https://stackoverflow.com/questions/45197777/how-do-i-update-anaconda
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
<br>
<br> 참고로 terminal 계정이 root냐 아니냐에 따라서 계정에 따른 실행 가능 상황이 달라질 수 있으니 조심.
<br> pychram에 바로 갱신 되는 건 확인함.

-----------------------------------------------------------------------------
<br><br>



### 6. torchvision 설치
https://github.com/pytorch/vision
<br> pycharm기준 가상환경에서 pip로 설치하니깐 된다. conda로는 안되었음.<br><br>
```pip install torchvision```
<br> 
<br> update 19.4.15
<br><br> 알고 보니 그냥 Conda install로 다 설치가 가능했음.<br><br>
```conda install torchvision```


-----------------------------------------------------------------------------
<br><br>



### 7. matplotlib 설치
https://anaconda.org/conda-forge/matplotlib
<br> conda로 하는 것은 쓸데없는 짓이었다. 그냥 pip로 해야 됨. <br><br> 
```pip install matplotlib```
<br> 
<br><br> 알고 보니 그냥 Conda install로 다 설치가 가능했음.<br><br>
```conda install matplotlib```

-----------------------------------------------------------------------------
<br><br>



### 8. opencv 설치
https://anaconda.org/anaconda/libopencv
<br> python버전만인지, c++에서도 되는 건지는 모르겠다. <br><br> 
```
conda install -c anaconda libopencv
conda install -c anaconda py-opencv
```
<br> 
<br> 둘 다 설치한 상태인데 누구 덕에 되는 지는 잘 모르겠다. 
<br><br> 알고 보니 그냥 Conda install로 다 설치가 가능했음.<br><br>
``` conda install opencv ```


-----------------------------------------------------------------------------
<br><br>





### 주의점
<br> 절대 다운로드 중에는 잘못 받는 중이라도 뭘 건드리지 마라 절대. 
<br> pkg끼리 꼬이면 답도 없으며, python경우, link가 아예 broken까지 뜸

-----------------------------------------------------------------------------
<br><br>
