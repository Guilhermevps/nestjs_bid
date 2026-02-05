# 🏛️ Bidding Search Engine (Buscador de Licitações)

[Portuguese version below](#português)

## 🌎 Overview

A robust and scalable API designed to aggregate and search Brazilian public bids. This project serves as a technical showcase for **Mid/Senior level** skills, focusing on performance, security, and maintainability using industry-best practices.

### 🚀 Key Technical Highlights

- **Distributed Rate Limiting:** Implemented with **Redis** to protect the infrastructure against scraping and DoS attacks.
- **Asynchronous Architecture:** Utilizing NestJS `forRootAsync` patterns to ensure secure environment variable loading.
- **Containerized Environment:** Fully orchestrated with **Docker**, ensuring consistency between development and production.
- **Clean Code & SOLID:** Developed with a focus on maintainability and decoupled logic.

### 🛠️ Tech Stack

- **Framework:** NestJS (Node.js)
- **Database:** PostgreSQL (TypeORM)
- **Cache/Security:** Redis
- **Infrastructure:** Docker & Docker Compose

---

## 🇧🇷 Português

### 📝 Descrição

Uma API robusta e escalável desenvolvida para agregar e buscar licitações públicas brasileiras. Este projeto funciona como um atestado técnico de nível **Pleno/Sênior**, com foco em performance, segurança e facilidade de manutenção.

### 🚀 Destaques Técnicos

- **Rate Limiting Distribuído:** Implementado com **Redis** para proteger a infraestrutura contra scrapers e ataques de DoS.
- **Arquitetura Assíncrona:** Uso de padrões `forRootAsync` do NestJS para garantir o carregamento seguro de variáveis de ambiente.
- **Ambiente Conteinerizado:** Orquestração completa via **Docker**, garantindo que o ambiente de dev seja idêntico ao de produção.
- **SOLID & Clean Code:** Foco em desacoplamento e facilidade de evolução do código.

---

## ⚙️ Setup & Installation / Instalação

### Prerequisites / Pré-requisitos

- Docker & Docker Compose
- Node.js (v18+)
- NPM or Yarn

### 1. Configure Environment / Configurar Variáveis

Copy the example file to `.env`:
`cp .env.example .env`

The `.env` file should look like this (default for Docker):
O arquivo `.env` deve seguir este modelo (padrão para o Docker):

```env
# Database Configuration
DB_HOST=localhost
DB_PORT=5432
DB_USERNAME=postgres
DB_PASSWORD=password_database
DB_DATABASE=local_database
DB_SYNCHRONIZE=true

# Redis Configuration
REDIS_HOST=localhost
REDIS_PORT=6379

# Environment
NODE_ENV=development
```

### 2. Run Infrastructure / Subir Infraestrutura

`docker-compose up -d`

### 3. Start Application / Iniciar Aplicação

```bash
npm install
npm run start:dev
```
