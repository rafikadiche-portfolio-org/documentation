# Rafik Adiche — Technical Profile & Project Documentation

This document is a technical reference companion to [rafikadiche.com](https://rafikadiche.com): a fuller
look at the stack, experience, and project work behind the site, with links out to the deeper,
project-level documentation for anyone evaluating the work more closely.

## About

I'm a full-stack JavaScript developer based in Paris, with 11+ years shipping production web
applications — from React and Next.js interfaces to the Node.js and AWS backends that run them. I've
worked both direct-hire and through consulting/ESN engagements, including client work in the banking
sector.

Three things I value most in how I work:

- **Curiosity** — I'd rather understand a system than pattern-match it. Eleven years in, I still read
  the code, ask why, and learn the business behind every build.
- **Adaptability** — Telecom, banking, retail, cloud — different problems, the same calm. I step into a
  new codebase, stack, or team and find my footing quickly.
- **Ownership** — A client's problem is mine until it ships. I see it through launch and say so plainly
  when something isn't ready yet.

**Previously worked with:** HP / HPE, IRT SystemX, LinkByNet, BNP Paribas, Société Générale, Carrefour,
OVHcloud.

## Technical Stack

**Frontend** — HTML5, CSS3, Tailwind CSS, JavaScript (ES6+), TypeScript; React ecosystem (Next.js,
Redux, Zustand, Formik); mobile (React Native, Ionic, Capacitor).

**Backend** — Node.js (NestJS, Express.js); databases (MongoDB, PostgreSQL, Redis); message brokers
(Apache Kafka, RabbitMQ).

**Platforms** — AWS (Lambda, S3, EC2, CloudFront, IAM, Route 53, ACM).

**CI/CD & DevOps** — GitHub Actions.

**Artificial Intelligence** — LLM APIs (Claude, Gemini, LLaMA); workflow automation (Make, Airtable);
Model Context Protocol (FastMCP, Claude Code CLI, Smithery).

## Featured Projects

Live, running work — not just a tool list. Each project below is a full build: frontend, backend, and
the infrastructure it deploys to. Source repositories are private, same positioning as this site's own
five repos; the links below resolve for anyone with repo access.

### Holiday Atlas

An interactive world map showing public holidays by country, in English or French, backed by a live MCP
server any AI client can call directly.

- **Live demo:** [holiday-atlas.rafikadiche.com](https://holiday-atlas.rafikadiche.com)
- **Stack:** Next.js, React, TypeScript, Tailwind CSS, Node.js, AWS Lambda, Terraform, Docker, FastMCP
- **Project documentation:**
  - [Frontend README](https://github.com/holiday-atlas-org/frontend/blob/main/README.md)
  - [Backend README](https://github.com/holiday-atlas-org/backend/blob/main/README.md)
  - [Infrastructure README](https://github.com/holiday-atlas-org/infrastructure/blob/main/README.md)

### NexusBench

A dashboard for comparing pricing, context window, and modalities across the top LLM providers, built on
the same frontend/backend/infrastructure pattern as Holiday Atlas, with its own MCP-plus-REST backend.

- **Status:** In development — not yet deployed or published to GitHub.
- **Stack:** Next.js, TypeScript, Node.js, AWS Lambda, Terraform, FastMCP
- **Project documentation:** architecture, API reference, MCP usage, and deployment notes are written
  and will be linked here once the repositories are published.

## Contact

- **LinkedIn:** [linkedin.com/in/rafik-adiche-7aa28635](https://www.linkedin.com/in/rafik-adiche-7aa28635)
- **GitHub:** [github.com/rafikadiche](https://github.com/rafikadiche)
- **Location:** Paris, France — open to freelance and remote engagements
