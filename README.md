# JoyFace - Facial expressions for controlling a wheelchair
Paper executável desenvolvido na disciplina IA369Z - Reprodutibilidade em Pesquisa Computacional - FEEC - Unicamp

In this work, we proposes the development of a human-computer interaction based on computer vision called JoyFace. It features a solution for people with motor disabilities such as cerebral palsy, muscular dystrophy, amyotrophic lateral sclerosis, cerebrovascular accident among others. It allows using a front camera already existing in most devices and controlling them through expressions or facial movements.A wheelchair simulation has also been developed and can be tested in real time on this executable paper.

See the Executable Paper here: https://github.com/suzanasvm/SmileFace/blob/master/deliver/JoyFace_ExecutablePaper.ipynb

See the PDF version of the Paper here: https://github.com/suzanasvm/SmileFace/blob/master/deliver/JoyFace_FACIAL%20EXPRESSIONS%20FOR%20CONTROLLING%20A%20WHEELCHAIR.pdf

# Montagem de Ambiente
A proposta deste paper executável é permitir que o usuário controle uma cadeira de rodas disponibilizada em um ambiente de simulação utilizando expressões faciais captadas pela webcam. 
Como pode ser visto no vídeo disponível https://www.youtube.com/watch?v=uzecwOaiKik

Primeiramente faça o download do repositório do projeto, utilize o comando: 
<br>git clone https://github.com/suzanasvm/SmileFace

Para reproduzir este projeto você de possuir:
 - Uma webcam 
 - Python na versão 2.7
 - Biblioteca OpenCV na versão 3.1.0
 - Biblioteca Matplot na versão 2.0.2 
 - Software de Simulação V-Rep na modalidade Edu.

Abaixo temos as orientações para a montagem de ambiente em cada sistema operacional. Após instalar o ambiente necessário, o usuário deve abrir o software V-Rep e clicar em File > Open Scene e indicar o arquivo LCA.ttt que foi disponibilizado no github na pasta /deliver/VRep.

Feito isto, o usuário deverá abrir o jupyter notebook com o paper executável e utilizar a opção Cell > Run All para que o código seja executado por completo, após alguns segundos observe ao fim da seção Anexes, o feedback da webcam em tempo real e você estará pronto para controlar com seu próprio rosto, a cadeira de rodas disponível na simulação do V-Rep.
É ideal que o usuário disponibilize metade da tela para a exibição do V-Rep e a outra metade para o jupyter notebook.

# WINDOWS
<br><b> Pacote de Instalação:</b>
<br>Foi criado um pacote de instalação para o ambiente Linux com todas as dependências necessárias. 
<br> Disponível no link: https://drive.google.com/open?id=0BzSRLfh3WveOMjMtd3NGb0ZNUUE
<br> Baixe o pacote 

<br><b> Instalação Manual:</b>
<b>Conda:</b>  Foi utilizada a versão presente do Conda compatível com Python 2.7 que pode ser baixada através deste link https://conda.io/miniconda.html 
<br><b>OpenCV:</b> Foi utilizada a versão 3.1.0.3 da biblioteca openCV compatível com Python 2.7 
<br>A biblioteca pode ser baixada através do link: https://pypi.python.org/pypi/opencv-python/3.1.0.3 (opencv_python-3.1.0.3-cp27-cp27mu-manylinux1_x86_64.whl (md5)) 
<br>Abrir o prompt de comando do windows, utilizar o comando cd até chegar a pasta em que arquivo .whl se encontra, rodar o comando pip install opencv_python-3.1.0.3-cp27-cp27mu-manylinux1_x86_64.whl. 
<br><b>Matplotlib</b> Foi utilizada a versão 2.0.2 da biblioteca, utilize o comando: conda install -c conda-forge matplotlib=2.0.2 para a instalação.
<br><b>V-REP:</b> Software de Simulação utilizado. Um pacote para o Windows foi criado para facilitar a instalação das dependências do V-REP, disponível neste link: https://drive.google.com/open?id=0BzSRLfh3WveOMjMtd3NGb0ZNUUE. Caso utilize o pacote, os passos abaixos não necessitam ser seguidos.
<br>Caso não utilize o pacote de instalação, utilize o link para download do V-Rep http://www.coppeliarobotics.com/downloads.html utilizando a versão EDU. 
<br>Acesse no repositório git a pasta deliver/VRep/Windows e copie os arquivos qwindows.dll e remoteApi.dll para a mesma pasta do arquivo JoyFace_ExecutablePaper.ipynb

# Ubuntu
<b>Conda:</b> Utilizar a versão Anaconda compatível com Python 2.7, que pode ser encontrada no link https://www.continuum.io/downloads 
Após o download abrir o terminal, utilizar o comando bash Anaconda2-4.4.0-Linux-x86_64.sh 
<br>Caso deseje, o usuário pode criar um enviroment para o paper executável utilizando os comandos: 
<br>conda create --name SEUNOMEDEAMBIENTE
<br>Acesse o ambiente criado com o comando: conda activate SEUNOMEDEAMBIENTE 
<br><b>OpenCV:</b> Foi utilizada a versão 3.1.0.3 do openCV compatível com python 2.7 que pode ser instalada através do comando: conda install -c wheeler-microfluidics opencv-python=3.1.0.3
<br><b>Matplotlib</b> Foi utilizada a versão 2.0.2 da biblioteca, pode ser utilizando o comando conda install -c conda-forge matplotlib=2.0.2 para a instalação.
<br><b>V-REP:</b> Software de Simulação utilizado. Pode ser baixado no link http://www.coppeliarobotics.com/downloads.html utilizando a versão EDU. 
<br> Após o download do V-REP descompacte a pasta. Feito isso utilize o terminal do Ubuntu para navegar até a pasta descompactada, execute o comando ./vrep.sh para rodar o V-REP.
<br>Acesse no repositório git a pasta deliver/VRep/Linux e acesse a pasta 32Bit ou 64Bit de acordo com as configurações da sua máquina
copie o arquivo remoteApi.so e cole na mesma pasta do arquivo JoyFace_ExecutablePaper.ipynb

# Mac OS
<b>Conda:</b>  Utilizar a versão Anaconda compatível com Python 2.7, que pode ser encontrada no link https://www.continuum.io/downloads 
<br><b>OpenCV:</b> Foi utilizada a versão 3.1.0.3 do openCV compatível com python 2.7 que pode ser encontrada no link: https://pypi.python.org/pypi/opencv-python/3.1.0.3 ou através do comando pip install opencv-python 
<br><b>Matplotlib</b> Foi utilizada a versão 2.0.2 da biblioteca, pode ser utilizando o comando conda install -c conda-forge matplotlib=2.0.2 para a instalação.
<br><b>V-REP:</b> Software de Simulação utilizado. Pode ser baixado no link http://www.coppeliarobotics.com/downloads.html utilizando a versão EDU. Os arquivos vrep.py, vrepConst.py devem estar na mesma pasta do jupyter notebook a ser rodado, mas se encontram disponíveis no pacote.

# Outra Alternativa: Imagem Docker

Baixar o Docker e utilizar a imagem disponível em: https://hub.docker.com/r/patavee/scipy-matplotlib-opencv/
<br>Executando o comando docker pull patavee/scipy-matplotlib-opencv
<br>Verificar se a imagem está disponível utilizando o comando docker images
<br>Para rodar a imagem, utilize o comando:	docker run -d -p 8888:8888 scipy-matplotlib-opencv

Após subir a imagem docker, verifique seu sistema operacional e siga as intruções de instalação do software de simulação V-Rep


