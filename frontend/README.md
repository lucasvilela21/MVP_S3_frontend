# Meu Front

Projeto de MVP para conclusão do Sprint 3 da Pós Graduação em Engenharia de Software pela PUC-RIO.

Projeto com finalidade de cadastrar Artesões e Vendas dos Artesões, para futuro uso em uma feira de voluntários da APAE de 
Mogi das Cruzes.

---
## Como executar em modo de desenvolvimento

Basta fazer o download do projeto e abrir o arquivo index.html no seu browser.

## Como executar através do Docker

Certifique-se de ter o [Docker](https://docs.docker.com/engine/install/) instalado e em execução em sua máquina.

Navegue até o diretório que contém o Dockerfile no terminal e seus arquivos de aplicação e
Execute **como administrador** o seguinte comando para construir a imagem Docker:

```
$ docker build --pull --rm -f "frontend\Dockerfile" -t mvpfrontend "frontend" 
```

Uma vez criada a imagem, para executar o container basta executar, **como administrador**, seguinte o comando:

```
$ docker run -d -p 8080:80 mvpfrontend
```

Uma vez executando, para acessar o front-end, basta abrir o [http://localhost:8080/#/](http://localhost:8080/#/) no navegador.

## API Externa

Foi utilizado a API externa Currency Exchange (https://rapidapi.com/fyhao/api/currency-exchange). Tem como objetivo fornecer cotações de diversas moedas em tempo real.
Não possui licença e foi utilizado as seguintes API-Key e API-Host:
'X-RapidAPI-Key': '4ef470d2a0mshc6208929ad76353p1cd7c9jsn001071105199',
'X-RapidAPI-Host': 'currency-exchange.p.rapidapi.com'
Foi utilizado o metodo GET.