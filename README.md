# Minha API em REST

Projeto parte da disciplina de **Desenvolvimento Full Stack Avançado** - PUC Rio

O objetivo aqui é apresetar uma API em REST (componente C), que interage com o Front-End (componente A) e uma API externa (componente B).

---
## Como executar

1. Clonar o repositório;
2. Instalar as libs python listadas em **requirements.txt**;
3. Excecutar os comandos abaixo pelo terminal (recomendado o uso de venv).

Para instalar as libs:

``` $ pip3 install -r requirements.txt ```

Para executar a API:

``` $ flask run --host 0.0.0.0 --port 5000 ```

Para reiniciar o servidor após uma mudança no código (modo de desenvolvimento):

``` $ flask run --host 0.0.0.0 --port 5000 --reload ```

Para conferir o status da API, abra o http://localhost:5000/#/ no navegador!

---
## Como executar através do Docker

1. Instalar o [Docker](https://docs.docker.com/engine/install/) em sua máquina;
2. Naveguar até o diretório que contém os arquivos **Dockerfile.txt** e **requirements.txt** terminal.
3. Execute **como administrador** o comando a seguir para criar a imagem:

``` $ docker build --pull --rm -f "componenteC/Dockerfile.txt" -t mvp2:latest "componenteC" ```

Para executar o container:

``` $ docker run -p 5000:5000 mvp2 ```

Para conferir o status da API, abra o http://localhost:5000/#/ no navegador!
