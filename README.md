# Ezequiel Vecchio

<p align="center">
  <strong>Software Developer & AI Architect · E-Commerce Optimization · Local-First Systems</strong>
</p>

<p align="center">
  <a href="#english">🇺🇸 English</a> • <a href="#español">🇪🇸 Español</a>
</p>

---

<h2 id="english" align="center">🇺🇸 English Version</h2>

I am a Software Developer and Architect based in Argentina. I design modular, high-performance software systems—which I refer to as **Blueprints**—tailored to optimize conversions, automate operations with private artificial intelligence, and protect user data via local-first design architectures.

I build software that balances production reliability with user privacy, focusing on robust data structures, edge architectures, and smooth user experiences.

---


### Integrable Solutions (Blueprints)

*   **[NubeBoost](https://github.com/Evecchio/nubeboost)** — Checkout and load-speed optimization framework for Tiendanube. Re-engineers visual hierarchy and user flows to reduce cart abandonment by up to 35%.
*   **[CoreStore Headless](https://github.com/Evecchio/corestore-headless)** — Ultra-fast headless e-commerce frontend built with **Next.js 15**, **React 19**, and **TypeScript**. Focuses on offline-persistent carts, immediate loading, and SEO optimization.
*   **[FlowCommerce](https://github.com/Evecchio/flowcommerce)** — AI-powered WhatsApp sales automation. Converts informal chat conversations into structured, automated orders.
*   **[SpendGuard Mobile](https://github.com/Evecchio/spendguard-mobile)** — A 100% private expense tracker written in **Kotlin** and **Jetpack Compose**. Listens to local bank notifications in the background, extracts transaction details via Regex, and stores data in a local encrypted **Room DB**.
    ```mermaid
    sequenceDiagram
        autonumber
        participant App as Bank App
        participant OS as Android OS
        participant Service as Background Listener Service
        participant Parser as Regex Engine
        participant DB as Encrypted Room DB
        
        App->>OS: Trigger Transaction Notification
        OS->>Service: Intercept Notification Event
        Service->>Parser: Extract Notification Text
        Parser->>Parser: Process Regex (Amount, Date, Merchant)
        Parser->>DB: Save Encrypted Record
    ```
*   **[SafeRAG Local](https://github.com/Evecchio/saferag-local)** — A fully offline corporate assistant. Combines **FastAPI**, **Ollama**, and **Chroma DB** to parse documents and answer queries locally without network requests.
    ```mermaid
    graph TD
        subgraph Ingestion ["1. Local Ingest (Offline)"]
            Doc["User Documents"] --> Parser["PDF/Text Parser"]
            Parser --> Splitter["Text Splitter"]
            Splitter --> Embedder["Local Embedder"]
            Embedder --> VectorDB[("Local Chroma DB")]
        end
        subgraph Pipeline ["2. Query & Generation (Offline)"]
            Query["User Query"] --> EmbedQuery["Embed Query"]
            EmbedQuery --> VectorDB
            VectorDB --> Context["Context Retrieval"]
            Context --> LLM["Local Ollama LLM"]
            Query --> LLM
            LLM --> Response["Response"]
        end
    ```
*   **[DropLand](https://github.com/Evecchio/DropLand)** — Local network downloader. Written in **Python** and **Tkinter**, it runs a lightweight web server that allows users to manage, convert, and trigger media downloads from any mobile device on the network.
*   **[DRDV Framework](https://github.com/Evecchio/drdv-framework)** — A YAML-based validation runtime for multi-agent LLM systems. Enforces strict behavior contracts through the *Design-Review-Decide-Validate* lifecycle.
    ```mermaid
    stateDiagram-v2
        [*] --> Design : Agent Request
        Design --> Review : Spec Created
        Review --> Decide : Behavior Checks Passed
        Decide --> Validate : Decision Logged
        Validate --> Execution : Verified Contract Compliance
        Execution --> [*]
    ```
*   **[ZenSpend Engine](https://github.com/Evecchio/zenspend-engine)** — Offline-first database design and local AI viability research MVP for corporate finance.

---

### Technical toolkit

These are the technologies I use across high-performance web applications, local AI integrations, mobile development, and systems engineering.

**Frontend and Design**
<p>
  <a href="https://react.dev/"><img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React" /></a>
  <a href="https://nextjs.org/"><img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" /></a>
  <a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" /></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"><img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" /></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/HTML"><img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" /></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/CSS"><img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" /></a>
</p>

**Backend and AI**
<p>
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" /></a>
  <a href="https://fastapi.tiangolo.com/"><img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" /></a>
  <a href="https://ollama.com/"><img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" alt="Ollama" /></a>
  <a href="https://www.trychroma.com/"><img src="https://img.shields.io/badge/Chroma_DB-FFDE4D?style=for-the-badge" alt="Chroma DB" /></a>
</p>

**Mobile and Local-First**
<p>
  <a href="https://kotlinlang.org/"><img src="https://img.shields.io/badge/Kotlin-0095D5?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin" /></a>
  <a href="https://developer.android.com/compose"><img src="https://img.shields.io/badge/Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white" alt="Jetpack Compose" /></a>
  <a href="https://developer.android.com/training/data-storage/room"><img src="https://img.shields.io/badge/Room_DB-003B57?style=for-the-badge&logo=sqlite&logoColor=white" alt="Room DB" /></a>
  <a href="https://developer.android.com/"><img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android" /></a>
</p>

**DevOps and Distribution**
<p>
  <a href="https://git-scm.com/"><img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" /></a>
  <a href="https://github.com/features/actions"><img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions" /></a>
</p>

---

### Find me online

<p align="center">
  <a href="https://evecchio.github.io/FVision-Builders/"><img src="https://img.shields.io/badge/Portfolio-111827?style=for-the-badge&logo=firefoxbrowser&logoColor=white" alt="Portfolio" /></a>
  <a href="https://github.com/Evecchio"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="mailto:eivec@hotmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

<p align="center">
  Argentina · UTC−3
</p>

---
---

<h2 id="español" align="center">🇪🇸 Versión en Español</h2>

Soy desarrollador de software y arquitecto de sistemas basado en Argentina. Me especializo en diseñar arquitecturas modulares de alto rendimiento—a las que llamo **Blueprints**—enfocadas en maximizar conversiones en e-commerce, automatizar operaciones con inteligencia artificial privada y proteger la privacidad de los datos mediante sistemas local-first.

Creo código estructurado que equilibra la estabilidad en producción con la privacidad absoluta del usuario final.


### Soluciones Integrables (Blueprints)

*   **[NubeBoost](https://github.com/Evecchio/nubeboost)** — Optimizador de velocidad y checkout para Tiendanube. Modifica la jerarquía visual y los flujos UX reduciendo el abandono de carrito hasta en un 35%.
*   **[CoreStore Headless](https://github.com/Evecchio/corestore-headless)** — Frontend headless de alta velocidad desarrollado con **Next.js 15**, **React 19** y **TypeScript**. Incorpora carrito de compras persistente offline y SEO optimizado.
*   **[FlowCommerce](https://github.com/Evecchio/flowcommerce)** — Automatización de ventas por WhatsApp con Inteligencia Artificial. Convierte chats informales en pedidos estructurados y automatizados.
*   **[SpendGuard Mobile](https://github.com/Evecchio/spendguard-mobile)** — Gestor de finanzas personales 100% privado en **Kotlin** y **Jetpack Compose**. Escucha notificaciones bancarias en segundo plano, extrae datos mediante Regex y los almacena localmente en una base de datos cifrada **Room**.
    ```mermaid
    sequenceDiagram
        autonumber
        participant App as Bank App
        participant OS as Android OS
        participant Service as Background Listener Service
        participant Parser as Regex Engine
        participant DB as Encrypted Room DB
        
        App->>OS: Trigger Transaction Notification
        OS->>Service: Intercept Notification Event
        Service->>Parser: Extract Notification Text
        Parser->>Parser: Process Regex (Amount, Date, Merchant)
        Parser->>DB: Save Encrypted Record
    ```
*   **[SafeRAG Local](https://github.com/Evecchio/saferag-local)** — Asistente de IA documental completamente offline. Integra **FastAPI**, **Ollama** y **Chroma DB** para procesar y responder consultas sobre documentos corporativos localmente.
    ```mermaid
    graph TD
        subgraph Ingestion ["1. Local Ingest (Offline)"]
            Doc["User Documents"] --> Parser["PDF/Text Parser"]
            Parser --> Splitter["Text Splitter"]
            Splitter --> Embedder["Local Embedder"]
            Embedder --> VectorDB[("Local Chroma DB")]
        end
        subgraph Pipeline ["2. Query & Generation (Offline)"]
            Query["User Query"] --> EmbedQuery["Embed Query"]
            EmbedQuery --> VectorDB
            VectorDB --> Context["Context Retrieval"]
            Context --> LLM["Local Ollama LLM"]
            Query --> LLM
            LLM --> Response["Response"]
        end
    ```
*   **[DropLand](https://github.com/Evecchio/DropLand)** — Gestor de descargas en red local. Escrito en **Python** y **Tkinter**, monta un servidor web liviano para controlar, convertir y programar descargas multimedia de forma remota desde cualquier móvil en la red.
*   **[DRDV Framework](https://github.com/Evecchio/drdv-framework)** — Runtime de gobernanza basado en YAML para sistemas multi-agente de LLM. Valida contratos de comportamiento bajo el ciclo *Design-Review-Decide-Validate*.
    ```mermaid
    stateDiagram-v2
        [*] --> Design : Agent Request
        Design --> Review : Spec Created
        Review --> Decide : Behavior Checks Passed
        Decide --> Validate : Decision Logged
        Validate --> Execution : Verified Contract Compliance
        Execution --> [*]
    ```
*   **[ZenSpend Engine](https://github.com/Evecchio/zenspend-engine)** — Diseño de bases de datos offline-first e investigación de viabilidad de IA local para finanzas corporativas.

---

### Toolkit técnico

Estas son las tecnologías que utilizo en el desarrollo de aplicaciones web de alto rendimiento, integraciones de IA local, desarrollo móvil y arquitectura de sistemas.

**Frontend y Diseño**
<p>
  <a href="https://react.dev/"><img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React" /></a>
  <a href="https://nextjs.org/"><img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white" alt="Next.js" /></a>
  <a href="https://www.typescriptlang.org/"><img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" /></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript"><img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" /></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/HTML"><img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" /></a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/CSS"><img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" /></a>
</p>

**Backend e IA**
<p>
  <a href="https://www.python.org/"><img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" /></a>
  <a href="https://fastapi.tiangolo.com/"><img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" /></a>
  <a href="https://ollama.com/"><img src="https://img.shields.io/badge/Ollama-000000?style=for-the-badge&logo=ollama&logoColor=white" alt="Ollama" /></a>
  <a href="https://www.trychroma.com/"><img src="https://img.shields.io/badge/Chroma_DB-FFDE4D?style=for-the-badge" alt="Chroma DB" /></a>
</p>

**Móvil y Local-First**
<p>
  <a href="https://kotlinlang.org/"><img src="https://img.shields.io/badge/Kotlin-0095D5?style=for-the-badge&logo=kotlin&logoColor=white" alt="Kotlin" /></a>
  <a href="https://developer.android.com/compose"><img src="https://img.shields.io/badge/Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white" alt="Jetpack Compose" /></a>
  <a href="https://developer.android.com/training/data-storage/room"><img src="https://img.shields.io/badge/Room_DB-003B57?style=for-the-badge&logo=sqlite&logoColor=white" alt="Room DB" /></a>
  <a href="https://developer.android.com/"><img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android" /></a>
</p>

**DevOps y Distribución**
<p>
  <a href="https://git-scm.com/"><img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" /></a>
  <a href="https://github.com/features/actions"><img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions" /></a>
</p>

---

### Dónde encontrarme

<p align="center">
  <a href="https://evecchio.github.io/FVision-Builders/"><img src="https://img.shields.io/badge/Portfolio-111827?style=for-the-badge&logo=firefoxbrowser&logoColor=white" alt="Portafolio" /></a>
  <a href="https://github.com/Evecchio"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="mailto:eivec@hotmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

<p align="center">
  Argentina · UTC−3
</p>
