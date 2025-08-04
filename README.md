<h1 align="center">📦 QRCode.Generator</h1>

<p align="center">
  <img alt="Último Commit" src="https://img.shields.io/github/last-commit/LeoSOliveira0/qrcode.generator?style=for-the-badge" />
  <img alt="Java" src="https://img.shields.io/badge/Java-93.3%25-blue?style=for-the-badge&logo=java" />
  <img alt="Linguagens" src="https://img.shields.io/github/languages/count/LeoSOliveira0/qrcode.generator?style=for-the-badge" />
</p>

<p align="center">
  <img alt="Java" src="https://img.shields.io/badge/-Java-007396?style=for-the-badge&logo=openjdk&logoColor=white" />
  <img alt="Spring Boot" src="https://img.shields.io/badge/-Spring_Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" />
  <img alt="Docker" src="https://img.shields.io/badge/-Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img alt="AWS" src="https://img.shields.io/badge/-AWS-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white" />
</p>

---

## 🚀 Funcionalidades

- 🧾 Gera códigos QR a partir de texto ou URLs
- ☁️ Faz upload da imagem gerada para o Amazon S3
- 🧼 Arquitetura limpa com design orientado ao domínio (DDD)

---

## 🛠 Tecnologias Utilizadas

- Java 17  
- Spring Boot 3  
- Maven  
- Amazon S3 (AWS SDK)  
- Docker (opcional para deploy)  

---

## 📁 Estrutura do Projeto

```
qrcode.generator/
├── controller/           # Controladores REST
├── dto/                  # Objetos de Transferência de Dados
├── service/              # Lógica de negócio para geração de QR Code
├── ports/                # Interfaces para abstração
├── infrastructure/       # Implementações concretas (ex.: adaptador S3)
└── Application.java      # Ponto de entrada do Spring Boot
```

---

## 🔧 Como Começar

### 1. Clone o repositório

```bash
git clone https://github.com/LeoSOliveira0/qrcode.generator.git
cd qrcode.generator
```

### 2. Configure as credenciais da AWS

Certifique-se de configurar suas credenciais da AWS para acessar um bucket S3.

### 3. Execute a aplicação

```bash
./mvnw spring-boot:run
```

Acesse: `http://localhost:8080`

---

## 📡 Uso da API

### `POST /api/qrcode/generate`

**Exemplo de Requisição:**

```json
{
  "text": "https://github.com/LeoSOliveira0"
}
```

**Resposta:**

```json
{
  "imageUrl": "https://s3.amazonaws.com/seu-nome-do-bucket/qr-code-id.png"
}
```

---
