# Hi, I'm Mebrahtom Kidane

### Full-Stack Software Engineer | Software Systems Architect

I architect high-end, resilient software systems from the ground up. With deep expertise in the **Node.js**, **React**, and **TypeScript** ecosystems, I specialize in building full-stack applications and developer tooling where high performance and scalability aren't just features—they are the foundation.

## 1. Core Engineering Philosophy

- **Performant UI/UX & Aesthetic Animation:**

  - Animation is used intentionally to reduce cognitive load and provide clear visual feedback for every user interaction.

  - I prioritize 60fps consistency by utilizing hardware-accelerated transitions and minimizing main-thread blocking.

- **High-Performance Engineering:**

  - I prioritize maximum performance across the entire stack, from optimized backend queries to ultra-responsive frontend logic and background services.

  - Every line of code, whether on the client or the server, is engineered for peak efficiency, delivering a seamless, high-velocity system.

- **Readable, Modular, and Scalable Code:**

  - I prioritize code that is easy to understand and maintain over unnecessarily complex solutions.

  - Guided by **DRY** (Don't Repeat Yourself) and Single Responsibility principles, I break logic into small, focused modules rather than bloated, multi-hundred-line components.

  - This ensures that even a system with 500+ source files remains transparent, well-defined, and easy to navigate.

- **TypeScript over Vanilla JS:**

  - I utilize TypeScript to build self-documenting, robust codebases.

  - By enforcing strict typing from the database layer to the UI, I eliminate the unpredictability of vanilla JavaScript. This end-to-end predictability provides the confidence required for fearless refactoring.

- **Data Integrity & Resilience:**

  - I address edge cases at the architectural level. I implement strict transactional architectures and robust error-handling to guarantee absolute consistency.

  - By treating "unhappy paths" as first-class citizens, I build systems that neutralize failures before they reach the user.

## 2. Technology Stack

| Category            | Tools & Technologies                                           |
| :------------------ | :------------------------------------------------------------- |
| **Languages**       | TypeScript, JavaScript (ES6+)                                  |
| **Frontend**        | React, Zustand, React Query, Styled Components, React Router   |
| **Backend**         | Node.js, ExpressJS, Socket.io (Real-time), REST APIs           |
| **Static Analysis** | TypeScript Compiler API (AST Traversal), Prettier API          |
| **Database/ORM**    | Sequelize (PostgreSQL, MySQL, SQLite)                          |
| **Validation**      | Zod                                                            |
| **Infrastructure**  | Supabase Storage, Service Workers, Multi-process Orchestration |
| **Build Tools**     | Rspack, SWC, SVGR, Biome, Prettier                             |
| **Design & Assets** | Inkscape (High-Fidelity SVG Iconography & Vector Design)       |

## 3. Featured Projects

### 3.1. [SemayChat](https://github.com/mebrahtomkg/semaychat)

SemayChat is a high-performance, real-time messaging platform engineered for reliability and user privacy. This project serves as a comprehensive demonstration of my ability to architect and deploy complex, production-grade full-stack systems from the ground up.

<p align="center">
  <img src="https://github.com/user-attachments/assets/08ba9551-303a-4a5b-8ba1-7f71e303a3b2" alt="SemayChat App Preview" width="800">
</p>

- **Architectural Details**

  - **Advanced Message Queuing:** When a user writes, edits, or deletes a message and hits send button, the project doesn't just make an API call. Instead, it queues these actions into a global Zustand-based store, where a background processor executes them sequentially. This ensures strict **FIFO ordering** and automatic retries upon network restoration to maintain data integrity.

  - **Database-Agnostic Architecture:** Leveraged Sequelize to support PostgreSQL, MySQL, and even SQLite, enabling flexible, environment-specific deployments without code changes.

  - **Storage-Agnostic File Management:** Engineered a provider-based abstraction layer supporting both **Local disk** and **Supabase cloud storage**, optimized via a **Service Worker-driven** caching layer for high-speed media delivery.

  - **Custom Build Pipeline:** Developed a specialized **Rspack plugin** for Service Worker orchestration, ensuring seamless asset caching and maintaining Hot Module Replacement (HMR) compatibility during development.

  - **Granular Privacy Framework:** Built a robust management system allowing users to independently control the visibility of their email, "last seen" status, and profile assets.

  - Manages over 500 source files while maintaining a premium UI/UX and **ACID-compliant** transactions for all backend operations.

### 3.2. [SpeedyDevHook](https://github.com/mebrahtomkg/speedy-dev-hook)

A high-performance **Sublime Text plugin** designed to transform the lightweight editor into a high-end IDE comparable to VS Code, specifically for **Web Development and JavaScript/TypeScript projects**. It bridges Sublime’s agility with a Node.js background service to provide deep code intelligence without compromising speed.

- **Core Feature Set:**

  - **Smart Select:** Employs AST-powered logic to intelligently expand text selections based on code hierarchy (functions, arrays, objects), going far beyond simple regex matching.

  - **Seamless Formatting:** Offloads **Prettier** execution to a background Node.js instance, allowing for high-fidelity code formatting across dozens of file types without blocking the editor UI.

  - **Task Management (List Scripts):** Dynamically scans the project for `package.json` files and provides a native quick-panel to browse all available `npm` scripts.

  - **Integrated Execution:** Launches scripts directly into native terminal emulators (CMD, Terminal.app, Gnome-terminal, etc.) using a transactional spawning strategy that persists independently of the editor.

- **Architectural Details**

  - **Ultra-Fast Client-Server Architecture:** By utilizing a persistent Node.js background service instead of spawning new processes for every action, the system eliminates cold-start overhead. This architecture delivers near-instantaneous performance:

    - **Code Formatting:** < 80ms.
    - **Smart-Select:** < 40ms.
    - **List-Scripts:** < 50ms.

  - **AST-Driven Intelligence:** Utilizes the **TypeScript Compiler API** to perform structural code analysis, enabling "Smart Selection" that understands code hierarchy (functions, objects, arrays) far beyond regex capabilities.

  - **Hybrid Client-Server Lifecycle:** Engineered a resource-aware architecture using a **Python-based heartbeat system** and Node.js middleware to manage an auto-shutdown mechanism, ensuring zero idle resource consumption.

  - **Non-Blocking Performance:** Offloads heavy tasks like Prettier formatting and AST parsing to a background process, maintaining a lag-free, 60fps editing experience in the host editor.

  - **Cross-Platform Orchestration:** Features a robust terminal spawning system that handles native terminal emulation across Windows, macOS, and Linux, independent of the parent process.

  - **Optimized Build Pipeline:** Bundled with **Rspack and SWC** into a single optimized CommonJS execution unit to minimize startup latency and dependency overhead.
