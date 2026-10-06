# Hola, soy Santiago 👋

**Software · Web · Automatización · Datos & IA aplicada**
Medellín, Colombia (Remoto) · [santiago.marulandal@udea.edu.co](mailto:santiago.marulandal@udea.edu.co) · +57 300 867 4483

Desarrollador de software con 6+ años en tecnología, datos y educación. Construyo productos reales con IA aplicada: sitios corporativos, landing pages, tiendas online, material educativo digital y plataformas con chatbots y RAG. En Sura automatizé procesos manuales que ocupaban meses de trabajo.

## 🚀 Proyectos Destacados

| Proyecto | Stack | Qué es | Demo |
|----------|-------|--------|------|
| **[Terramind](https://github.com/Marusan94/Terramind)** | `React 18/TS` · `Tailwind` · `FastAPI` · `PostgreSQL/PostGIS` · `Redis` · `Multi-LLM` · `Docker` · `CI/CD` | Calidad del aire con IA: datos en vivo de SIATA (PM2.5/PM10 y AQI por comuna), radar de lluvia, mapa 3D, copiloto con RAG normativo | [Ver en vivo](https://terramind-mu.vercel.app) |
| **[DQ Observatory](https://github.com/Marusan94/dq-observatory)** | `React` · `TypeScript` · `FastAPI` · `Pandas` · `PostgreSQL/SQLite` · `Docker` | Calidad de datos antes de producción: carga CSV/XLSX/JSON, perfilado automático, puntaje por dimensiones, detección de duplicados, vacíos y derivas | [Ver en vivo](https://dq-observatory.onrender.com) |
| **[EDU.CORE](https://github.com/Marusan94/plataforma-estudiantil)** | `Java Spring Boot` · `JPA` · `JavaScript` · `CSS` · `SQL` · `Docker` | Gestión y acompañamiento estudiantil: API REST por capas, autenticación por roles, módulos académicos y frontend con persistencia relacional | [Ver en vivo](https://educore-frontend-co5c.onrender.com) |
| **[Query Lands](https://github.com/Marusan94/query-lands)** | `Next.js` · `TypeScript` · `Tailwind` · `SQLite/WASM` · `Tutor con IA` · `Vitest` | Práctica de SQL gamificada: 16 retos en el navegador + 3 de JS, tutor con IA, repaso espaciado y seguimiento de progreso | [🚀 Live](https://tech-interview-lab.vercel.app) |
| **[Pulso GitHub](https://github.com/Marusan94/pulso-github)** | `Python` · `GitHub API` · `GitHub Actions` · `Playwright` | Ranking en español del ecosistema: 500 repos + 200 tendencias, buscador, analytics y visualización 3D con actualización semanal automática | [Ver en vivo](https://marusan94.github.io/pulso-github/) |
| **[DataFlow](https://github.com/Marusan94/DataFlow)** | `Python` · `Streamlit` · `Pandas` | Hub de analítica de datos agnóstico: analizar → evaluar → asistir → actuar | [Ver en vivo](https://eduanalytics.onrender.com) |

### 🧭 En breve: problema → automatización → resultado

- **Terramind** — Problema: los datos de calidad del aire existen pero nadie los entiende. | Automatización: mapa 3D que se actualiza solo + copiloto multi-LLM con RAG normativo. | Resultado: cualquiera consulta el aire de su ciudad sin saber de datos.
- **DQ Observatory** — Problema: duplicados, vacíos y drift llegan a producción y rompen reportes. | Automatización: subes un CSV y obtienes perfilado, puntaje por dimensiones y alertas. | Resultado: el error se detecta antes de costar dinero.
- **Pulso GitHub** — Problema: nadie mantiene un ranking del open source en español. | Automatización: GitHub Actions lee la API, rankea 500 repos y publica la web. | Resultado: ranking vivo en español, actualizado solo.
- **Query Lands** — Problema: aprender SQL exige instalar entornos y resulta aburrido. | Automatización: 16 retos SQL + 3 de JS en el navegador, con tutor IA que corrige al instante. | Resultado: practicas desde el primer clic, con cero fricción.
- **DataFlow** — Problema: analizar datos exige varias herramientas y saber programar. | Automatización: hub donde subes datos y analizas, evalúas y actúas en un solo lugar. | Resultado: desplegado y usable hoy.

---

### 🔎 Detalle de funcionalidades por proyecto

#### **Terramind** — Inteligencia ambiental Valle de Aburrá
- Datos en vivo: SIATA (PM2.5/PM10, AQI por comuna), Open-Meteo, RainViewer, radar de lluvia
- Mapa 3D interactivo (MapLibre + deck.gl): terreno, edificios extruidos, capas aire/agua/vegetación/comunas
- Copiloto IA multi-LLM (Groq/Gemini/OpenRouter) con RAG normativo (Decreto 1076, guías OMS, ODS) + citas
- 11 tabs dashboard: AQI, historia, alertas, pronóstico 48h/semanal, share links
- Pipeline híbrido: 17 servicios anti-corrupción, simulación determinística, tile cache, SSE streaming
- Demo sin API keys + full stack local (Docker Compose: PostGIS + Redis + FastAPI + Vite)

#### **DQ Observatory** — Puerta de calidad antes de producción
- Ingest: CSV/XLSX/JSON con validación extensión/MIME/size/encoding, hash, versionado
- Profiling determinístico: tipos físico/semántico + confianza, matriz de nulos, duplicados exactos/subconjunto, detectores email/tel/URL/UUID/moneda/%, outliers IQR/Z, PII hints
- Score transparente: completitud 25 + validez 25 + consistencia 20 + unicidad 15 + integridad 15
- Issues explorer: severidad/categoría/columna/estado/auto-fix/búsqueda + paginación, drawer detalle
- Cleaning workspace: preview before/after → apply → nueva versión, undo via lineage, reset v1, audit log
- Drift: schema + distribución (KS, PSI, KL, χ²) entre versiones; correlaciones Pearson/Spearman/Cramér/Theil
- Jobs/webhooks (cron, HMAC, retry exponencial), contratos de datos, AutoML rules, lineage DAG, stream WS
- Export: CSV/XLSX/JSON/Parquet/Delta/Avro/ZIP bundle con filtros y rangos
- Tour guiado 6 pasos + 27 tests backend + 6 E2E Playwright + benchmarks publicados

#### **Pulso GitHub** — Ranking vivo en español, actualizado solo
- Top 500 repos + 200 trending (30d) → fetch GitHub API → taxonomía 17 categorías → descripciones sintéticas en español
- Actualización semanal automática (GitHub Actions lunes 06:00 UTC) → build estático 17 temas + analytics + news + galaxia 3D
- Analytics: curva log-stars con labels, radar por categoría, growth leaders CSV, histograma, serie por repo al click
- Galaxia 3D (`docs/galaxia.html`): 700 estrellas, tamaño=stars, color=lenguaje, search/filtros, camera fly-to, similar-repo links
- Descargas: CSV/Excel/JSON/PDF desde cualquier vista; "My picks" ☆ en localStorage
- 8 E2E Playwright en Chromium real + verify.py (data + JS + tracker + WCAG contrast)

#### **Query Lands** — Práctica SQL/JS gamificada sin instalar
- 16 retos SQL (SELECT → window functions) + 3 retos JS (FizzBuzz, palíndromo, agrupa-y-promedia)
- Validación SQLite WASM en browser (sql.js) + Monaco Editor + tests visibles + ocultos anti-memorización
- Viaje 4 islas animadas (día, faro nocturno, volcán, cristales) + ruta dorada progresiva + velero + tesoro
- Tutor IA socrático (Gemini Flash): pistas progresivas, explicación paso a paso, generador retos auto-validados
- Simulacro 45 min: 4 retos mixtos + corrección IA con rúbrica detallada
- Gamificación: XP, niveles/100, racha + heatmap 8 sem, monedas, logros, misiones diarias, certificado imprimible
- Accesibilidad: modo calma, foco visible, skip-link, texto escalable, sonido off, reduced-motion, tema claro/oscuro yin-yang
- 22 tests Vitest + ESLint 9 + TS strict + deploy automático Vercel

#### **DataFlow** — Hub analítica self-service para cualquier CSV
- Flujo unificado: Analizar → Evaluar → Asistir → Actuar (4 tipos de proyecto agnósticos)
- Perfilado: tipos, nulos, duplicados, categorías, numéricos, fechas + visualizaciones Plotly interactivas
- Chat IA opcional (OpenRouter) con fallback local sin API key
- Auth simulada 7 pantallas (login/registro/2FA/recupero) + 4 roles: Analista/Desarrollador/Estudiante/Investigador
- Dataset de ejemplo (`datos_ejemplo.csv`: ventas genéricas) para probar sin subir nada
- Deploy Render (`render.yaml`), runtime python-3.11.9, MIT license

## 💼 Experiencia

**Analista TI — SURA** · Jul 2023 – Dic 2024 · 1 año 6 meses
Interfaces React conectadas a servicios backend e integración de APIs. Automatización con Python y RPA (UiPath) para tareas operativas. SQL, reportes, KPIs y mesa de ayuda: atención de tickets en producción bajo SLA.

**Customer Service — Bancolombia** · Jul 2021 – Oct 2023 · 2 años 4 meses
Resolución y escalamiento de tickets con seguimiento de SLA. Análisis de casos en bases de datos para diagnóstico y reportes. Monitoreo de KPIs de servicio en Excel y análisis de indicadores de calidad.

**Customer Service — Tigo** · Oct 2019 – Jun 2021 · 1 año 9 meses
Análisis de casos y reportes de operación en Excel para el seguimiento de indicadores. Gestión de tickets y escalamiento a áreas técnicas. Medición de KPIs de satisfacción y tiempos de resolución.

**Tutor TI de Programación — Cymetria** · Ene – Jun 2026 · 6 meses
Diseño de cursos y materiales: lógica de programación, Python y análisis de datos. Dirección técnica de desarrollos llevados a despliegue.

**Tutor TI — AlgoNova** · Nov 2025 – Ago 2026 · 10 meses
Escuela internacional online (90+ países). Python, Roblox Studio (Lua, mundos 3D) y Scratch. Sesiones en vivo y seguimiento del progreso de cada estudiante.

**Coordinador de plataforma de inscripción — Smart Films** · Jun – Sep 2025 · 4 meses
Administración de plataforma en WordPress: contenidos, usuarios y formularios. Base de datos de inscritos y producción audiovisual del festival.

**STEM Teacher — Colegio Rafael Uribe Uribe** · 2023 · 1 año
Docencia en Ciencias Naturales y Educación Ambiental. Diseño de guías, talleres y evaluaciones.

## 🎓 Educación y Certificaciones

- Lic. Ciencias Naturales y Ed. Ambiental — Universidad de Antioquia, 2025
- Técnico en Desarrollo de Software — Cesd, 2024
- Examen de competencia lectora en inglés — Escuela de Idiomas, UdeA, 2026
- Claude 101 — Anthropic, 2026
- WordPress No-Code — Platzi, 2025
- SQL/MySQL · FastAPI · Python · Java Spring — Platzi, 2024

## 🛠️ Stack

**Programación** — React 18 · TypeScript · JavaScript · Tailwind · HTML/CSS responsive · Python · FastAPI · APIs REST · SQL/MySQL · PostgreSQL · POO · WordPress · Elementor · WooCommerce

**Automatización y RPA** — Python (scripts, ETL, scraping) · UiPath · n8n (webhooks, Docker) · integración de APIs · chatbots y asistentes con LLMs (Groq, Gemini, OpenRouter)

**DevOps y calidad** — Git/GitHub · Actions (CI/CD) · Docker · Vercel/Render · Vitest · Playwright E2E

**Diseño, 3D y contenido** — Usabilidad y mobile-first · Figma · modelado de mundos 3D (Roblox Studio) · creación por bloques (Scratch) · producción y edición audiovisual · copy web y redes

## 🏆 Logros

- **SURA:** automatizé procesos manuales engorrosos y reduje meses de trabajo a una semana.
- **SURA:** despejé el backlog vencido con automatización y SQL; tiempo y calidad mejorados en 40%, equipo en 98%.
- **Tigo y Bancolombia:** elevé la calidad del servicio a 98% con seguimiento de indicadores.
- Formación y certificación de estudiantes internacionales de Latinoamérica.

## 🌐 Idiomas

Español — Nativo · Inglés — B2+ técnico

## 📫 Contacto

- **LinkedIn:** [santi-marulanda](https://linkedin.com/in/santi-marulanda)
- **Email:** santiago.marulandal@udea.edu.co
- **Teléfono:** +57 300 867 4483
- **GitHub:** [Marusan94](https://github.com/Marusan94)