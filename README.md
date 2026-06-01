# Docker Laravel

Ambiente Docker para aplicações Laravel utilizando Nginx, PHP-FPM e MySQL, projetado para desenvolvimento local e implantação padronizada.

## Visão Geral

Este projeto fornece uma stack completa para execução de aplicações Laravel em containers Docker. A arquitetura foi construída para oferecer isolamento de dependências, facilidade de configuração e consistência entre ambientes de desenvolvimento e homologação.

## Arquitetura

A stack é composta pelos seguintes serviços:

- Nginx
- PHP 7.4
- PHP-FPM 7.4
- MySQL 5.7.22

## Recursos

- Ambiente Laravel pronto para uso
- Containers isolados e reutilizáveis
- Nginx configurado como Web Server
- PHP-FPM para processamento das aplicações
- Banco de dados MySQL integrado
- Fácil personalização para novos projetos
- Integração com GitHub Actions

## Requisitos

- Docker
- Docker Compose
- Git

## Clone Repository

```bash
git clone https://github.com/<username>/docker-laravel.git

cd docker-laravel
```

## Build Environment

```bash
docker-compose build
```

## Start Services

```bash
docker-compose up -d
```

## Check Running Containers

```bash
docker ps
```

## Access Application

```bash
http://localhost
```

## Enter PHP Container

```bash
docker exec -it php-fpm bash
```

## Install Laravel Dependencies

```bash
composer install
```

## Generate Application Key

```bash
php artisan key:generate
```

## Run Database Migrations

```bash
php artisan migrate
```

## Stop Environment

```bash
docker-compose down
```

## Project Structure

```text
.
├── docker
├── nginx
├── php
├── mysql
├── docker-compose.yml
└── README.md
```

## GitHub Actions

O projeto possui suporte para integração contínua através do GitHub Actions, permitindo automatizar processos como:

- Build da aplicação
- Execução de testes
- Validação de código
- Deploy automatizado

Os workflows podem ser personalizados conforme a necessidade do projeto.

## Casos de Uso

- Desenvolvimento local de aplicações Laravel
- Ambientes de homologação
- Projetos corporativos
- Laboratórios e estudos
- Padronização de ambientes entre equipes

## Contribuição

Contribuições, correções e melhorias são bem-vindas.

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Open a Pull Request

## Licença

Este projeto está disponível sob a licença definida pelo mantenedor do repositório.
