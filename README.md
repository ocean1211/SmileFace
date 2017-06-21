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
<b> Pacote de Instalação:</b>
<br>Foi criado um pacote de instalação para o ambiente Windows com todas as dependências necessárias. 
<br> Disponível no link: https://drive.google.com/open?id=0BzSRLfh3WveOMjMtd3NGb0ZNUUE
<br> Baixe o pacote de instalação e descompacte-o, execute o arquivo Setup SmileFace.exe 

<br><b> Instalação Manual:</b>
<br><b>Conda:</b>  Foi utilizada a versão do Conda compatível com Python 2.7 que pode ser baixada através deste link https://conda.io/miniconda.html 
<br><b>OpenCV:</b> Foi utilizada a versão 3.1.0.3 da biblioteca openCV compatível com Python 2.7 
<br>A biblioteca pode ser baixada através do link: https://pypi.python.org/pypi/opencv-python/3.1.0.3 (opencv_python-3.1.0.3-cp27-cp27mu-manylinux1_x86_64.whl (md5)) 
<br>Abrir o prompt de comando do windows, utilizar o comando cd até chegar a pasta em que arquivo .whl se encontra, rodar o comando pip install opencv_python-3.1.0.3-cp27-cp27mu-manylinux1_x86_64.whl. 
<br><b>Matplotlib</b> Foi utilizada a versão 2.0.2 da biblioteca, utilize o comando: conda install -c conda-forge matplotlib=2.0.2 para a instalação.
<br><b>V-REP:</b> Software de Simulação utilizado. Faça download do V-Rep http://www.coppeliarobotics.com/downloads.html utilizando a versão EDU. 
<br>Acesse a pasta deliver/VRep/Windows e ali escolha 32Bit ou 64Bit de acordo com as configurações da sua máquina e copie os arquivos qwindows.dll e remoteApi.dll para a mesma pasta do arquivo JoyFace_ExecutablePaper.ipynb

# Ubuntu
<b>Conda:</b> Utilizar a versão Anaconda compatível com Python 2.7, que pode ser encontrada no link https://www.continuum.io/downloads 
<br>Após o download abrir o terminal, utilizar o comando bash Anaconda2-4.4.0-Linux-x86_64.sh 
<br>Caso deseje, o usuário pode criar um enviroment para o paper executável utilizando os comandos: 
<br>conda create --name SEUNOMEDEAMBIENTE
<br>Acesse o ambiente criado com o comando: conda activate SEUNOMEDEAMBIENTE 
<br><b>OpenCV:</b> Foi utilizada a versão 3.1.0.3 do openCV compatível com python 2.7 que pode ser instalada através do comando: conda install -c wheeler-microfluidics opencv-python=3.1.0.3
<br><b>Matplotlib</b> Foi utilizada a versão 2.0.2 da biblioteca, pode ser utilizando o comando conda install -c conda-forge matplotlib=2.0.2 para a instalação.
<br><b>V-REP:</b> Software de Simulação utilizado. Pode ser baixado no link http://www.coppeliarobotics.com/downloads.html utilizando a versão EDU. 
<br> Após o download do V-REP descompacte a pasta. Feito isso utilize o terminal do Ubuntu para navegar até a pasta descompactada, execute o comando ./vrep.sh para rodar o V-REP.
<br>Acesse a pasta deliver/VRep/Linux e escolha a pasta 32Bit ou 64Bit de acordo com as configurações da sua máquina
copie o arquivo remoteApi.so e cole na mesma pasta do arquivo JoyFace_ExecutablePaper.ipynb

# Mac OS
<b>Conda:</b>  Utilizar a versão Anaconda compatível com Python 2.7, que pode ser encontrada no link https://www.continuum.io/downloads 
<br><b>OpenCV:</b> Foi utilizada a versão 3.1.0.3 do OpenCV compatível com python 2.7 que pode ser encontrada no link: https://pypi.python.org/pypi/opencv-python/3.1.0.3 ou através do comando pip install opencv-python 
<br><b>Matplotlib</b> Foi utilizada a versão 2.0.2 da biblioteca, pode ser utilizando o comando conda install -c conda-forge matplotlib=2.0.2
<br><b>V-REP:</b> Software de Simulação utilizado. Pode ser baixado no link http://www.coppeliarobotics.com/downloads.html utilizando a versão EDU.
<br>Acesse a pasta deliver/VRep/MacOS e copie o arquivo remoteApi.dylib e cole na mesma pasta do arquivo JoyFace_ExecutablePaper.ipynb

# EXECUTANDO O PAPER

1. Abra o V-REP e utilize a simulação disponibilizada. No V-REP clicar em File > Open Scene e indicar o arquivo LCA.ttt que foi disponibilizado na pasta /deliver/VRep.

2. Inicie o jupyter através do comando: jupyter notebook. Indique a pasta /deliver e abra o arquivo JoyFace_ExecutablePaper.ipynb

3. No notebook do paper executável utilize a opção Cell > Run All para que o código seja executado por completo.

4. Divida a tela do computador de tal forma que seja possível visualizar a simulação do V-Rep e o notebook do paper ao mesmo tempo. Observe na seção de anexos, o feedback da web cam e controle a cadeira de rodas disponível na simulação V-REP.

