# learning-heroku
Passo a passo para levantar uma aplicação em **python** no Heroku.

# Install & Login
Apenas é preciso fazer estas etapas uma vez.  

Instalação: `sudo snap install heroku --classic`  
Com heroku instalado você pode facilmente linkar um projeto existente ao site Heroku.

Login: `heroku login`  
Irá abrir uma janela para você confirmar o login.  

# Project Files
(considerando que você já possui um projeto Git o qual você deseja jogar na web)  

Arquivos importantes para python:  
  * runtime.txt
    * Heroku irá ler deste arquivo a versão de python que deve ser utilizada
  * requirements.txt
    * Heroku irá ler deste arquivo os pacotes a serem instalados no ambiente virtual

# Project Deploy

