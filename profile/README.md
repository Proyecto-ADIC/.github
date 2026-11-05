<div align="center">
  <img src="./banner.svg" alt="ADIC – Plataforma Deportiva" width="100%">
</div>

<br>

<div align="center">

[![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)](https://github.com/Proyecto-ADIC/adic-platform-api)
[![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white)](https://github.com/Proyecto-ADIC/adic-platform-web)
[![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://github.com/Proyecto-ADIC/adic-platform-api)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=flat-square&logo=postgresql&logoColor=white)](https://github.com/Proyecto-ADIC/adic-platform-api)
[![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)](https://github.com/Proyecto-ADIC/adic-platform-infra)
[![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)](https://github.com/Proyecto-ADIC/adic-platform-infra)
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)](https://github.com/Proyecto-ADIC/adic-platform-infra)

</div>

---

## Repositorios

| Repositorio | Descripción | Stack |
|---|---|---|
| [**adic-platform-api**](https://github.com/Proyecto-ADIC/adic-platform-api) | REST API backend — gestión de competencias, inscripciones, puntajes y sincronización offline | NestJS · TypeORM · PostgreSQL · Keycloak · AWS S3 |
| [**adic-platform-web**](https://github.com/Proyecto-ADIC/adic-platform-web) | Sitio web público — calendario de eventos, resultados y galería multimedia | Angular 21 · Angular Material |
| [**adic-platform-backoffice**](https://github.com/Proyecto-ADIC/adic-platform-backoffice) | Portal administrativo — CRUD completo, reportes PDF con QR y autorización de dispositivos | Angular 21 · Tailwind CSS · jsPDF |
| [**adic-platform-pwa**](https://github.com/Proyecto-ADIC/adic-platform-pwa) | App Progressive Web App para árbitros — offline-first con sincronización automática | Angular 21 · Service Worker · Dexie (IndexedDB) |
| [**adic-platform-infra**](https://github.com/Proyecto-ADIC/adic-platform-infra) | Infraestructura como código — EC2, S3, CloudFront, ECR, IAM y CI/CD | Terraform · AWS · GitHub Actions · Docker |

---

## Ecosistema

<div align="center">
  <img src="./architecture.svg" alt="ADIC – Arquitectura del Sistema" width="100%">
</div>

---

## Módulos principales

**Gestión deportiva**
- **Competencias** — creación y administración de eventos deportivos
- **Disciplinas y categorías** — estructura jerárquica configurable
- **Inscripciones** — registro de competidores por evento
- **Puntajes** — evaluación por plantillas configurables
- **Resultados** — cálculo y publicación de clasificaciones

**Operaciones**
- **Carnet deportivo** — emisión y gestión de carnets por competidor
- **Instituciones** — gestión de clubes y organizaciones afiliadas
- **Gestión de usuarios** — roles y permisos vía Keycloak
- **Reportes** — exportación a PDF con QR y Excel

**PWA offline-first**
- Descarga de bundle de competencia para trabajo sin conectividad
- Almacenamiento local en IndexedDB (Dexie)
- Autorización de dispositivo por código único / QR
- Sincronización automática al recuperar conexión

---

## Stack tecnológico

| Capa | Tecnologías |
|---|---|
| **Backend** | NestJS 11 · TypeScript 5.7 · TypeORM 0.3 · PostgreSQL 16 |
| **Frontend** | Angular 21 (Standalone) · Angular Material 21 · SCSS · Tailwind CSS 4 |
| **Auth** | Keycloak (OpenID Connect) · JWT Bearer · RBAC |
| **Storage** | AWS S3 · CloudFront · IndexedDB (Dexie) |
| **Infra** | AWS EC2 · ECR · SSM · Terraform 1.10 |
| **CI/CD** | GitHub Actions · GitHub OIDC · Docker Compose |
| **Testing** | Jest · Supertest · Vitest |

---

<div align="center">
  <sub>Proyecto de Grado · Universidad Católica del Uruguay · 2026</sub>
</div>
