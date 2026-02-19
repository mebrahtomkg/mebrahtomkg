# Hi, I'm Mebrahtom Kidane

### Full-Stack Software Engineer | Software Systems Architect

I am a software engineer dedicated to building high-performance, resilient, and scalable full-stack web applications. I don't just write code; I architect high-end software systems from the ground up, leveraging my deep expertise in the Node.js, React, and Socket.io ecosystems.

## 1. Core Engineering Philosophy

- **Resilience by Design:** I prioritize architectural reliability by decoupling user actions from immediate network dependencies through request-queue-based systems and background processing.

- **Data Integrity & ACID Principles:** I implement strict transactional architectures for all state-mutating operations, utilizing row-level locking and two-phase resource cleanup to guarantee absolute data consistency.

- **Performance Optimization:** I advocate for a "Zero-Lag" philosophy, utilizing dynamic CSS variable injection for theming and hardware-accelerated animation engines that synchronize with the React lifecycle.

- **Type-Safe Scalability:** With a codebase that is 98% TypeScript, I enforce strict typing from the database layer to the UI to significantly reduce runtime exceptions and facilitate long-term maintenance.

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
