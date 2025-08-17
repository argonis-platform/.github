# 🚀 Argonis

> **The unified knowledge platform that bridges the gap between document management, wiki collaboration, file sharing, and team workspaces.**
Argonis is a **modern, self-hosted platform** that combines document management, wiki collaboration, and file synchronization into a single, scalable solution. Built for both tech-savvy individuals and enterprise environments.

## Why Argonis?

Tired of switching between **file storage**, **wiki**, and **document management** tools? Argonis combines them into **one self-hosted platform**.
**Document management** with modern classification. **Wiki collaboration** for knowledge building. **File sync** across desktop and mobile. **All in one place**, on your infrastructure.

## Features

| Feature | Status | Description |
|---------|--------|-------------|
| **Core Backend** | ✅ MVP | GraphQL API, multi-workspace architecture, unified document/file/folder system |
| **Web Client** | ✅ MVP | React interface with real-time updates, modern UI components |
| **Document Types** | ✅ MVP | Markdown documents + binary files, version control, preview system |
| **Access Control** | ✅ MVP | Granular permissions, team roles, guest sharing with expiration |
| **Search & Organization** | ✅ MVP | Full-text search, tagging system, activity logs and audit trails |
| **Real-time Collaboration** | 🔄 Planned | Live document editing, comment threads, cursor tracking |
| **Content Processing** | 🔄 Planned | Auto-classification, semantic search, document summaries |
| **Desktop Sync** | 🔄 Planned | Cross-platform clients (Windows/macOS/Linux) with offline support |
| **Mobile Apps** | 🔄 Planned | iOS/Android apps with offline caching and conflict resolution |
| **Advanced Auth** | 🔄 Planned | LDAP/SAML integration, SSO providers, multi-factor authentication |
| **Workflow Engine** | 🔄 Planned | Review processes, approval workflows, automated actions |
| **API Extensions** | 🔄 Planned | Webhooks, custom metadata fields, third-party integrations |
| **Analytics** | 🔄 Planned | Usage dashboard, content insights, compliance reporting |

## Architecture

**Backend Services:** Django 5 core with **GraphQL API** (graphene), **PostgreSQL** primary database, **Redis** for caching and real-time features, **MinIO** S3-compatible storage, **Celery** background processing.
**Client Applications:** **React 18 + Vite** web client with shadcn/ui, **Tauri** desktop sync clients, **React Native** mobile apps with offline support.
**Infrastructure:** **Docker** containerization, **Kubernetes** deployment manifests, **Traefik** reverse proxy and load balancer.
