# JoyFace - Facial expressions for controlling a wheelchair
Paper executável desenvolvido na disciplina IA369Z - Reprodutibilidade em Pesquisa Computacional - FEEC - Unicamp

In this work, we proposes the development of a human-computer interaction based on computer vision called JoyFace. It features a solution for people with motor disabilities such as cerebral palsy, muscular dystrophy, amyotrophic lateral sclerosis, cerebrovascular accident among others. It allows using a front camera already existing in most devices and controlling them through expressions or facial movements.A wheelchair simulation has also been developed and can be tested in real time on this executable paper.

See the Paper Preview here: https://github.com/suzanasvm/SmileFace/blob/master/deliver/SmileFace_052517_PaperPreviewV3.ipynb

See the PDF version of the Paper here: https://github.com/suzanasvm/SmileFace/blob/master/deliver/JoyFace_FACIAL%20EXPRESSIONS%20FOR%20CONTROLLING%20A%20WHEELCHAIR.pdf



# Montagem de Ambiente
A proposta deste paper executável é permitir que o usuário controle uma cadeira de rodas disponibilizada em um ambiente de simulação utilizando expressões faciais captadas pela webcam. 
Como pode ser visto no vídeo disponível https://www.youtube.com/watch?v=uzecwOaiKik

Para tanto o usuário deve possuir uma webcam ativa, a versão 2.7 do Python, a biblioteca OpenCV na versão 3.1.0 e o software de simulação V-Rep na versão Edu.

Abaixo temos as orientações para a montagem de ambiente em cada sistema operacional. Após instalar o ambiente necessário, o usuário deve abrir o software V-Rep e clicar em File > Open Scene e indicar o arquivo LCA.ttt que foi disponibilizado no github e no pacote de instalação. 

Feito isto, o usuário deverá abrir o jupyter notebook com o paper executável e utilizar a opção Cell > Run All para que o código seja executado por completo, após alguns segundos a seção anterior as References mostrará a webcam do usuário e estará pronta para controlar a cadeira de rodas da simulação V-Rep.
É ideal que o usuário disponibilize metade da tela para a exibição do V-Rep e a outra metade para o jupyter notebook.

# WINDOWS 10 - 64 BITS

<b>Conda:</b>  Foi utilizada a versão presente do Conda compatível com Python 2.7 que pode ser baixada através deste link https://conda.io/miniconda.html 
<br><b>OpenCV:</b> Foi utilizada a versão 3.1.0.3 da biblioteca openCV compatível com Python 2.7 A biblioteca pode ser baixada através do link: https://pypi.python.org/pypi/opencv-python/3.1.0.3 (opencv_python-3.1.0.3-cp27-cp27mu-manylinux1_x86_64.whl (md5)) 
<br>Abrir o prompt de comando do windows, utilizar o comando cd até chegar a pasta em que arquivo .whl se encontra, rodar o comando pip install opencv_python-3.1.0.3-cp27-cp27mu-manylinux1_x86_64.whl. 
<br><b>V-REP:</b> Software de Simulação utilizado. Um pacote para o Windows foi criado para facilitar a instalação das dependências do V-REP, disponível neste link: https://drive.google.com/open?id=0BzSRLfh3WveOMjMtd3NGb0ZNUUE. Caso utilize o pacote, os passos abaixos não necessitam ser seguidos.
<br>Caso não utilize o pacote de instalação, utilize o link para download do V-Rep http://www.coppeliarobotics.com/downloads.html utilizando a versão EDU. Os arquivos remoteApi.dll, vrep.py, vrepConst.py devem estar na mesma pasta do jupyter notebook a ser rodado.

# Ubuntu
<b>Conda:</b> Utilizar a versão Anaconda compatível com Python 2.7, que pode ser encontrada no link https://www.continuum.io/downloads 
Após o download abrir o terminal, utilizar o comando bash Anaconda2-4.4.0-Linux-x86_64.sh 
<br>Caso deseje, o usuário pode criar um enviroment para o paper executável utilizando os comandos: 
<br>Csource ~/.bashrc 
<br>Cconda create --name my_env python=2.7 
<br>Csource activate my_env 
<br><b>OpenCV:</b> Foi utilizada a versão 3.1.0.3 do openCV compatível com python 2.7 que pode ser encontrada no link: https://pypi.python.org/pypi/opencv-python/3.1.0.3 
<br><b>V-REP:</b> Software de Simulação utilizado. Pode ser baixado no link http://www.coppeliarobotics.com/downloads.html utilizando a versão EDU. Os arquivos vrep.py, vrepConst.py devem estar na mesma pasta do jupyter notebook a ser rodado.

# Mac OS
<b>Conda:</b>  Utilizar a versão Anaconda compatível com Python 2.7, que pode ser encontrada no link https://www.continuum.io/downloads 
<br><b>OpenCV:</b> Foi utilizada a versão 3.1.0.3 do openCV compatível com python 2.7 que pode ser encontrada no link: https://pypi.python.org/pypi/opencv-python/3.1.0.3 ou através do comando pip install opencv-python 
<br><b>V-REP:</b> Software de Simulação utilizado. Pode ser baixado no link http://www.coppeliarobotics.com/downloads.html utilizando a versão EDU. Os arquivos vrep.py, vrepConst.py devem estar na mesma pasta do jupyter notebook a ser rodado, mas se encontram disponíveis no pacote.


