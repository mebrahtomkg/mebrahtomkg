# Hi, I'm Mebrahtom Kidane

### Full-Stack Software Engineer | Software Systems Architect

I am a software engineer dedicated to building high-performance, resilient, and scalable full-stack web applications. I don't just write code; I architect high-end software systems from the ground up, leveraging my deep expertise in the Node.js, React, and Socket.io ecosystems.

## 1. Core Engineering Philosophy

- **Full-Stack Performance & Fluidity:** I advocate for a "Zero-Lag" philosophy across the entire stack, from optimized backend queries to ultra-responsive frontends. I believe software should feel as good as it looks; therefore, I utilize hardware-accelerated animations and efficient state management to ensure every interaction is smooth and intentional. To me, "done" means the system is not just functional, but attractive and high-performing, ensuring a premium experience that never feels sluggish or unpolished.

- **Readable, Modular, and Scalable Architecture:** I prioritize code that is easy to understand and maintain over unnecessarily complex solutions. Guided by DRY (Don't Repeat Yourself) and Single Responsibility principles, I break logic into small, focused files rather than bloated, multi-hundred-line components. This ensures that even a system with 500+ source files never feels like a "blackbox," but rather a collection of transparent, well-defined models and subsystems that are easy to navigate and scale.

- **TypeScript over Vanilla JS:** I favor TypeScript to ensure a self-documenting, robust codebase where the architecture is easy to understand and navigate. By enforcing strict typing from the database layer to the UI, I eliminate the unpredictability of vanilla JavaScript and catch errors during development rather than in production. This approach guarantees end-to-end predictability and provides the developer confidence required for fearless refactoring and simplified long-term maintenance.

- **Data Integrity & Proactive Error Resilience:** I handle edge cases at the architectural level before a single line of code reaches the testing phase. I implement strict transactional architectures for all state-mutating operations—following the "all-or-nothing" principle—utilizing row-level locking and two-phase resource cleanup to guarantee absolute consistency. By treating "unhappy paths" as first-class citizens during development, I neutralize failures at the source, ensuring the system remains stable and predictable under any condition.

## 2. Technology Stack

| Category           | Tools & Technologies                                         |
| :----------------- | :----------------------------------------------------------- |
| **Languages**      | TypeScript (98% of codebase), JavaScript                     |
| **Frontend**       | React, Zustand, React Query, Styled Components, React Router |
| **Backend**        | Node.js, ExpressJS, Socket.io (Real-time)                    |
| **Database/ORM**   | Sequelize (PostgreSQL, MySQL, SQLite), Zod                   |
| **Infrastructure** | Supabase Storage, Local Disk Storage, Service Workers        |
| **Build Tools**    | Rspack, SWC, SVGR, Biome, Prettier                           |

## 3. Featured Project: [SemayChat](https://github.com/mebrahtomkg/semaychat)

SemayChat is a high-performance, real-time messaging platform engineered for reliability and user privacy. This project serves as a comprehensive demonstration of my ability to architect and deploy complex, production-grade full-stack systems from the ground up.

- **Advanced Message Queuing:** When a user writes, edits, or deletes a message and hits a button, the project doesn't just make an API call. Instead, it queues these actions into a global Zustand-based store, where a background processor executes them sequentially. This ensures strict **FIFO ordering** and automatic retries upon network restoration to maintain data integrity.

- **Database-Agnostic Architecture:** Leveraged Sequelize to support PostgreSQL, MySQL, and even SQLite, enabling flexible, environment-specific deployments without code changes.

- **Storage-Agnostic File Management:** Engineered a provider-based abstraction layer supporting both local disk and Supabase cloud storage, optimized via a **Service Worker-driven** caching layer for high-speed media delivery.

- **Custom Build Pipeline:** Developed a specialized **Rspack plugin** for Service Worker orchestration, ensuring seamless asset caching and maintaining Hot Module Replacement (HMR) compatibility during development.

- **Granular Privacy Framework:** Built a robust management system allowing users to independently control the visibility of their email, "last seen" status, and profile assets.

> **Architectural Note:** The project manages over 500 source files, delivering a high-end UI/UX while ensuring **ACID-compliant transactions** for all backend data operations.
