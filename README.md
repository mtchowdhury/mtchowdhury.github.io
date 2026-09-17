# Lead Software Engineer

Berlin, Germany · [LinkedIn](https://www.linkedin.com/in/tawhid-chowdhury-) · [cmdtawhid@gmail.com](mailto:cmdtawhid@gmail.com)

9+ years architecting and shipping scalable systems across fintech, enterprise SaaS and
AI-driven platforms. I lead engineering teams, mentor developers, and turn complex, ambiguous
problems into production systems — architecture and strategy through implementation and
operations. EU Blue Card holder, available immediately.

#### Technical Skills
**Languages & frameworks:** C#, .NET 8, ASP.NET Core, EF Core, TypeScript, Angular, NgRx, React
**AI engineering:** LLM fine-tuning, agentic systems & tool calling, RAG, vector search, Model Context Protocol (MCP)
**Data:** PostgreSQL, SQL Server, Redis, MongoDB, Elasticsearch, pgvector
**Cloud & DevOps:** Azure, Azure DevOps, AWS S3, Docker, CI/CD, RabbitMQ
**Leadership:** team leadership, hiring & technical interviewing, Agile process design, code review


## Work Experience
**Lead Software Engineer @ Noca GmbH (_Dec 2024 - Present_)**
- Rebuilt the company's core ERP/PIM platform into a production .NET, Angular and PostgreSQL system, leading a small team through architecture, code review and delivery
- Designed an AI-driven data ingestion feature: customers upload product sheets in any format or language, and a fine-tuned LLM maps them onto internal data entities for review and import, replacing manual re-keying entirely
- Built the supporting AI platform — a provider-agnostic abstraction over Anthropic, Mistral and Moonshot, a Model Context Protocol (MCP) server, and a RAG pipeline using vector embeddings (pgvector)
- Owned infrastructure end to end: Dockerised CI/CD on Azure DevOps across multiple Linux servers, health-gated rolling deployments for zero-downtime releases, and PostgreSQL mirroring
- Established the engineering process from scratch — a custom Agile workflow in Azure Boards, sprint planning and standups — plus the hiring pipeline: designed the technical interview, evaluated candidates, onboarded and mentored engineers
- [www.noca-mobility.com](https://www.noca-mobility.com)

**Senior Developer @ Optimizely Inc. (_May 2023 - Feb 2024_)**
- Designed and developed scalable backend services for Optimizely's Content and Commerce Cloud platforms, leveraging .NET Core, MSSQL, Elasticsearch, and Azure to ensure high availability and performance.
- Contributed to migrating legacy systems onto a modern, scalable architecture, improving flexibility and maintainability.
- Collaborated on API development for headless CMS integration with front-end frameworks like React and Angular, enhancing content delivery speed and efficiency.
- Engaged in technical architecture discussions, implemented SaaS-based solutions, and ensured adherence to industry best practices across the development team.
- Improved code quality and performance through continuous integration, automated testing and performance tuning, shortening deployment cycles.
- [www.optimizely.com](https://www.optimizely.com)

**Software Engineer @ ASAI Management Services Ltd. (_Nov 2020 - Apr 2023_)**
- Designed and developed micro-service-based financial solutions using .NET Core, Angular, MSSQL, and MongoDB, following the Saga pattern and clean architecture principles
- Developed a real-time data pulling service architecture for consolidating financial data from multiple servers across different countries, using .Net Core, message broker (RabbitMQ) and ELK stack. This portal automated the whole manual report consolidation process organization-wide
- Developed back-end services for report generation from across 13 countries financial and operational data with complex and dynamic query and stored procedures with SQL and .Net Core
- Coordinated with cross-functional (QA, Implementation, BA, Operations etc.) teams to ensure seamless integration and deployment of new features
- [www.asa-international.com](www.asa-international.com)

**Software Engineer @ M2SYS Technology (_Mar 2020 - Nov 2020_)**
- Developed and maintained a Drag-and-Drop SaaS platform using Angular, .NET Core, PostgreSQL, and Apache Solr
- Developed cross-platform desktop applications using Electron JS, enhancing user experience and application performance
- Collaboration with product managers to define project requirements and deliver software solutions on time
- [www.m2sys.com](www.m2sys.com)

**Asst. Software Engineer @ ASA Bangladesh (_Jan 2017 - Feb 2020_)**
-  Designed and developed next-generation enterprise solution using .Net, AngularJS, MSSQL, responsible for managing daily operation of core financial services, running in over 3200+ branches
- Collaboration in data migration of over 16 years of data using SQL scripting and long running scheduler services, from offline branch system to online system
- [asa.org.bd](https://asa.org.bd)



## Education
- B.Sc. Computer Science and Engineering | American International University-Bangladesh (_Sep 2011 - Dec 2015_)

## Certifications
- Optimizely Certified Content Cloud Developer
- Top-Up IT Training (LICT, Employment and Governance Project, BD) | Native Android Application Development (180 Hrs.)


## Projects

### Personal AI Assistant (personal project)
- Self-hosted assistant I built for my own use and run daily — expenses, tasks and structured notes, with an AI layer that reads and writes them through tool calling

- .NET 8 API, Angular 17 web client, Flutter iOS app, PostgreSQL + pgvector
- Provider-agnostic AI layer (Anthropic, Mistral) on Microsoft.Extensions.AI: adding a provider is one builder class, the chat service is untouched
- AI tools are deliberately read + add only — no update, delete or merge tool, so a model error or a prompt injection in an uploaded receipt cannot destroy existing records
- Photograph a receipt and the model extracts every line item with a canonical name, so spending groups across shops and brands
- Entries are chunked and embedded into pgvector for semantic search alongside pg_trgm full-text
- Deployed over Tailscale with Docker Compose; per-user AI credentials AES-encrypted at rest
- [Source](https://github.com/mtchowdhury/personal_ai_assistant)

### CloudApper
- No-Code Platform for Enterprise Web / Mobile app

- Developed several major front end modules using Angular 8, devexpress, akita, AWS S3 etc. , that provides complex UI/UX supporting DnD for custom UI building from scratch without coding.
- Maintained and developed backend modules like custom dynamic report generation, API for web app, API for mobile App, with .Net Core, PostgreSQL, Apache Solr
- [More Info](https://www.cloudapper.ai)

### ASAI Micro-Finance Banking System(AMBS)
- Main 360° Solution for ASA International that runs over 14 Countries worldwide

- Migrated major modules like accounts, finance, operations from mono web-form to micro-service architecture solution from scratch
- Maintained and enhanced legacy web-form, web-service tools that was partially operational globally
- Wrote complex stored procedures for different on demand report along with standard accounting reports
- Developed long running backend services for live reporting and data migration and consolidation from prod to report server
- Tech Stacks: .Net Core, Angular, React, Web form, MS SQL, Mongo, RabbitMQ, Kibana, Elasticsearch etc.

### ASA Bangladesh Micro-Finance Management System(AMMS)
- Main Core Solution for ASA Bangladesh that runs over 3200++ branches across the country

- Developed next generation online system using .Net, AngularJS, MS SQL, Jquery etc. from offline Win Form application. This enabled the organisation to avoid consolidating daily scattered branch data, remove the necessity of manually collecting confidential operational data and get rid of the hassle of machine centric hardware compatibility for each branch.
- Wrote many complex sql queries and long running services to migrate and archive more than 16 years of 3200++ branches data to develop the reporting server

### NextReady Ltd.
- SaaS based career consultancy system that provides various services including resume building on custom templates, resume/ portfolio scanner and improvement, job feed generation based on real time data scrapping and user defined criterias.

- Tech Stacks: .Net Core, Angular, python, MSSQL etc
- [More Info](http://nextready.org/home)

### RightPatient System
- Patient identity and authentication platform used in US healthcare: biometric authentication, patient health records and appointment management

- Tech Stacks: .Net, ElectronJS, MSSQL, jQuery etc.
- [More Info](https://www.rightpatient.com/)
