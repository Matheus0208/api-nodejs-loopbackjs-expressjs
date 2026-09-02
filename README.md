# Curso AWS Prático — API em 90 segundos

Este repositório é o resultado prático da **Aula 5** do curso **AWS na Prática**, do canal [Um Inventor Qualquer](https://www.youtube.com/c/UmInventorQualquer) no YouTube. Nele você encontra uma API REST completa, criada em poucos minutos com **LoopbackJS** (sobre **ExpressJS**), pronta para rodar em containers **Docker** com um banco de dados **MySQL**.

▶️ **Vídeo da aula:** [Criando uma API em 90 segundos | NodeJS com LoopbackJS/ExpressJS](https://youtu.be/bU4M9tZhsTs)
📺 **Playlist completa do curso:** [AWS na Prática](https://www.youtube.com/playlist?list=PLOF5f9_x-OYUaqJar6EKRAonJNSHDFZUm)

## Sobre o projeto

O objetivo desta aula é mostrar, na prática, como sair do zero até uma API funcional em pouquíssimo tempo, usando o gerador de aplicações do Loopback 4. O resultado é um CRUD de **Produtos** (`Product`), com model, repository, controller e datasource já configurados para MySQL, tudo rodando dentro de containers Docker.

## Estrutura do repositório

```
.
├── docker/           # Dockerfiles e scripts para build/execução do ambiente
├── www/
│   └── api/          # Código-fonte da API (LoopbackJS)
├── docker-compose.yml
└── README.md
```

Resumo dos recursos gerados:

- **App**: `api` (LoopbackJS 4, com ESLint, Prettier, Mocha, Docker e repositórios habilitados)
- **Datasource**: `mysql`, conectado ao container MySQL do ambiente Docker
- **Model**: `Product`, com as propriedades `id`, `name`, `category`, `cost` e `price`
- **Repository**: `ProductRepository`, usando `DefaultCrudRepository`
- **Controller**: `ProductController`, com CRUD REST completo exposto em `/products`

