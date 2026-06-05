# Minisource

**Modern microservices platform built with Go, .NET, and Next.js**

Minisource is a comprehensive microservices ecosystem providing authentication, storage, notifications, payments, and more. All services are designed for scalability, observability, and developer productivity.

---

## 🚀 Core Services

### Security & Identity
- **[auth](https://github.com/minisource/auth)** - Authentication and authorization service (JWT, OAuth, users)  
  🌐 [auth.minisource.ir](https://auth.minisource.ir)

### API & Gateway
- **[gateway](https://github.com/minisource/gateway)** - API gateway and edge routing for all services  
  🌐 [gateway.minisource.ir](https://gateway.minisource.ir)

### Data & Storage
- **[storage](https://github.com/minisource/storage)** - Object and file storage service (S3-compatible)  
  🌐 [storage.minisource.ir](https://storage.minisource.ir)

- **[log](https://github.com/minisource/log)** - Centralized logging and log aggregation  
  🌐 [log.minisource.ir](https://log.minisource.ir)

### Communication
- **[notifier](https://github.com/minisource/notifier)** - Notification service for emails, SMS, and push notifications  
  🌐 [notifier.minisource.ir](https://notifier.minisource.ir)

- **[comment](https://github.com/minisource/comment)** - Comment service with moderation  
  🌐 [comment.minisource.ir](https://comment.minisource.ir)

### Content & User Engagement
- **[cms](https://github.com/minisource/cms)** - Content Management System and blog platform  
  🌐 [cms.minisource.ir](https://cms.minisource.ir)

- **[feedback](https://github.com/minisource/feedback)** - Feedback collection and survey backend  
  🌐 [feedback.minisource.ir](https://feedback.minisource.ir)

- **[ticket](https://github.com/minisource/ticket)** - Support ticket and helpdesk system  
  🌐 [ticket.minisource.ir](https://ticket.minisource.ir)

### Background Processing
- **[scheduler](https://github.com/minisource/scheduler)** - Distributed job scheduler and cron service  
  🌐 [scheduler.minisource.ir](https://scheduler.minisource.ir)

### Commerce
- **[payment](https://github.com/minisource/payment)** - Payment processing and gateway integration  
  🌐 [payment.minisource.ir](https://payment.minisource.ir)

---

## 🛠️ SDKs & Libraries

### Go Ecosystem
- **[go-sdk](https://github.com/minisource/go-sdk)** - Go SDK with clients for all Minisource services
- **[go-common](https://github.com/minisource/go-common)** - Shared Go utilities, helpers, and libraries
- **[go-template](https://github.com/minisource/go-template)** - Go project template with best practices

### .NET Ecosystem
- **[csharp-sdk](https://github.com/minisource/csharp-sdk)** - C# SDK and client libraries
- **[csharp-common](https://github.com/minisource/csharp-common)** - Shared C# utilities and helpers

---

## 📦 Templates & Tools

- **[front-template](https://github.com/minisource/front-template)** - Next.js 15 + shadcn/ui + Tailwind template  
  Modern frontend starter with TypeScript, Zustand, TanStack Query, Docker, and CI/CD

- **[infra](https://github.com/minisource/infra)** - Infrastructure-as-code, Terraform modules, and deployment scripts  
  🌐 [infra.minisource.ir](https://infra.minisource.ir)

- **[doc](https://github.com/minisource/doc)** - Documentation site and content  
  🌐 [doc.minisource.ir](https://doc.minisource.ir)

---

## 🏗️ Tech Stack

| Layer | Technologies |
|-------|-------------|
| **Backend** | Go, .NET 8, Node.js |
| **Frontend** | Next.js 15, React 19, TypeScript |
| **UI** | shadcn/ui, Tailwind CSS |
| **State** | Zustand, TanStack Query |
| **Database** | PostgreSQL, Redis |
| **Message Queue** | RabbitMQ, Kafka |
| **Storage** | MinIO (S3), Azure Blob |
| **Observability** | Prometheus, Grafana, Loki |
| **Infrastructure** | Docker, Kubernetes, Terraform |
| **CI/CD** | GitHub Actions |
| **Container Registry** | [Docker Hub (`minisource`)](https://hub.docker.com/orgs/minisource/repositories) |

---

## 📖 Getting Started

Each repository contains:
- 📄 Comprehensive README with setup instructions
- 🐳 Docker Compose for local development
- ⚙️ CI/CD workflows with GitHub Actions (build → push to Docker Hub on `main`)
- 🔒 Security policy and vulnerability reporting
- 🧪 Unit and integration tests

### Quick Start Example

```bash
# Clone a service
git clone https://github.com/minisource/auth
cd auth

# Run with Docker Compose
docker-compose up -d

# Or run natively
make run
```

### Docker Hub CI/CD

Service images are built by GitHub Actions and pushed to Docker Hub after a successful build on the default branch. Configure these repository secrets:

- `DOCKERHUB_USERNAME` — Docker Hub username or organization
- `DOCKERHUB_TOKEN` — Docker Hub access token

```bash
# Pull and run a production image
docker pull minisource/auth:latest
export TAG=latest
docker compose -f docker-compose.prod.yml up -d
```

---

## 🤝 Contributing

We welcome contributions! Please check each repository's `CONTRIBUTING.md` for guidelines.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'feat: add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 🔒 Security

Found a security vulnerability? Please **DO NOT** open a public issue.  
Email us at: **security@minisource.ir**

See our [Security Policy](https://github.com/minisource/.github/blob/main/SECURITY.md) for details.

---

## 📝 License

All Minisource projects are licensed under the MIT License unless otherwise specified.

---

## 📬 Contact

- 🌐 Website: [minisource.ir](https://minisource.ir)
- 📧 Email: info@minisource.ir
- 🐛 Issues: Open in respective repositories

---

<p align="center">
  <sub>Built with ❤️ by the Minisource team</sub>
</p>
