# timerActivities API
API  para gerenciar e cronometrar  tarefas usando PYTHON, FLASK e SWAGGER .

Acesse aqui  o github com um exemplo do front-end para a aplicação : https://github.com/morettonijose/timerActivities-frontEnd
 
## Requisitos

- Python 3.x
- pip (gerenciador de pacotes Python)

## Instalação


### 1. Clone o repositório

```bash
git clone https://github.com/morettonijose/timerActivities-API.git seu-repositorio
cd seu-repositorio
```



### 2.  Crie e ative um ambiente virtual



Verifique se tem o python instalado em seu terminal verificando a versão do Python   : 

**WINDOWS /linux**
```bash
python --version
```

**MAC OS**
```bash
python3 --version
```

 Se não tem o python instalado , acesse o link a seguir para instalar, e então reinicie o seu terminal.

Baixe e Instale aqui : https://www.python.org/downloads/ ; 

Após reiniciar o terminal, verifique novamente se  o python foi instalado verificando a versão do Python   : 

**WINDOWS /linux**
```bash
python —-version
```

**MAC OS**
```bash
python3 --version
```


Uma vez que você teve sucesso em verificar a versão do Phyton , você pode prosseguir com a intalação . 


#### WINDOWS / LINUX 
```bash
python -m venv venv
source venv/bin/activate
```


#### MAC OS
```bash
python3 -m venv venv
. venv/bin/activate
```






### 3.   Instale o PIP

Você também precisará do **pip** para gerenciar a instalação das bibliotecas necessárias ao projeto. 

verifique se o pip está instalado digitando o comando abaixo. 

#### WINDOWS/LINUX  
```bash
pip --version
```

#### MAC OS 
```bash
pip3 --version
```

Se você teve erro ao tentar executar o comando acima, então você precisa instalar o pip e após isto verificar novamente se o pip foi instalado.

#### WINDOWS/LINUX  
```bash
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
pip --version
```

#### MAC OS 
```bash
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
pip3 --version
```

Uma vez que você teve sucesso em verificar a versão do pip e que ele esta instalado , você pode prosseguir com a intalação da bibliotecas necessárias ao projeto. 






### 4.   Instale as bibliotecas necessárias

Verifique as bibliotecas atualmente instaladas.

#### WINDOWS/LINUX  
```bash
pip list
```

#### MAC OS 
```bash
pip3 list
```

Instale as bibliotecas necessárias ao projeto : 

#### WINDOWS/LINUX  
```bash
pip install -r static/requirements.txt
pip list
```


#### MAC OS  
```bash
pip3 install -r static/requirements.txt
pip3 list
```

Após este ponto você deverá ter recebido como retorno  a lista das bibliotecas instaladas. 
Certifique-se de que as seguintes bibliotecas estejam instaladas : 

Flask            
Flask-Cors       
Flask-RESTful     
Flask-SQLAlchemy  
flask-swagger-ui  
SQLAlchemy        


Se as bibliotecas foram listadas corretamente, você pode prosseguir para o próximo passo. 

Caso tenha tido problema neste passo, verifique as possiveis soluções na sessão de erros no final deste documento. 



### 5. Rodando o Projeto

**WINDOWS / LINUX**
```bash
python app.py
```

**MAC OS**
```bash
python3 app.py
```


### 6. PRONTO!! Sua instância foi ativada com sucesso

**Você receberá uma mensagem do tipo :**
```bash
 * Serving Flask app 'app'
 * Debug mode: on
WARNING: This is a development server. Do not use it in a production deployment. Use a production WSGI server instead.
 * Running on http://127.0.0.1:5000
Press CTRL+C to quit
 * Restarting with stat
 * Debugger is active!
 * Debugger PIN: 608-878-228
```

E então já  poderá acessar a API no endereço a seguir  : **http://127.0.0.1:5000/**  

Você não conseguirá visualizar a api diretamente na url acima pois não há nenhum endpoint no endereço principal da api .

Para visualizar a API e saber sobre os endpoints e  documentação, acessse o SWAGGER em seu navegador .

O link para o SWAGGER da documentação da api está a seguir  : **http://127.0.0.1:5000/swagger/**

A seguir você  encontrar o link do repositório github com um exemplo do front-end para a aplicação :  
**https://github.com/morettonijose/timerActivities-frontEnd**







### 7. Possíveis soluções de erros


#### **ERRO DE ESCRITA NO BANCO DE DADOS**

Caso tenha erro ao tentar executar a escrita no banco de dados deve-se verificar e corrigir a permissão de escrita do arquivo e respectivo diretorio, conforme a seguir :  

```bash
  * chmod 755 /instance
  * chmod 666 /instance/activities.db
  * chown seu_usuario:seu_grupo /instance/activities.db
```

 

**ERRO DE INSTALACAO DAS BIBLIOTECAS**

####  **Para instalar manualmente as Blibliotecas  Necessárias :**


**WINDOWS/LINUX :**
```bash

pip install  flask

pip install flask-restful

pip install flask-swagger-ui

pip install -U Flask-SQLAlchemy

pip  install flask-cors

//verifica bibliotecas instaladas no ambiente
pip list
```



 
**MAC OS :**

```bash
pip3 install Flask
  
pip3 install  flask

pip3 install flask-restful

pip3 install flask-swagger-ui

pip3 install -U Flask-SQLAlchemy

pip3  install flask-cors

//verifica bibliotecas instaladas no ambiente
pip3 list
```
 
**/////////////////////////////////////////////////////////////////**



