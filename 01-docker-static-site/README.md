# Site Estático com Docker

Este projeto tem como objetivo demonstrar conceitos fundamentais de Docker (Containerização de uma aplicação)

## Objetivos

- Demonstrar conhecimentos básicos de Docker
- Criar e executar uma imagem Docker do zero utilizando Nginx

## Estrutura

```text
.
├── index.html        
├── style.css         
└── Dockerfile        # Instruções de construção da imagem
```
## Funcionamento

Pré-requisitos
- Git instalado
- Docker desktop instalado e rodando

1. Clonar o repositório
Digite no terminal:
git clone [https://github.com/iszxsz/docker-to-kubernetes-lab.git](https://github.com/iszxsz/docker-to-kubernetes-lab.git)

Entre na pasta do projeto digitando no terminal:
cd docker-to-kubernetes-lab
cd 01-docker-static-site

2. Contruir a imagem Docker
No terminal digite:
docker build -t site-docker .

3. Executar o contâiner
No terminal digite:
docker run -d -p 8080:80 --name static-site site-docker

4. Acessar a aplicação
No navegador acesse: http://localhost:8080
