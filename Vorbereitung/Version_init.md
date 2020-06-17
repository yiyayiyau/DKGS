# Halten gleichen Version: Plattform: Anaconda; Packets: python, scipy, numpy matplotlib, pandas, statsmodels, sklearn, opencv

um die gleiche version zu halten. Ich habe hier ein "environment.yml" beigefügt. Bitte folgends:
 
* Install Anaconda
* Copie **environment.yml** zu den Verzeichnis wo die Anaconda sind. z.B.: Bei mir **C:/hengwang/Anaconda3** , dann **C:/hengwang/enviroment.yml**
* Öffnen "Anaconda Prompt" und den Befehl geben: **conda env create -f environment.yml**
 Es wird automatisch ein enviroment "ml" erzeugen, darin wird numpy, scipy, matplotlib, pandas,statsmodels,sklearn, und opencv2 und opencv contrib installieren.

Du kannst in "Anaconda Prompt" den Befehl:
**activate ml**   activate the env. ml und dann 
**conda list scipy** eingeben um die scipy version zu gucken. 
**conda list numpy** und so weiter
die entsprechend Version sind folgendes: 

scipy: 1.4.1
numpy: 1.18.1
matplotlib: 3.1.3
pandas: 1.0.3
statsmodels: 0.11.1
sklearn: 0.22.1 
opencv-contrib-python 4.2.0.34 (Befehl: **conda list opencv**)


Erganzung:
	pip install PIL
	caffe
	Spyder
1 工具清单
2 安装/更新nvida驱动
3 安装cuda
4 安装cudnn
5 安装Anaconda
6 安装tensorflow-gpu
7 安装keras
8 检验tensorflow+keras环境