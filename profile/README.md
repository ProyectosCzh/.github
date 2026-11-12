<div align="center">

  <img src="./assets/banner.svg" alt="ProyectosCzh" width="100%">

  <br>

  <h3>Carlos Moisés Zambrana Hurtado</h3>
  <p><strong>Ingeniería de Sistemas · Backend · APIs · Automatización · Cómputo científico</strong></p>

  <p>
    <a href="mailto:carlosmzambranah19@gmail.com"><img src="./assets/badges/email.svg" alt="Email" height="32"></a>
    <a href="https://www.linkedin.com/in/carlos-mzambrana"><img src="./assets/badges/linkedin.svg" alt="LinkedIn" height="32"></a>
    <a href="https://github.com/ProyectosCzh"><img src="./assets/badges/github.svg" alt="GitHub" height="32"></a>
  </p>

</div>

---

## `01` · Sobre el proyecto

**ProyectosCzh** es mi laboratorio de ingeniería: un espacio donde cada repositorio es un sistema completo, con su arquitectura, su base de datos, sus pruebas y su documentación.

Trabajo el ciclo completo de desarrollo —levantamiento y análisis de requerimientos, historias de usuario, MVPs iterativos, pruebas de APIs y despliegue— bajo marcos ágiles (**Scrum** y **Kanban**), con énfasis en **código limpio**, **contratos tipados** y **validación continua**.

| Enfoque | Descripción |
| :--- | :--- |
| **Arquitectura** | Diseño de APIs REST, modelado de dominio y persistencia relacional. |
| **Automatización** | Herramientas CLI de línea de comandos para tareas operativas del día a día. |
| **Cómputo** | Modelado numérico, simulación financiera y análisis de datos. |
| **Estructuras de datos** | Implementaciones propias de TADs: tablas hash, AVL, grafos, listas y colas. |

---

## `02` · Proyectos destacados

<div align="center">

<a href="https://github.com/ProyectosCzh/web-sistema-laboratorios"><img src="./assets/projects/labmanage-web.svg" alt="LABMANAGE Web" width="100%"></a>
<a href="https://github.com/ProyectosCzh/api-sistema-laboratorios"><img src="./assets/projects/labmanage-api.svg" alt="LABMANAGE API" width="100%"></a>

</div>

### `LABMANAGE` · Plataforma de gestión de laboratorios

Suite full-stack para la administración y control operativo de laboratorios: reservas de aulas y turnos, estados por aula, asignación de docentes, mantenimiento y estadísticas en vivo.

| Capa | Repositorio | Stack |
| :--- | :--- | :--- |
| **Frontend** | [web-sistema-laboratorios](https://github.com/ProyectosCzh/web-sistema-laboratorios) | `Astro 7` `React 19` `TypeScript` `Tailwind 4` `TanStack Query` |
| **API** | [api-sistema-laboratorios](https://github.com/ProyectosCzh/api-sistema-laboratorios) | `Node.js` `Express 5` `TypeScript` `Prisma` `PostgreSQL` `Zod` |

<details>
<summary><b>Detalles técnicos</b></summary>

- **Frontend:** Astro en modo `server` con islas React `client:only`, estado de sesión en `localStorage`, capa de API con interceptores de autenticación y manejo de errores, TanStack Query como única fuente de verdad del estado remoto.
- **API:** Express 5 + TypeScript estricto, ORM Prisma sobre PostgreSQL (Neon), caché en memoria con invalidación *write-through* y deduplicación *single-flight*.
- **Seguridad:** doble token (access JWT 15 min + refresh JWT 7 días) con sesiones persistidas, `bcryptjs`, Helmet, CORS con credenciales, *rate limiting* por endpoint y validación Zod en el límite.
- **Documentación:** referencia interactiva con Scalar y especificación OpenAPI 3.x.

</details>

---

<div align="center">

<a href="https://github.com/ProyectosCzh/riskv2cla"><img src="./assets/projects/smartrisk.svg" alt="SmartRisk" width="100%"></a>
<a href="https://github.com/ProyectosCzh/backendcanchago"><img src="./assets/projects/canchago.svg" alt="CanchaGo" width="100%"></a>

</div>

### `SmartRisk` · Robo-asesor académico con simulación de portafolios

Plataforma web de simulación financiera y dimensionamiento automatizado de portafolios. Aplica TADs, hashing y persistencia a un problema real: la optimización de portafolios de inversión mediante métodos de *Financial Engineering*.

| Detalle | Descripción |
| :--- | :--- |
| **Motor financiero** | Optimización de **Markowitz** (máxima razón de Sharpe y mínima varianza) con frontera eficiente y **Simulación Monte Carlo** sobre GBM. |
| **Stack** | `Python 3.11` `Streamlit` `NumPy` `SciPy` `Pandas` `Plotly` `yfinance` |
| **Persistencia** | JSON con *sharding* por usuario y escritura atómica. |
| **Repositorio** | [riskv2cla](https://github.com/ProyectosCzh/riskv2cla) |

### `CanchaGo` · Backend de reservas deportivas

Servicio backend con la lógica de negocio y la gestión de reservas de canchas: autenticación, disponibilidad de horarios y control de turnos.

| Detalle | Descripción |
| :--- | :--- |
| **Stack** | `Python` `Django 5` `Django REST Framework` `JWT` `PostgreSQL` `Gunicorn` |
| **Repositorio** | [backendcanchago](https://github.com/ProyectosCzh/backendcanchago) |

---

<div align="center">

<a href="https://github.com/ProyectosCzh/DocsOrganizator"><img src="./assets/projects/docsorganizator.svg" alt="DocsOrganizator" width="100%"></a>
<a href="https://github.com/ProyectosCzh/Comparativo-Euler-Runge-Kutta"><img src="./assets/projects/euler-rk.svg" alt="Euler vs Runge-Kutta" width="100%"></a>

</div>

### `DocsOrganizator` · Organizador de documentos con eliminación de duplicados

Utilidad de línea de comandos para clasificar documentos automáticamente y eliminar duplicados mediante metadatos EXIF/QuickTime con ExifTool.

- **Modo copia estricto por defecto:** la biblioteca original nunca se modifica.
- Ordena por **fecha de captura real** en carpetas `Año\Mes`, independiente de la fecha del sistema de archivos.
- Detección de duplicados en **dos fases**: muestra rápida por tamaño + hash, y confirmación total por MD5.
- **Trazabilidad total:** cada operación queda registrada en CSV, con bitácora de respaldo e importación incremental reanudable.

| Detalle | Descripción |
| :--- | :--- |
| **Stack** | `Perl` `Python` `ExifTool` `CLI` |
| **Repositorio** | [DocsOrganizator](https://github.com/ProyectosCzh/DocsOrganizator) |

### `Comparativo Euler vs. Runge-Kutta` · Análisis numérico

Implementación y análisis comparativo entre los métodos de Euler y Runge-Kutta, con verificación simbólica de las soluciones y medición de los errores de aproximación.

| Detalle | Descripción |
| :--- | :--- |
| **Stack** | `Python` `FastAPI` `SymPy` `Uvicorn` |
| **Repositorio** | [Comparativo-Euler-Runge-Kutta](https://github.com/ProyectosCzh/Comparativo-Euler-Runge-Kutta) |

---

<div align="center">

<a href="https://github.com/ProyectosCzh/ProyectoFinalEstructuraAvanzada-Pirata"><img src="./assets/projects/tesoro-pirata.svg" alt="El Tesoro del Pirata" width="100%"></a>

</div>

### Proyectos de estructuras de datos

| Repositorio | Descripción | Stack |
| :--- | :--- | :--- |
| **[El Tesoro del Pirata](https://github.com/ProyectosCzh/ProyectoFinalEstructuraAvanzada-Pirata)** | Juego de búsqueda de caminos con **BFS** sobre un **grafo ponderado**, mapa interactivo con *pan* y *zoom* sincronizado, y **árbol de pistas n-ario**. | `C++` `Raylib` |

---

## `03` · Stack tecnológico

<div align="center">

| Área | Tecnologías |
| :--- | :--- |
| **Lenguajes** | <img src="./assets/icons/cplusplus.svg" width="40" height="40" alt="C++" title="C++"> <img src="./assets/icons/python.svg" width="40" height="40" alt="Python" title="Python"> <img src="./assets/icons/csharp.svg" width="40" height="40" alt="C#" title="C#"> <img src="./assets/icons/javascript.svg" width="40" height="40" alt="JavaScript" title="JavaScript"> <img src="./assets/icons/typescript.svg" width="40" height="40" alt="TypeScript" title="TypeScript"> <img src="./assets/icons/dart.svg" width="40" height="40" alt="Dart" title="Dart"> <img src="./assets/icons/perl.svg" width="40" height="40" alt="Perl" title="Perl"> <img src="./assets/icons/mysql.svg" width="40" height="40" alt="SQL" title="SQL"> |
| **Frontend** | <img src="./assets/icons/html5.svg" width="40" height="40" alt="HTML5" title="HTML5"> <img src="./assets/icons/css3.svg" width="40" height="40" alt="CSS3" title="CSS3"> <img src="./assets/icons/react.svg" width="40" height="40" alt="React" title="React"> <img src="./assets/icons/astro.svg" width="40" height="40" alt="Astro" title="Astro"> <img src="./assets/icons/tailwindcss.svg" width="40" height="40" alt="Tailwind CSS" title="Tailwind CSS"> <img src="./assets/icons/bootstrap.svg" width="40" height="40" alt="Bootstrap" title="Bootstrap"> |
| **Backend & APIs** | <img src="./assets/icons/nodedotjs.svg" width="40" height="40" alt="Node.js" title="Node.js"> <img src="./assets/icons/express.svg" width="40" height="40" alt="Express" title="Express"> <img src="./assets/icons/fastapi.svg" width="40" height="40" alt="FastAPI" title="FastAPI"> <img src="./assets/icons/django.svg" width="40" height="40" alt="Django" title="Django"> <img src="./assets/icons/dotnet.svg" width="40" height="40" alt="ASP.NET Core" title="ASP.NET Core"> <img src="./assets/icons/swagger.svg" width="40" height="40" alt="Swagger" title="Swagger"> <img src="./assets/icons/prisma.svg" width="40" height="40" alt="Prisma" title="Prisma"> <img src="./assets/icons/zod.svg" width="40" height="40" alt="Zod" title="Zod"> |
| **Bases de datos** | <img src="./assets/icons/postgresql.svg" width="40" height="40" alt="PostgreSQL" title="PostgreSQL"> <img src="./assets/icons/microsoftsqlserver.svg" width="40" height="40" alt="SQL Server" title="SQL Server"> <img src="./assets/icons/sqlite.svg" width="40" height="40" alt="SQLite" title="SQLite"> <img src="./assets/icons/mysql.svg" width="40" height="40" alt="MySQL" title="MySQL"> |
| **Datos & Cómputo** | <img src="./assets/icons/pandas.svg" width="40" height="40" alt="Pandas" title="Pandas"> <img src="./assets/icons/numpy.svg" width="40" height="40" alt="NumPy" title="NumPy"> <img src="./assets/icons/scipy.svg" width="40" height="40" alt="SciPy" title="SciPy"> <img src="./assets/icons/sympy.svg" width="40" height="40" alt="SymPy" title="SymPy"> <img src="./assets/icons/streamlit.svg" width="40" height="40" alt="Streamlit" title="Streamlit"> <img src="./assets/icons/plotly.svg" width="40" height="40" alt="Plotly" title="Plotly"> |
| **Móvil & Escritorio** | <img src="./assets/icons/flutter.svg" width="40" height="40" alt="Flutter" title="Flutter"> <img src="./assets/icons/cplusplus.svg" width="40" height="40" alt="C++" title="C++"> <img src="./assets/icons/raylib.svg" width="40" height="40" alt="Raylib" title="Raylib"> |
| **QA & Herramientas** | <img src="./assets/icons/pytest.svg" width="40" height="40" alt="pytest" title="pytest"> <img src="./assets/icons/postman.svg" width="40" height="40" alt="Postman" title="Postman"> <img src="./assets/icons/git.svg" width="40" height="40" alt="Git" title="Git"> <img src="./assets/icons/github.svg" width="40" height="40" alt="GitHub" title="GitHub"> <img src="./assets/icons/vite.svg" width="40" height="40" alt="Vite" title="Vite"> <img src="./assets/icons/visualstudiocode.svg" width="40" height="40" alt="VS Code" title="VS Code"> <img src="./assets/icons/rider.svg" width="40" height="40" alt="JetBrains Rider" title="JetBrains Rider"> |
| **Cloud & Despliegue** | <img src="./assets/icons/vercel.svg" width="40" height="40" alt="Vercel" title="Vercel"> <img src="./assets/icons/netlify.svg" width="40" height="40" alt="Netlify" title="Netlify"> <img src="./assets/icons/render.svg" width="40" height="40" alt="Render" title="Render"> <img src="./assets/icons/linux.svg" width="40" height="40" alt="Linux" title="Linux"> |

</div>

---

## `04` · Metodología y trayectoria

| Área | Detalle |
| :--- | :--- |
| **Flujo de ingeniería** | Levantamiento de requerimientos, historias de usuario, desarrollo iterativo de MVPs, pruebas de APIs y documentación técnica. |
| **Calidad** | Código limpio, tipado estricto, validación en el límite de la API y pruebas automatizadas. |
| **Documentación** | README técnico por proyecto con arquitectura, modelo de datos, flujo de uso y scripts reproducibles. |
| **Desarrollo freelance** | `2025 — Presente` · Aplicaciones a medida, integración de APIs y herramientas de análisis de datos en coordinación directa con clientes. |

---

<div align="center">

### ¿Tienes una idea de proyecto o buscas colaborar en código?

Escríbeme por correo o LinkedIn — respondo siempre.

<br>

<a href="mailto:carlosmzambranah19@gmail.com"><img src="./assets/badges/email.svg" alt="Email" height="32"></a>
&nbsp;
<a href="https://www.linkedin.com/in/carlos-mzambrana"><img src="./assets/badges/linkedin.svg" alt="LinkedIn" height="32"></a>
&nbsp;
<a href="https://github.com/ProyectosCzh"><img src="./assets/badges/github.svg" alt="GitHub" height="32"></a>

<br><br>

<sub>Hecho por <a href="https://github.com/ProyectosCzh">ProyectosCzh</a></sub>

</div>
