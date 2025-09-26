
# Stock Management

Este projeto é uma aplicação full-stack desenvolvida com Ruby on Rails no backend e Vue.js 3 no frontend, implementando arquiteturas robustas e escaláveis em ambas as camadas.




## Stack utilizada

**Front-end:** Vue.js, Pinia, Axios, Bootstrap e Vue3-Toastfy

**Back-end:** Rails, JWT authentication e Dry Validation

**Database:** PostgreSQL

**Setup:** Docker


## Aprendizados

Este projeto representa um marco significativo na minha jornada como desenvolvedor, sendo minha primeira aplicação considerada verdadeiramente robusta com uma arquitetura em camadas bem definida. Pude finalmente colocar em prática conceitos que até então conhecia apenas teoricamente, como os padrões Service e Repository, que implementei para distribuir responsabilidades de forma mais organizada. Uma das principais conquistas foi conseguir atribuir tarefas específicas para cada camada, evitando aqueles controllers ou services que acumulam múltiplas responsabilidades. Outro grande avanço foi minha primeira experiência completa com Docker: se antes eu apenas subia containers prontos, desta vez enfrentei o desafio de arquitetar e configurar todo o ambiente do zero, o que me deu uma compreensão muito mais profunda de containerização e orquestração de ambientes.

## Backend - Rails com Arquitetura Aprimorada MVC

Fluxo de Requisição:

Routes → Controller → Service → Validator (← Retorno) → Repository → Database (← Retorno)

Com relação ao backend, foi especialmente enriquecedor implementar pela primeira vez métodos avançados de tratamento de concorrência, como locks, para garantir a integridade dos dados em operações críticas. Além disso, integrei ao projeto um sistema de Jobs para processamento assíncrono, Esses eram conceitos que eu já dominava teoricamente, mas que só pude compreender verdadeiramente sua complexidade e importância ao aplicá-los em um cenário real, enfrentando e solucionando os desafios práticos que surgiram durante a implementação.




## Frontend - Vue.js com Arquitetura Modular

Estrutura Hierárquica:

View → Module → Service → API

No front-end, busquei implementar uma componentização eficiente e estratégica, focando não apenas na reutilização de código, mas principalmente na criação de componentes com baixo acoplamento e alta coesão. Essa abordagem foi pensada para facilitar significativamente a implementação de testes automatizados, já que componentes independentes e bem delimitados em suas responsabilidades permitem testes mais isolados, previsíveis e de mais fácil manutenção.
## Futuras Melhorias

Como melhorias futuras para o projeto, pretendo focar em três áreas principais de evolução. Primeiramente, a implementação de testes automatizados tanto no frontend quanto no backend é uma prioridade, criando uma suíte robusta que garanta a confiabilidade e a manutenibilidade do código. Em segundo lugar, planejo realizar refatorações estratégicas em alguns services, buscando aplicar princípios de código limpo para torná-los mais coesos, legíveis e de fácil manutenção. Por fim, quero explorar mais conceitos avançados do backend, como a implementação de WebSockets para funcionalidades em tempo real, além de aprofundar conhecimentos em otimização de performance, caching e padrões arquiteturais mais complexos que possam elevar ainda mais a qualidade e a escalabilidade da aplicação.


## Instalação

Para executar o projeto em sua máquina local, siga os passos abaixo:

Pré-requisito: É necessário ter o Docker instalado em seu sistema. Caso ainda não possua, você pode baixá-lo em docker.com

```bash
  git clone https://github.com/Raphael-Maximowski/stock-management-docker.git
  cd stock-management-docker
  git submodule update --init --recursive
  docker compose build
  docker compose up
```
    