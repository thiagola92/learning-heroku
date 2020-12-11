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
`heroku create`  
Esse comando por si já levanta seu projeto na web (se nenhum nome for especificado, um nome aleatório é gerado). Neste caso foi gerado um projeto com nome pacific-shelf-08133  

URL para a aplicação:  
https://pacific-shelf-08133.herokuapp.com/  

A branch em que o heroku trabalha se chama **heroku**  
Para levantar qualquer mudança para sua aplicação web você deve alterar a branch heroku e atualizar ela com  
`git push heroku main`  

Se você tentar atualizar sua aplicação sem especificar a linguagem utilizada, heroku irá tentar identificar a linguagem e configurar para você, porém caso ele não consiga você deve configurar na mão  
`heroku buildpacks:set heroku/python`  

# Referências
https://devcenter.heroku.com/articles/python-runtimes  
https://devcenter.heroku.com/articles/buildpacks    