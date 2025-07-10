<h1 align="center">📦 QRCode.Generator</h1>
<p align="center"><em>Transform Ideas into Instant, Shareable Visuals</em></p>

<p align="center">
  <img alt="Last Commit" src="https://img.shields.io/github/last-commit/LeoSOliveira0/qrcode.generator?style=for-the-badge" />
  <img alt="Java" src="https://img.shields.io/badge/Java-93.3%25-blue?style=for-the-badge&logo=java" />
  <img alt="Languages" src="https://img.shields.io/github/languages/count/LeoSOliveira0/qrcode.generator?style=for-the-badge" />
</p>

<p align="center"><em>Built with the tools and technologies:</em></p>

<p align="center">
  <img alt="Markdown" src="https://img.shields.io/badge/-Markdown-000?style=for-the-badge&logo=markdown" />
  <img alt="Docker" src="https://img.shields.io/badge/-Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />
  <img alt="XML" src="https://img.shields.io/badge/-XML-0060ac?style=for-the-badge&logo=xml&logoColor=white" />
</p>

---

## 🚀 Features

- 🧾 Generate QR codes from text or URLs
- ☁️ Uploads the generated image to Amazon S3
- 🧼 Clean architecture with domain-driven design
- 🔌 Easy to expand and maintain

---

## 🛠 Technologies

- Java 17
- Spring Boot 3
- Maven
- Amazon S3 (AWS SDK)
- Docker (optional for deployment)
- JUnit (tests)

---

## 📁 Project Structure

```
qrcode.generator/
├── controller/           # REST controllers
├── dto/                  # Data Transfer Objects
├── service/              # Business logic for QR generation
├── ports/                # Interfaces for abstraction
├── infrastructure/       # Concrete implementations (e.g., S3 adapter)
└── Application.java      # Spring Boot entry point
```

---

## 🔧 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/LeoSOliveira0/qrcode.generator.git
cd qrcode.generator
```

### 2. Set up AWS credentials

Make sure to configure your AWS credentials to access an S3 bucket.

### 3. Run the application

```bash
./mvnw spring-boot:run
```

Visit: `http://localhost:8080`

---

## 📡 API Usage

### `POST /api/qrcode/generate`

**Request Example:**

```json
{
  "text": "https://github.com/LeoSOliveira0"
}
```

**Response:**

```json
{
  "imageUrl": "https://s3.amazonaws.com/your-bucket-name/qr-code-id.png"
}
```

---

## 📄 License

Licensed under the [MIT License](LICENSE).

---

## 👤 Author

Made with ❤️ by [@LeoSOliveira0](https://github.com/LeoSOliveira0)
