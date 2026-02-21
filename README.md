# Hi, I'm Mebrahtom Kidane

### Full-Stack Software Engineer | Software Systems Architect

I architect high-end, resilient software systems from the ground up. With deep expertise in the **Node.js**, **React**, and **Socket.io** ecosystems, I specialize in building full-stack applications where high performance and scalability aren't just features—they are the foundation.

## 1. Core Engineering Philosophy

- **Performant UI/UX & Aesthetic Animation:**

  - Animation is used intentionally to reduce cognitive load and provide clear visual feedback for every user interaction.

  - I prioritize 60fps consistency by utilizing hardware-accelerated transitions and minimizing main-thread blocking.

- **High-Performance Engineering:**

  - I prioritize maximum performance across the entire stack, from optimized backend queries to ultra-responsive frontend logic.

  - Every line of code, whether on the client or the server, is engineered for peak efficiency, delivering a seamless, high-velocity system.

- **Readable, Modular, and Scalable Code:**

  - I prioritize code that is easy to understand and maintain over unnecessarily complex solutions.

  - Guided by DRY (Don't Repeat Yourself) and Single Responsibility principles, I break logic into small, focused files rather than bloated, multi-hundred-line components.

  - This ensures that even a system with 500+ source files never feels like a "blackbox," but rather a collection of transparent, well-defined models and subsystems that are easy to navigate and scale.

- **TypeScript over Vanilla JS:**

  - I utilize TypeScript to build self-documenting, robust codebases.

  - By enforcing strict typing from the database layer to the UI, I eliminate the unpredictability of vanilla JavaScript. This end-to-end predictability provides the confidence required for fearless refactoring and long-term maintenance.

- **Data Integrity & Resilience:**

  - I address edge cases at the architectural level. I implement strict transactional architectures and row-level locking to guarantee absolute consistency.

  - By treating "unhappy paths" as first-class citizens, I build systems that neutralize failures before they reach the user.

## 2. Technology Stack

| Category            | Tools & Technologies                                                      |
| :------------------ | :------------------------------------------------------------------------ |
| **Languages**       | TypeScript (Expert), JavaScript (Expert/ES6+)                             |
| **Frontend**        | React (Specialist), Zustand, React Query, Styled Components, React Router |
| **Backend**         | Node.js, ExpressJS, Socket.io (Real-time)                                 |
| **Database/ORM**    | Sequelize (PostgreSQL, MySQL, SQLite)                                     |
| **Validation**      | Zod                                                                       |
| **Infrastructure**  | Supabase Storage, Local Disk Storage, Service Workers                     |
| **Build Tools**     | Rspack, SWC, SVGR, Biome, Prettier                                        |
| **Design & Assets** | Inkscape (High-Fidelity SVG Iconography & Vector Design)                  |

## 3. Featured Project: [SemayChat](https://github.com/mebrahtomkg/semaychat)

SemayChat is a high-performance, real-time messaging platform engineered for reliability and user privacy. This project serves as a comprehensive demonstration of my ability to architect and deploy complex, production-grade full-stack systems from the ground up.

- **Advanced Message Queuing:** When a user writes, edits, or deletes a message and hits a button, the project doesn't just make an API call. Instead, it queues these actions into a global Zustand-based store, where a background processor executes them sequentially. This ensures strict **FIFO ordering** and automatic retries upon network restoration to maintain data integrity.

- **Database-Agnostic Architecture:** Leveraged Sequelize to support PostgreSQL, MySQL, and even SQLite, enabling flexible, environment-specific deployments without code changes.

- **Storage-Agnostic File Management:** Engineered a provider-based abstraction layer supporting both local disk and Supabase cloud storage, optimized via a **Service Worker-driven** caching layer for high-speed media delivery.

- **Custom Build Pipeline:** Developed a specialized **Rspack plugin** for Service Worker orchestration, ensuring seamless asset caching and maintaining Hot Module Replacement (HMR) compatibility during development.

- **Granular Privacy Framework:** Built a robust management system allowing users to independently control the visibility of their email, "last seen" status, and profile assets.

- Manages over 500 source files while maintaining a premium UI/UX and **ACID-compliant** transactions for all backend operations.
