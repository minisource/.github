# Minisource

**Modern microservices platform built with Go, .NET, and Next.js**

Minisource is a comprehensive microservices ecosystem providing authentication, storage, notifications, payments, and more. All services are designed for scalability, observability, and developer productivity.

---

## 📁 Project Structure

```
.
├── auth/                       # Authentication & Authorization
│   ├── backend/                # Go service (JWT, RBAC, OAuth, users)
│   └── front/                  # Admin panel (Next.js 15)
├── gateway/                    # API gateway and edge routing
│   └── backend/
├── notifier/                   # Notification service
│   ├── backend/                # Go service (email, SMS, push, in-app, WS)
│   └── front/                  # Admin panel (Next.js 15)
├── storage/                    # Object and file storage service
│   └── backend/
├── log/                        # Centralized logging
│   └── backend/
├── scheduler/                  # Distributed job scheduler
│   └── backend/
├── comment/                    # Comment service with moderation
│   └── backend/
├── feedback/                   # Feedback collection
│   └── backend/
├── ticket/                     # Support ticket system
│   └── backend/
├── payment/                    # Payment processing (.NET)
│   └── backend/
├── cms/                        # Content Management System
│   └── backend/
├── doc/                        # Documentation site
│   └── backend/
├── infra/                      # Infrastructure-as-code
│   └── backend/
├── go-common/                  # Shared Go utilities
│   └── backend/
├── go-sdk/                     # Go SDK
│   └── backend/
├── go-template/                # Go project template
│   └── backend/
├── csharp-common/              # Shared C# utilities
│   └── backend/
├── csharp-sdk/                 # C# SDK
│   └── backend/
├── flutter-template/           # Flutter mobile app template
│   └── backend/
├── front-template/             # Next.js frontend template (source)
│   ├── src/
│   │   ├── api/                # API layer (Axios + services)
│   │   ├── app/                # Next.js App Router pages
│   │   │   ├── (auth)/         # Login, Register, Forgot Password
│   │   │   └── (main)/         # Dashboard, Admin, Profile
│   │   ├── components/         # shadcn/ui components
│   │   ├── hooks/              # React Query hooks
│   │   ├── stores/             # Zustand state management
│   │   └── types/              # TypeScript types
│   ├── Dockerfile              # Production container
│   └── docker-compose.yml      # Docker Compose
├── front-template/             # Next.js frontend template (source)
└── .github/profile/README.md   # This file
```

---

## 🚀 Core Services

### Security & Identity
- **[auth](backend/auth)** - Authentication and authorization service (JWT, OAuth, users, RBAC)  
  🌐 [auth.minisource.ir](https://auth.minisource.ir)

### API & Gateway
- **[gateway](backend/gateway)** - API gateway and edge routing for all services  
  🌐 [gateway.minisource.ir](https://gateway.minisource.ir)

### Data & Storage
- **[storage](backend/storage)** - Object and file storage service (S3-compatible)  
  🌐 [storage.minisource.ir](https://storage.minisource.ir)

- **[log](backend/log)** - Centralized logging and log aggregation  
  🌐 [log.minisource.ir](https://log.minisource.ir)

### Communication
- **[notifier](backend/notifier)** - Notification service for emails, SMS, and push notifications  
  🌐 [notifier.minisource.ir](https://notifier.minisource.ir)

- **[comment](backend/comment)** - Comment service with moderation  
  🌐 [comment.minisource.ir](https://comment.minisource.ir)

### Content & User Engagement
- **[cms](backend/cms)** - Content Management System and blog platform  
  🌐 [cms.minisource.ir](https://cms.minisource.ir)

- **[feedback](backend/feedback)** - Feedback collection and survey backend  
  🌐 [feedback.minisource.ir](https://feedback.minisource.ir)

- **[ticket](backend/ticket)** - Support ticket and helpdesk system  
  🌐 [ticket.minisource.ir](https://ticket.minisource.ir)

### Background Processing
- **[scheduler](backend/scheduler)** - Distributed job scheduler and cron service  
  🌐 [scheduler.minisource.ir](https://scheduler.minisource.ir)

### Commerce
- **[payment](backend/payment)** - Payment processing and gateway integration  
  🌐 [payment.minisource.ir](https://payment.minisource.ir)

---

## 🖥️ Frontend

### Auth Admin Panel (`auth/front/`)
A comprehensive admin dashboard for the Authentication Service built with Next.js 15, shadcn/ui, and TypeScript:

- **Authentication**: Email/password, Phone OTP, Google OAuth2, Registration, Password Reset
- **Admin Management**: Users CRUD, Roles & Permissions, Service Clients
- **Profile**: Profile settings, Password change, Session management, Linked Accounts
- **Security**: JWT tokens, RBAC, Account lockout, OTP verification, Token validation

```bash
cd auth/front
npm install
cp .env.example .env.local
npm run dev
```

### Notifier Admin Panel (`notifier/front/`)
A complete admin dashboard for the Notification Service built with Next.js 15, shadcn/ui, and TypeScript:

- **Dashboard**: Overview metrics, notification type distribution, quick actions
- **Notifications**: Create/send notifications (email, SMS, push, in-app), view/filter by user, mark as read
- **Templates**: Full CRUD with variables, provider integration, activate/deactivate
- **Preferences**: Per-user channel preferences, instant vs digest, frequency settings
- **Admin**: Users, delivery logs, system settings

```bash
cd notifier/front
npm install
cp .env.example .env.local
npm run dev
```

---

## 🛠️ SDKs & Libraries

### Go Ecosystem
- **[go-sdk](backend/go-sdk)** - Go SDK with clients for all Minisource services
- **[go-common](backend/go-common)** - Shared Go utilities, helpers, and libraries
- **[go-template](backend/go-template)** - Go project template with best practices

### .NET Ecosystem
- **[csharp-sdk](backend/csharp-sdk)** - C# SDK and client libraries
- **[csharp-common](backend/csharp-common)** - Shared C# utilities and helpers

---

## 📦 Templates & Tools

- **[front-template](front-template)** - Next.js 15 + shadcn/ui + Tailwind template  
  Modern frontend starter with TypeScript, Zustand, TanStack Query, Docker, and CI/CD

- **[infra](backend/infra)** - Infrastructure-as-code, Terraform modules, and deployment scripts  
  🌐 [infra.minisource.ir](https://infra.minisource.ir)

- **[doc](backend/doc)** - Documentation site and content  
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
| **Storage** | SILO (S3, MinIO fork — https://silo.pgsty.com/), Azure Blob |
| **Observability** | Prometheus, Grafana, Loki |
| **Infrastructure** | Docker, Kubernetes, Terraform |
| **CI/CD** | GitHub Actions |
| **Container Registry** | [Docker Hub (`minisource`)](https://hub.docker.com/orgs/minisource/repositories) |

---

## 📖 Getting Started

Each service in `backend/` contains:
- 📄 Comprehensive README with setup instructions
- 🐳 Docker Compose for local development
- ⚙️ CI/CD workflows with GitHub Actions
- 🔒 Security policy and vulnerability reporting
- 🧪 Unit and integration tests

### Quick Start Example

```bash
# Start the auth service
cd backend/auth
docker-compose up -d
make run

# Start the auth frontend admin panel
cd front
npm install
npm run dev
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
