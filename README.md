# Abraham Lipa Calabilla

<p align="left">
  <strong>Senior Software Analyst · .NET & Azure Backend Specialist · Software Architecture</strong><br>
  Lima, Perú · English C2 Proficient (EF SET 73/100)
</p>

<p align="left">
  <a href="https://www.linkedin.com/in/abrlipac/"><img src="https://img.shields.io/badge/LinkedIn-abrlipac-0077B5?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:alipacala@outlook.com"><img src="https://img.shields.io/badge/Email-alipacala%40outlook.com-0078D4?style=flat&logo=microsoftoutlook&logoColor=white" alt="Email" /></a>
  <a href="https://github.com/alipacala/dev-vault"><img src="https://img.shields.io/badge/Dev--Vault-Enterprise%20Catalog-black?style=flat&logo=github&logoColor=white" alt="Dev-Vault" /></a>
</p>

---

## 📌 Perfil Profesional

Desarrollador de software con **3+ años full-time**, especializado en backend de alto rendimiento con **.NET (.NET 8 / .NET 10)** y ecosistema **Azure / Cloud**. Especialista en el diseño de microservicios, APIs REST críticas, arquitecturas orientadas a eventos (**CQRS, Event Sourcing**) y persistencia optimizada con **Entity Framework Core** y **SQL Server / PostgreSQL**.

Liderazgo técnico comprobado como referente para equipos de desarrollo: conducción de code review diario (~40 PRs/semana), mentoría técnica, mitigación proactiva de deuda técnica y diseño de contratos desacoplados.

---

## 🚀 Focos Principales de Experiencia y Arquitectura

### 1. 🏢 IDS Latam — Senior Software Analyst
*Sistemas de misión crítica para empresas mineras de primer nivel*

- **Arquitectura Backend & Core:** Lideré decisiones técnicas sobre sistemas backend en **.NET 8 / C#**, microservicios con **CQRS sobre MediatR**, Repository Pattern e inyección de dependencias sobre 12 módulos core (asistencia, control de acceso, autorizaciones internas, gestión SOMMA, contratos, seguros y vehículos).
- **Liderazgo Técnico:** Referente técnico para un equipo de **5+ ingenieros**, dirigiendo code reviews de **~40 PRs semanales**, estableciendo estándares de código y proponiendo mejoras transversales adoptadas en producción.
- **Autorización Multi-Tenant:** Implementé la arquitectura de autorización de extremo a extremo para **~100 roles y 8 clientes corporativos**, con roles en base de datos, filtrado multi-tenant (`IHasCustomer` / `IHasCuenta`) y caché distribuido de 15 minutos con invalidación inmediata.
- **Mensajería Asíncrona Resiliente:** Integración con **Azure Service Bus** (colas y topics) en 4 áreas de negocio (autorización, contratos, vehículos y seguros internos) con patrones de idempotencia y reintentos.
- **Optimización de Persistencia & Carga:** Mitigación de problemas N+1 con `AsNoTracking` y `AsSplitQuery`, operaciones batch con `ExecuteUpdate`/`ExecuteDelete` y `BulkExtensions`. **Reducción de 50% a 80% en tiempos de latencia** en reportes masivos de 10,000+ filas y consultas frontend.
- **Operación Cloud en Azure:** Despliegue en 2 regiones y 6 tenants usando Azure App Service, Azure Functions (notificaciones serverless), Azure SQL, Key Vault (secretos rotados vía RBAC), Azure AD (OpenIdConnect) y observabilidad con Azure Application Insights.

---

### 2. ⚡ Aegirax — Plataforma SaaS en Producción
*Plataforma propietaria diseñada y operada bajo estándares de ingeniería de alta fiabilidad*

- **Arquitectura Hexagonal & DDD:** Microservicios en **.NET 10 / C# 12** estructurados en 5 *Bounded Contexts*, Clean Architecture, value objects con Vogen y validaciones con FluentValidation.
- **CQRS & Event Sourcing:** Implementación avanzada con **Wolverine + Marten** sobre PostgreSQL, desacoplando comandos de mutación y eventos inmutables de dominio.
- **Identidad & Caché Distribuido:** Autenticación y autorización federada con **Keycloak (OIDC / JWT multi-tenant)**, filtrado dinámico por tenant y caché distribuido de alto rendimiento con **Redis**.
- **Infraestructura Cloud Serverless:** Despliegue continuo de 8 microservicios en **Google Cloud Run (GCP)** mediante Docker multi-stage y **GitHub Actions** conectado por **Workload Identity Federation** (cero credenciales estáticas en repositorios).
- **Cultura de Calidad & Testing Real:** Suite automatizada de **1,353 tests** (unitarios, de integración y de arquitectura) ejecutados con xUnit, FluentAssertions y **Testcontainers** contra instancias reales de PostgreSQL y Redis.
- **Observabilidad & Gobernanza Spec-Driven:** Instrumentación de trazas y métricas mediante **OpenTelemetry (OTLP)** y Cloud Logging; flujo de ingeniería guiado por especificaciones con 127 planes ejecutados, 26 ADRs (*Architecture Decision Records*) y 224 deudas técnicas cerradas con ciclo de vida.
- **Mobile Companion:** Aplicación móvil cross-platform desarrollada con **Expo SDK (React Native)**, TypeScript, expo-router y NativeWind.

---

### 3. 🏨 Arenas Hotel & Spa — Property Management System (PMS)
*Sistema integral de hotelería, resort, spa y gastronomía llevado de cero a producción*

- **Centralización Multi-Dominio:** Diseñé y desarrollé de extremo a extremo la plataforma que centraliza más de 20 operaciones operativas en 3 áreas comerciales: **Hospedaje (Hotel), Spa & Bienestar, y Alimentos & Bebidas (Restaurante)**.
- **Cuenta Maestra de Liquidación:** Implementación del modelo de estado de cuenta unificado (`nro_registro_maestro`), permitiendo consumos cruzados entre departamentos (cargos de restaurante y spa a la habitación) y liquidación consolidada en el check-out.
- **Cumplimiento Normativo (MINCETUR):** Módulo automatizado de registro de huéspedes y cálculo de tasas de ocupación para la generación de reportes oficiales requeridos por el Ministerio de Comercio Exterior y Turismo del Perú.
- **Punto de Venta e Impresión Térmica:** Arquitectura de comandas gastronómicas con escandallo (recetas e inventario) y enrutamiento por red a impresoras térmicas ESC/POS de cocina y bar.

---

## 🛠️ Stack Tecnológico & Habilidades

| Dominio | Tecnologías y Herramientas |
|---|---|
| **Backend & Lenguajes** | C# (.NET 8 / .NET 10), ASP.NET Core, Node.js, Python (Django, DRF), TypeScript |
| **Arquitectura & Patrones** | Clean Architecture, DDD, CQRS (MediatR, Wolverine), Event Sourcing (Marten), Hexagonal, Microfrontends (Single SPA), Repository Pattern, NSwag |
| **Bases de Datos & Caché** | SQL Server, Azure SQL Database, PostgreSQL, MariaDB/MySQL, Redis, Entity Framework Core, Dapper |
| **Cloud & Mensajería** | Microsoft Azure (App Service, Service Bus, Key Vault, Functions, App Insights, Azure DevOps), GCP (Cloud Run, Cloud Build, Pub/Sub), Cloudflare |
| **DevOps & CI/CD** | GitHub Actions (Workload Identity Federation), Azure Pipelines, Docker, Linux, Bash |
| **Testing & Calidad** | xUnit, Testcontainers, FluentAssertions, Respawn, Verify, Roslynator, SonarAnalyzer, Playwright |
| **Frontend & Mobile** | React, TypeScript, Zustand, SWR, Next.js, Angular, React Native (Expo) |

---

## 📦 Proyectos y Vault de Ingeniería

Para explorar modelos de dominio, esquemas de bases de datos DDL, patrones de concurrencia y especificaciones técnicas de proyectos pasados, visita mi repositorio de compilación arquitectónica:

👉 **[`alipacala/dev-vault`](https://github.com/alipacala/dev-vault)** — *Catálogo de microservicios, esquemas relacionales, diagramas dimensionales y guías de patrones enterprise.*
