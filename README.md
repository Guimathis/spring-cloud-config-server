# Spring Cloud Config Server

Este servidor centraliza as configurações de todos os microserviços do ecossistema.

## Configuração

O servidor está configurado para buscar arquivos de configuração em um repositório Git (ou diretório local simulando um repositório).

- **Porta:** 8888
- **Repositório Configurado:** `https://github.com/Guimathis/spring-cloud-configs`
- **Caminho de Busca:** `greeting-service*`

## Como acessar as configurações

Você pode visualizar as configurações carregadas acessando as seguintes URLs no navegador:

- **Greeting Service (Default):** `http://localhost:8888/greeting-service/default`
- **Greeting Service (Português):** `http://localhost:8888/greeting-service/pt`
- **Greeting Service (Inglês):** `http://localhost:8888/greeting-service/en`

## Como Executar

Execute o comando na pasta raiz do servidor:
```bash
mvn spring-boot:run
```
