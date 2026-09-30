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
