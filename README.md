<h1 align="center">Samuel Zuleta Castañeda</h1>
<p align="center">
  <b>Full Stack Developer</b> · Estudiante de Ingeniería de Sistemas (UTP)<br/>
  📍 Pereira, Colombia
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white" />
  <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat&logo=cloudflare&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/Claude_API-D97757?style=flat&logo=anthropic&logoColor=white" />
</p>

---

## 👋 Sobre mí

Desarrollo aplicaciones web de punta a punta: frontend en React + TypeScript, backend sobre Supabase/PostgreSQL y Node.js, y despliegue con CI/CD en GitHub Actions, Vercel y Cloudflare.

Me enfoco en productos completos y mantenibles: seguridad desde la base de datos (RLS, validación en servidor), pipelines de CI/CD con quality gates y documentación técnica que acompaña cada entrega.

---

## 🚀 Proyectos destacados

> Los repositorios son privados por acuerdos con clientes. Aquí resumo alcance, arquitectura y stack; el detalle técnico está disponible bajo solicitud.

### 🏗️ Landing corporativa — Hispánica Constructora
**🔗 En vivo:** [hispanicaconstructora.com](https://hispanicaconstructora.com)

Sitio web oficial de una constructora, orientado a generación de leads y presencia digital.

- Diseño 100% responsive (mobile-first), optimizado para SEO y rendimiento
- Galería interactiva de proyectos y animaciones suaves
- Formulario de contacto sobre **Cloudflare Worker** con validación de orígenes y endurecimiento
- Dominio propio en Cloudflare, analítica y previews por rama en Vercel
- Flujo Git con ramas `feature → develop → main` y PRs revisados

`TypeScript` · `Cloudflare Workers` · `Vercel` · `GitHub Actions`

---

### 📒 IA para Auditoría Contable y Revisoría Fiscal — Curso interactivo
**🔗 En vivo:** [auditoriacontable.vercel.app](https://auditoriacontable.vercel.app)

Desarrollado para una firma de consultoría contable y auditoría. Aplicación educativa que enseña a contadores, auditores y revisores fiscales colombianos a usar IA (Claude) en su trabajo, fundamentada en el DUR Tributario (Decreto 1625 de 2016) y el Decreto 2420 de 2015.

- **8 módulos** con teoría, ejemplos resueltos, quizzes y ejercicios **calificados por IA con rúbrica (0–100)**
- Evaluador pedagógico de prompts: fortalezas, errores, faltantes y versión mejorada
- Backend Node.js + Express como proxy seguro: la API key nunca llega al navegador, sesión obligatoria y **rate limit por estudiante**
- Autenticación y progreso en **Supabase** con Row Level Security por usuario
- Emisión de certificados con autorización de administrador y código de verificación
- Pipeline CI/CD: calidad → seguridad → migraciones → deploy

`React` · `Vite` · `Node.js` · `Express` · `Supabase` · `Claude API` · `Vercel`

---

### 🎓 Plataforma LMS / marketplace de cursos (proyecto freelance)

Plataforma de aprendizaje online completa —venta de cursos, streaming de video protegido, comunidad y CRM— construida de extremo a extremo en **5 módulos** con **55+ historias de usuario** aceptadas. El cliente opera el negocio de forma **autosuficiente desde el panel de administración**, sin depender del desarrollador para el día a día.

**🧑‍💼 Panel de administración autosuficiente**
- **Creación y edición de cursos** con editor master-detail: curso → módulos → lecciones, contenido en Markdown, trailer y portada
- **Subida de video** reanudable (TUS) directo al CDN de streaming, con estado de procesamiento y biblioteca de videos reutilizables
- Gestión de **categorías, nichos, instructores, estudiantes y cupones**, con soft-delete y papelera
- **Roles y permisos dinámicos (RBAC granular)**: se crean roles nuevos sin tocar código
- Configuración de **gamificación** (puntos, niveles, topes diarios), **moderación de comunidad**, **marketing** (Meta, GA4, Google Ads, TikTok) e **integraciones CRM**
- Bitácora de auditoría de acciones del panel y alertas del sistema

**🎓 Experiencia del estudiante**
- Catálogo con filtros, vista previa gratuita de 2 min y video con URLs firmadas que caducan
- Progreso por lección con “retomar donde quedé”, contenido personalizado por nicho y **certificados en PDF**
- Carrito, lista de deseos, cupones y checkout con tarjeta, PSE y Nequi
- **Comunidad** con espacios por curso, publicaciones, comentarios, reacciones, notificaciones y ranking

**🔐 Seguridad**
- Autenticación con Google OAuth + correo, **MFA (TOTP)**, bloqueo por fuerza bruta y CAPTCHA
- **49 tablas con Row Level Security**, ~280 políticas; el navegador nunca es la autoridad
- Precio cotizado y firmado en servidor, webhooks de pago verificados por firma
- Saneamiento de texto en base de datos, CSP estricta y headers de seguridad

**⚙️ Backend y automatización**
- **28 Edge Functions** (Deno): video, pagos, MFA, CRM, correo, suscripciones y eventos de marketing server-side
- Sincronización con CRM mediante **cola durable con reintentos**, carritos abandonados y recordatorios de renovación
- Jobs programados en **pg_cron + pg_net** con reconciliador de fallos y alertas al panel

**🚀 Pipeline de CI/CD (GitHub Actions)**

Cada push pasa por un pipeline de seis etapas; nada llega a producción sin superar las anteriores:

| Etapa | Qué garantiza |
|---|---|
| **1. Calidad** | TypeScript estricto, ESLint, tests unitarios (Vitest), typecheck y tests de Edge Functions (Deno), build y verificación de CSP |
| **2. Seguridad** | Auditoría de dependencias con allowlist justificado, escaneo de secretos (TruffleHog) y SAST OWASP Top 10 (Semgrep) |
| **3. Migraciones** | 235+ migraciones SQL versionadas: validación de consistencia, aplicación automática y verificación de invariantes del esquema en remoto |
| **4. Edge Functions** | Despliegue de las funciones solo después de que el esquema esté aplicado |
| **5. Deploy** | Build y despliegue en Vercel por entorno: preview por rama, dev y producción |
| **6. Smoke test** | Prueba post-deploy de flujos críticos contra la API; si falla, el deploy queda en rojo |

Además: **57 specs E2E con Playwright** (incluidas 27 pruebas adversariales de seguridad), pruebas de carga con k6 y un **manual técnico** que documenta arquitectura, modelo de datos y operación.

`React 19` · `TypeScript` · `Vite` · `Tailwind CSS 4` · `Supabase (Postgres 17, Auth, Edge Functions, Realtime, Storage)` · `pg_cron` · `Vercel` · `GitHub Actions` · `Playwright` · `Vitest` · `k6`

---

## 🛠️ Cómo trabajo

- Historias de usuario en **Gherkin** y entregas por módulos con acta de aceptación
- **CI/CD** con etapas de calidad → seguridad → migraciones → deploy → smoke test
- Flujo Git `feature → develop → main` con PRs revisados y despliegues por entorno
- Seguridad desde el diseño: RLS, secretos solo en backend, validación de webhooks
- Documentación técnica como parte del entregable

---

## 📫 Contacto

- ✉️ [samuel.zuleta@utp.edu.co](mailto:samuel.zuleta@utp.edu.co)
<h1 align="center">Samuel Zuleta Castañeda</h1>
<p align="center">
  <b>Full Stack Developer</b> · Estudiante de Ingeniería de Sistemas y Computación (UTP)<br/>
  📍 Pereira, Colombia
</p>

<p align="center">
  <img src="https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=flat&logo=tailwindcss&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3FCF8E?style=flat&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white" />
  <img src="https://img.shields.io/badge/Cloudflare-F38020?style=flat&logo=cloudflare&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/Playwright-2EAD33?style=flat&logo=playwright&logoColor=white" />
  <img src="https://img.shields.io/badge/Claude_API-D97757?style=flat&logo=anthropic&logoColor=white" />
</p>

---

## Sobre mí

Desarrollo aplicaciones web de punta a punta: frontend en React + TypeScript, backend sobre Supabase/PostgreSQL y Node.js, y despliegue con CI/CD en GitHub Actions, Vercel y Cloudflare.

Combino la ingeniería de software con experiencia profesional en **auditoría y cumplimiento tributario y laboral en Colombia**, lo que me permite construir productos que entienden el negocio del cliente y no solo la parte técnica.

---

## Proyectos destacados

> Los repositorios son privados por acuerdos con clientes. Aquí resumo alcance, arquitectura y stack; el detalle técnico está disponible bajo solicitud.

### Landing corporativa — Hispánica Constructora
** En vivo:** [hispanicaconstructora.com](https://hispanicaconstructora.com)

Sitio web oficial de una constructora, orientado a generación de leads y presencia digital.

- Diseño 100% responsive (mobile-first), optimizado para SEO y rendimiento
- Galería interactiva de proyectos y animaciones suaves
- Formulario de contacto sobre **Cloudflare Worker** con validación de orígenes y endurecimiento
- Dominio propio en Cloudflare, analítica y previews por rama en Vercel
- Flujo Git con ramas `feature → develop → main` y PRs revisados

`TypeScript` · `Cloudflare Workers` · `Vercel` · `GitHub Actions`

---

### IA para Auditoría Contable y Revisoría Fiscal — Curso interactivo
**🔗 En vivo:** [auditoriacontable.vercel.app](https://auditoriacontable.vercel.app)

Aplicación educativa que enseña a contadores, auditores y revisores fiscales colombianos a usar IA (Claude) en su trabajo, fundamentada en el DUR Tributario (Decreto 1625 de 2016) y el Decreto 2420 de 2015.

- **8 módulos** con teoría, ejemplos resueltos, quizzes y ejercicios **calificados por IA con rúbrica (0–100)**
- Evaluador pedagógico de prompts: fortalezas, errores, faltantes y versión mejorada
- Backend Node.js + Express como proxy seguro: la API key nunca llega al navegador, sesión obligatoria y **rate limit por estudiante**
- Autenticación y progreso en **Supabase** con Row Level Security por usuario
- Emisión de certificados con autorización de administrador y código de verificación
- Pipeline CI/CD: calidad → seguridad → migraciones → deploy

`React` · `Vite` · `Node.js` · `Express` · `Supabase` · `Claude API` · `Vercel`

---

### Plataforma LMS / marketplace de cursos (proyecto freelance)

Plataforma de aprendizaje online con cursos, instructores, comunidad, suscripciones y pagos, desarrollada de extremo a extremo en 5 módulos.

- **Infraestructura y autenticación** con MFA
- **Cursos y video** con streaming HLS, subidas TUS y reproducción firmada
- **Pagos** con pasarela colombiana, webhooks verificados por firma y flujo de suscripciones
- **Integración CRM** con cola de reintentos, carritos abandonados y recordatorios de renovación
- **Comunidad y gamificación** en tiempo real
- ~28 Edge Functions, eventos de marketing server-side y pipeline CI/CD con pruebas E2E

`React 19` · `TypeScript` · `Tailwind CSS 4` · `Supabase (Postgres, Auth, Edge Functions, Realtime)` · `Vercel` · `GitHub Actions` · `Playwright`

---

## Cómo trabajo

- Historias de usuario en **Gherkin** y entregas por módulos con acta de aceptación
- **CI/CD** con quality gates, migraciones versionadas y despliegues por entorno (preview / dev / prod)
- Seguridad desde el diseño: RLS, secretos solo en backend, validación de webhooks
- Documentación técnica como parte del entregable

---

## Contacto

- ✉️ [samuelzuleta276@gmail.com](mailto:samuelzuleta276@gmail.com)
