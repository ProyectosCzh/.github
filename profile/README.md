<div align="center">

  <img src="./assets/banner.svg" alt="ProyectosCzh" width="100%">

  <br><br>

  <img src="https://github.com/ProyectosCzh.png" alt="Logo ProyectosCzh" width="96" height="96">

  <h3>Carlos Moisés Zambrana Hurtado</h3>
  <p><strong>Ingeniería de Sistemas · Backend · APIs · Automatización · Cómputo científico</strong></p>

  <p>
    <a href="mailto:carlosmzambranah19@gmail.com"><img src="https://img.shields.io/badge/Email-carlosmzambranah19%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
    <a href="https://www.linkedin.com/in/carlos-mzambrana"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
    <a href="https://github.com/ProyectosCzh"><img src="https://img.shields.io/badge/GitHub-ProyectosCzh-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub"></a>
    <a href="https://github.com/ProyectosCzh?tab=repositories"><img src="https://img.shields.io/github/repos/ProyectosCzh?style=flat-square&logo=github&logoColor=white&label=Repos" alt="Repositorios"></a>
    <a href="https://github.com/ProyectosCzh"><img src="https://img.shields.io/github/followers/ProyectosCzh?style=flat-square&logo=github&logoColor=white&label=Followers" alt="Followers"></a>
    <a href="https://github.com/ProyectosCzh"><img src="https://img.shields.io/github/last-commit/ProyectosCzh?style=flat-square&logo=github&logoColor=white&label=Último%20commit" alt="Último commit"></a>
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

<a href="https://github.com/ProyectosCzh/web-sistema-laboratorios"><img src="https://opengraph.githubassets.com/1/ProyectosCzh/web-sistema-laboratorios" alt="LABMANAGE Web" width="100%"></a>
<a href="https://github.com/ProyectosCzh/api-sistema-laboratorios"><img src="https://opengraph.githubassets.com/1/ProyectosCzh/api-sistema-laboratorios" alt="LABMANAGE API" width="100%"></a>

</div>

### `LABMANAGE` · Plataforma de gestión de laboratorios

Suite full-stack para la administración y control operativo de laboratorios: reservas de aulas y turnos, estados por aula, asignación de docentes, mantenimiento y statistics en vivo.

| Capa | Repositorio | Stack |
| :--- | :--- | :--- |
| **Frontend** | [web-sistema-laboratorios](https://github.com/ProyectosCzh/web-sistema-laboratorios) | `Astro 7` `React 19` `TypeScript` `Tailwind 4` `TanStack Query` |
| **API** | [api-sistema-laboratorios](https://github.com/ProyectosCzh/api-sistema-laboratorios) | `Node.js` `Express 5` `TypeScript` `Prisma` `PostgreSQL` `Zod` |

<details>
<summary><b>Detalles técnicos</b></summary>

- **Frontend:** Astro en modo `server` con islas React `client:only`, estado de sesión en `localStorage`, capa de API con interceptores de autenticación y manejos de error, TanStack Query como única fuente de verdad del estado remoto.
- **API:** Express 5 + TypeScript estricto, ORM Prisma sobre PostgreSQL (Neon), caché en memoria con invalidación *write-through* y deduplicación *single-flight*.
- **Seguridad:** doble token (access JWT 15 min + refresh JWT 7 días) con sesiones persistidas, `bcryptjs`, Helmet, CORS con credenciales, *rate limiting* por endpoint y validación Zod en el límite.
- **Documentación:** referencia interactiva con Scalar y especificación OpenAPI 3.x.

</details>

---

<div align="center">

<a href="https://github.com/ProyectosCzh/riskv2cla"><img src="https://opengraph.githubassets.com/1/ProyectosCzh/riskv2cla" alt="SmartRisk" width="100%"></a>
<a href="https://opengraph.githubassets.com/1/ProyectosCzh/backendcanchago" alt="CanchaGo" width="100%"></a>

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

<a href="https://github.com/ProyectosCzh/DocsOrganizator"><img src="https://opengraph.githubassets.com/1/ProyectosCzh/DocsOrganizator" alt="DocsOrganizator" width="100%"></a>
<a href="https://opengraph.githubassets.com/1/ProyectosCzh/Comparativo-Euler-Runge-Kutta" alt="Euler vs Runge-Kutta" width="100%"></a>

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

### Proyectos de estructuras de datos

| Repositorio | Descripción | Stack |
| :--- | :--- | :--- |
| **[Hablacamba · Diccionario del Habla Popular Camba](https://github.com/ProyectosCzh/ProyectoFinalEstructuraAvanzada-Diccionario)** | Tabla hash con manejo de colisiones comparando **listas enlazadas** frente a **árboles AVL**, con búsqueda por *substring* y persistencia en archivo. | `C++` `Python` |
| **[El Tesoro del Pirata](https://github.com/ProyectosCzh/ProyectoFinalEstructuraAvanzada-Pirata)** | Juego de búsqueda de caminos con **BFS** sobre un **grafo ponderado**, mapa interactivo con *pan* y *zoom* sincronizado, y **árbol de pistas n-ario**. | `C++` `Raylib` |

---

## `03` · Stack tecnológico

<div align="center">

| Área | Tecnologías |
| :--- | :--- |
| **Lenguajes** | <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/cpp.svg" width="34" alt="C++" title="C++"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/python.svg" width="34" alt="Python" title="Python"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/csharp/csharp-original.svg" width="34" alt="C#" title="C#"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/javascript.svg" width="34" alt="JavaScript" title="JavaScript"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/typescript.svg" width="34" alt="TypeScript" title="TypeScript"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/dart.svg" width="34" alt="Dart" title="Dart"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/perl.svg" width="34" alt="Perl" title="Perl"> <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="SQL" title="SQL"> |
| **Frontend** | <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/html5.svg" width="34" alt="HTML5" title="HTML5"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/css3.svg" width="34" alt="CSS3" title="CSS3"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/react.svg" width="34" alt="React" title="React"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/astro.svg" width="34" alt="Astro" title="Astro"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/tailwindcss.svg" width="34" alt="Tailwind CSS" title="Tailwind CSS"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/bootstrap.svg" width="34" alt="Bootstrap" title="Bootstrap"> |
| **Backend & APIs** | <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/nodedotjs.svg" width="34" alt="Node.js" title="Node.js"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/express.svg" width="34" alt="Express" title="Express"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/fastapi.svg" width="34" alt="FastAPI" title="FastAPI"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/django.svg" width="34" alt="Django" title="Django"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/dotnet.svg" width="34" alt="ASP.NET Core" title="ASP.NET Core"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/swagger.svg" width="34" alt="Swagger" title="Swagger"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/prisma.svg" width="34" alt="Prisma" title="Prisma"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/zod.svg" width="34" alt="Zod" title="Zod"> |
| **Bases de datos** | <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/postgresql.svg" width="34" alt="PostgreSQL" title="PostgreSQL"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/microsoftsqlserver/microsoftsqlserver-original.svg" width="34" alt="SQL Server" title="SQL Server"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/sqlite.svg" width="34" alt="SQLite" title="SQLite"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/mysql.svg" width="34" alt="MySQL" title="MySQL"> |
| **Datos & Cómputo** | <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/pandas.svg" width="34" alt="Pandas" title="Pandas"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/numpy.svg" width="34" alt="NumPy" title="NumPy"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/scipy.svg" width="34" alt="SciPy" title="SciPy"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/sympy.svg" width="34" alt="SymPy" title="SymPy"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/streamlit.svg" width="34" alt="Streamlit" title="Streamlit"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/plotly.svg" width="34" alt="Plotly" title="Plotly"> |
| **Móvil & Escritorio** | <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/flutter.svg" width="34" alt="Flutter" title="Flutter"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/cplusplus.svg" width="34" alt="C++" title="C++"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/raylib.svg" width="34" alt="Raylib" title="Raylib"> |
| **QA & Herramientas** | <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/pytest.svg" width="34" alt="pytest" title="pytest"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/postman.svg" width="34" alt="Postman" title="Postman"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/git.svg" width="34" alt="Git" title="Git"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/github.svg" width="34" alt="GitHub" title="GitHub"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/vite.svg" width="34" alt="Vite" title="Vite"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/visualstudiocode.svg" width="34" alt="VS Code" title="VS Code"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/rider.svg" width="34" alt="Rider" title="Rider"> |
| **Cloud & Despliegue** | <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/vercel.svg" width="34" alt="Vercel" title="Vercel"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/netlify.svg" width="34" alt="Netlify" title="Netlify"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/render.svg" width="34" alt="Render" title="Render"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/docker.svg" width="34" alt="Docker" title="Docker"> <img src="https://cdn.jsdelivr.net/npm/simple-icons@latest/icons/linux.svg" width="34" alt="Linux" title="Linux"> |

</div>

---

## `04` · Metodología y trayectoria

| Área | Detalle |
| :--- | :--- |
| **Flujo de ingeniería** | Levantamiento de requerimientos, historias de usuario, desarrollo iterativo de MVPs, pruebas de APIs y documentación técnica. |
| **Calidad** | Código limpio, tipado estricto, validación en el límite de la API y pruebas automatizadas. |
| **Documentación** | README técnico por proyecto con arquitectura, modelo de datos, flujo de uso y scripts reproducible. |
| **Desarrollo freelance** | `2025 — Presente` · Aplicaciones a medida, integración de APIs y herramientas de análisis de datos en coordinación directa con clientes. |

---

<div align="center">

### ¿Tienes una idea de proyecto o buscas colaborar en código?

Escríbeme por correo o LinkedIn — respondo siempre.

<br>

<a href="mailto:carlosmzambranah19@gmail.com"><img src="https://img.shields.io/badge/Email-carlosmzambranah19%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>
&nbsp;
<a href="https://www.linkedin.com/in/carlos-mzambrana"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
&nbsp;
<a href="https://github.com/ProyectosCzh"><img src="https://img.shields.io/badge/GitHub-ProyectosCzh-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"></a>

<br><br>

<sub>Hecho con <a href="https://github.com/ProyectosCzh">ProyectosCzh</a></sub>

</div>
