# nighres


<details>
  <summary>nighres 설치 환경</summary>
  <br>
  <b>linux : 우분투 20.04.4LTS </b><br>
  <br>
  환경 구성에 pip이 필요하므로 다음 명령어를 사용하여 pip을 설치한다.<br>
  <code>sudo apt install python3-pip </code> <br>
  <br>
  Nighres를 설치하기 위해서는 다음의 세 조건이 만족해야한다. <br>
  
  * Python >= 3.5
  * Java JDK >= 1.7
  * JCC >= 3.0
  
  Nighres install 문서에 있는 Build Nighres 1번에 해당하는 방법(하단)으로 설치했다.<br>
  <code>sudo apt-get install openjdk-8-jdk </code><br>
  <code>export JCC_JDK=/usr/lib/jvm/java-8-openjdk-amd64</code><br>
  <code>python3 -m pip install jcc</code><br>
  <br>
  nighres를 사용하려면 numpy는 최대 1.16.4이어야 하는데, 이것이 Pandas와 Scipy의 높은 버전에서 맞지 않는다.<br>
  그리고 nilearn의 plotting을 사용하는데 필요한 matplotlib도 설치해주어야한다.<br>
  다음의 버전으로 설치하였다.<br>
  
  * Pandas == 1.1.0
  * Scipy == 1.4.0
  * matplotlib == 3.4.0
  * Numpy == 1.16.4
  
  pandas에서 버전이 맞지 않으면 numpy를 재설치하는 경우가 생길 수 있는데, 따라서 pandas와 scipy를 모두 재설치하고 난 후에 numpy를 재설치 하는 것이 좋다.<br>
  <code>pip install pandas==1.1.0</code><br>
  <code>pip install scipy==1.4.0</code><br>
  <code>pip install matplotlib==3.4.0</code><br>
  <code>pip install numpy==1.16.4</code><br>
  
  모든 설치를 마친 후 nighres와 nilearn을 설치한다.<br>
  <code>pip install nighres</code><br>
  <code>pip install -U --user nilearn</code><br>
</details>


7T 데이터.ipynb 는 데이터를 다운로드 하는 과정이 들어있는 파일입니다.
4layers와 10layers 폴더는 각각의 extracted_region 별로 Region Extraction, CRUISE, Volumetric layering의 과정이 정리된 파일들이 들어있습니다.
이 때, 4layers는 Volumetric layering의 layer 수가 4개, 10layers는 10개로 layer수의 차이를 비교하기 위해 

