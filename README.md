# SoftwArt — Documentation / Documentación

> 🇨🇴 [Español](#español) · 🌐 [English](#english)

---

## English

This repository contains the complete technical and academic documentation for **SoftwArt**, a web and mobile management system built for **Arte Café** — a framing and marquetry shop in Medellín, Colombia.

SoftwArt was developed as a capstone project for the **Technology in Software Analysis and Development** program at SENA (Servicio Nacional de Aprendizaje), Regional Antioquia.

> All documents are written in **Spanish** as required by the academic institution. For technical details about the system architecture, stack, and codebase — including full bilingual (EN/ES) documentation — refer to the linked repositories below.

### What's in this repo

| Folder / File | Contents |
|---|---|
| `manual-tecnico/` | Full technical manual — requirements, architecture, UML diagrams, database model, security, migrations and backups |
| `diagramas/casos-de-uso/` | 8 UML use case diagrams (general + one per process) |
| `diagramas/casos-de-uso/documentacion/` | Detailed use case documentation tables |
| `diagramas/c4/` | C4 model diagrams: Context, Container and Component |
| `diagramas/clases/` | UML class diagram |
| `diagramas/facilitacion-grafica/` | Graphic facilitation — full system flow with actors |
| `diagramas/mapa-procesos/` | Business process map (strategic, key and support processes) |
| `mhu/` | User Story Matrix: project vision, epics, and full HU + acceptance criteria |
| `product-backlog/` | Prioritized product backlog (81 user stories with story points) |
| `story-mapping/` | Story mapping with Fibonacci story point estimation |

### Live system

🌐 [softwart.online](https://softwart.online)

### Related repositories

| Repo | Description |
|---|---|
| [backend-softwart](https://github.com/SoftwArt/backend-softwart) | Node.js · Express · TypeScript · TypeORM · PostgreSQL |
| [frontend-softwart-2](https://github.com/SoftwArt/frontend-softwart-2) | React · TypeScript · Vite · Tailwind · shadcn/ui |
| [mobile-softwart](https://github.com/SoftwArt/mobile-softwart) | Flutter · Dart · Clean Architecture · Provider |

### Roadmap — DevOps & Infrastructure

The current deployment uses native CI/CD provided by Render and Vercel (auto-deploy on push to `main`). The following improvements are planned for future iterations:

| Item | Description | Status |
|---|---|---|
| **GitHub Actions pipelines** | Explicit CI/CD workflows — lint, build and deploy stages per environment (dev / prod) | 🔜 Planned |
| **Automated testing** | Unit and integration test suites for backend (Jest) and frontend (Vitest + Testing Library) | 🔜 Planned |
| **Containerization** | Dockerize the backend service and define a `docker-compose.yml` for local development | 🔜 Planned |
| **TypeORM migrations** | Replace `synchronize: true` with versioned migration files for safe schema changes in production | 🔜 Planned |
| **Backup strategy** | Supabase automatic backups are active. A documented restore procedure and periodic export policy are planned | 🔜 Planned |
| **Environment parity** | Align local, staging and production environments via `.env` schema validation (e.g. `zod` + `dotenv`) | 🔜 Planned |

### Built by

**Sergio E. León V.** — [@selvcebo](https://github.com/selvcebo)
SENA · Technology in Software Analysis and Development · Medellín, Colombia

---

## Español

Este repositorio contiene la documentación técnica y académica completa de **SoftwArt**, un sistema de gestión web y móvil desarrollado para **Arte Café** — una marquetería PYME ubicada en Laureles, Medellín, Colombia.

SoftwArt fue desarrollado como proyecto de grado de la **Tecnología en Análisis y Desarrollo de Software** del SENA, Regional Antioquia.

### Contexto del proyecto

Arte Café operaba con agendas físicas, recibos en papel y acuerdos verbales de pago. Los clientes debían ir presencialmente para agendar o visualizar su trabajo. Sin un registro estructurado, la dueña enfrentaba conflictos frecuentes por pagos mal manejados y pedidos sin seguimiento. SoftwArt reemplaza ese flujo documental con un sistema centralizado desplegado en producción.

### Contenido del repositorio

| Carpeta / Archivo | Contenido |
|---|---|
| `manual-tecnico/` | Manual técnico completo — requerimientos, arquitectura, diagramas UML, modelo de BD, seguridad, migraciones y backups |
| `diagramas/casos-de-uso/` | 8 diagramas UML de casos de uso (general + uno por proceso) |
| `diagramas/casos-de-uso/documentacion/` | Tablas de documentación detallada de casos de uso |
| `diagramas/c4/` | Diagramas del modelo C4: Contexto, Contenedor y Componentes |
| `diagramas/clases/` | Diagrama de clases UML |
| `diagramas/facilitacion-grafica/` | Facilitación gráfica — flujo completo del sistema con actores |
| `diagramas/mapa-procesos/` | Mapa de procesos del negocio (estratégicos, clave y de apoyo) |
| `mhu/` | Matriz de Historias de Usuario: visión del proyecto, épicas y HU completas con criterios de aceptación |
| `product-backlog/` | Product backlog priorizado (81 historias de usuario con story points) |
| `story-mapping/` | Story mapping con estimación de puntos de historia en Fibonacci |

### Sistema en producción

🌐 [softwart.online](https://softwart.online)

### Repositorios relacionados

| Repo | Descripción |
|---|---|
| [backend-softwart](https://github.com/SoftwArt/backend-softwart) | Node.js · Express · TypeScript · TypeORM · PostgreSQL |
| [frontend-softwart-2](https://github.com/SoftwArt/frontend-softwart-2) | React · TypeScript · Vite · Tailwind · shadcn/ui |
| [mobile-softwart](https://github.com/SoftwArt/mobile-softwart) | Flutter · Dart · Clean Architecture · Provider |

### Stack general

| Capa | Tecnología |
|---|---|
| Backend | Node.js 18 + Express + TypeScript + TypeORM |
| Base de datos | PostgreSQL 15 (Supabase en producción) |
| Auth | JWT (8h) + bcrypt (salt 10) |
| Frontend | React 18 + TypeScript + Vite + Tailwind + shadcn/ui |
| Mobile | Flutter 3 + Dart + Provider + Clean Architecture |
| Deploy | Render (backend) · Vercel (frontend) · Supabase (BD) |

### Roadmap — DevOps e Infraestructura

El despliegue actual usa el CI/CD nativo de Render y Vercel (deploy automático en cada push a `main`). Las siguientes mejoras están planificadas para iteraciones futuras:

| Ítem | Descripción | Estado |
|---|---|---|
| **Pipelines con GitHub Actions** | Workflows explícitos de CI/CD — etapas de lint, build y deploy por ambiente (dev / prod) | 🔜 Planificado |
| **Tests automatizados** | Suites de pruebas unitarias e integración para backend (Jest) y frontend (Vitest + Testing Library) | 🔜 Planificado |
| **Containerización** | Dockerizar el servicio backend y definir un `docker-compose.yml` para desarrollo local | 🔜 Planificado |
| **Migraciones TypeORM** | Reemplazar `synchronize: true` por archivos de migración versionados para cambios de esquema seguros en producción | 🔜 Planificado |
| **Estrategia de backups** | Los backups automáticos de Supabase están activos. Se planifica documentar el procedimiento de restauración y una política de exportación periódica | 🔜 Planificado |
| **Paridad de entornos** | Alinear los entornos local, staging y producción mediante validación de esquema `.env` (ej. `zod` + `dotenv`) | 🔜 Planificado |

### Desarrollado por

**Sergio E. León V.** — [@selvcebo](https://github.com/selvcebo)
SENA · Tecnología en Análisis y Desarrollo de Software · Medellín, Colombia
