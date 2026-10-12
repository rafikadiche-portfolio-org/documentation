# Technical stack

[Documentation index](../README.md)

This page lists the languages, frameworks and tools in use, by layer, and names the project that shows each one.

## At a glance

| Topic | Summary |
|---|---|
| Languages | TypeScript in strict mode, JavaScript, HCL for Terraform, Python for agent workflows |
| Frontend | React, Next.js with static export, Tailwind CSS |
| Backend | Node.js on AWS Lambda, NestJS, REST with OpenAPI, Model Context Protocol |
| Data | Amazon DynamoDB, Amazon S3, static JSON datasets |
| Cloud and delivery | AWS serverless services, Terraform, Docker, GitHub Actions |
| AI | MCP servers, CrewAI, Claude models, Claude Code |

The first five tables hold what runs in the three portfolio projects, so each row can be checked. The last table holds tools used in client roles, where the code is not public.

## Frontend

| Tool | Used for | Shown in |
|---|---|---|
| TypeScript, strict mode | All frontend code | [Holiday Atlas](../02-projects/holiday-atlas.md), [NexusBench](../02-projects/nexusbench.md), [rafikadiche.com](../02-projects/portfolio-site.md) |
| React and Next.js (App Router, static export) | Sites built as static files, with no web server in production | All three projects |
| Tailwind CSS with design tokens | Styling, light and dark themes | [Holiday Atlas UX design](https://github.com/holiday-atlas-org/documentation/blob/main/01-functional/ux-design.md), [NexusBench](../02-projects/nexusbench.md) |
| D3 and HTML canvas | An interactive globe drawn on a canvas | [Holiday Atlas frontend](https://github.com/holiday-atlas-org/documentation/blob/main/02-technical/frontend.md) |
| Recharts | Dashboard charts | [NexusBench](../02-projects/nexusbench.md) |
| Formik and Yup | Contact form state and validation | [rafikadiche.com](../02-projects/portfolio-site.md) |
| Vitest, React Testing Library, Playwright, axe-core | Unit, component, end-to-end and accessibility tests | [Holiday Atlas testing](https://github.com/holiday-atlas-org/documentation/blob/main/03-quality/testing.md) |

## Backend

| Tool | Used for | Shown in |
|---|---|---|
| Node.js on AWS Lambda | Every API in the portfolio | All three projects |
| NestJS, monorepo mode | Services for the data pipeline, the REST API and the MCP endpoint | [NexusBench](../02-projects/nexusbench.md) |
| REST with OpenAPI 3 | Public, documented APIs | [Holiday Atlas API reference](https://github.com/holiday-atlas-org/documentation/blob/main/02-technical/api-reference.md), [NexusBench Swagger UI](https://nexusbench.rafikadiche.com/api/docs) |
| Model Context Protocol | Tools that AI clients call directly: an SDK server over Streamable HTTP, and a small JSON-RPC handler written for a short-lived function | [NexusBench](../02-projects/nexusbench.md), [Holiday Atlas architecture](https://github.com/holiday-atlas-org/documentation/blob/main/02-technical/architecture.md) |
| zod | Schema validation at service boundaries | [Holiday Atlas backend](https://github.com/holiday-atlas-org/documentation/blob/main/02-technical/backend.md), [NexusBench](../02-projects/nexusbench.md) |
| Jest, Supertest, DynamoDB Local | Unit and end-to-end tests of the services | [NexusBench](../02-projects/nexusbench.md) |
| Node.js test runner | Unit tests of the contact API | [rafikadiche.com](../02-projects/portfolio-site.md) |

## Data

| Tool | Used for | Shown in |
|---|---|---|
| Amazon DynamoDB, single-table design | The catalog written by the data pipeline | [NexusBench](../02-projects/nexusbench.md) |
| Amazon S3 | Precomputed JSON read models and a raw data archive | [NexusBench](../02-projects/nexusbench.md) |
| Static JSON dataset | Holiday rules shipped inside the function, with no database | [Holiday Atlas backend](https://github.com/holiday-atlas-org/documentation/blob/main/02-technical/backend.md) |

## Cloud and delivery

| Tool | Used for | Shown in |
|---|---|---|
| AWS Lambda | Functions from container images and from bundled code | All three projects |
| Amazon API Gateway | HTTP APIs in front of the functions | [NexusBench](../02-projects/nexusbench.md), [rafikadiche.com](../02-projects/portfolio-site.md) |
| Amazon S3 and CloudFront | Static hosting behind a CDN, with a private origin | All three projects |
| AWS Step Functions, Amazon EventBridge, Amazon SQS | A scheduled, event-driven data pipeline | [NexusBench](../02-projects/nexusbench.md) |
| Amazon Route 53 and AWS Certificate Manager | DNS and TLS certificates | All three projects |
| Amazon SES | Outgoing email from the contact form | [rafikadiche.com](../02-projects/portfolio-site.md) |
| AWS IAM, AWS Secrets Manager | Scoped roles, secrets with rotation | [NexusBench](../02-projects/nexusbench.md), [Holiday Atlas security](https://github.com/holiday-atlas-org/documentation/blob/main/03-quality/security.md) |
| Amazon CloudWatch, Amazon SNS, AWS Budgets | Logs, alarms and cost alerts | [Holiday Atlas infrastructure](https://github.com/holiday-atlas-org/documentation/blob/main/02-technical/infrastructure.md), [NexusBench](../02-projects/nexusbench.md) |
| Terraform | All AWS resources, with remote state | All three projects |
| Docker and Amazon ECR | Function images, and a container for the Terraform and AWS tooling | [Holiday Atlas infrastructure](https://github.com/holiday-atlas-org/documentation/blob/main/02-technical/infrastructure.md), [rafikadiche.com](../02-projects/portfolio-site.md) |
| GitHub Actions | Checks on pull requests and automated deploys. NexusBench and the contact API of the site reach AWS through OIDC, with no stored cloud key | [Holiday Atlas operations](https://github.com/holiday-atlas-org/documentation/blob/main/03-quality/operations.md), [NexusBench](../02-projects/nexusbench.md), [rafikadiche.com](../02-projects/portfolio-site.md) |

## AI

| Tool | Used for | Shown in |
|---|---|---|
| MCP servers | Read-only tools over an existing API | [Holiday Atlas API reference](https://github.com/holiday-atlas-org/documentation/blob/main/02-technical/api-reference.md), [NexusBench](../02-projects/nexusbench.md) |
| CrewAI with Claude models | A multi-agent workflow that produced a dashboard specification, with human review points and a cost cap per run | [NexusBench](../02-projects/nexusbench.md) |
| Claude Code | Agent-assisted delivery of code and documentation, under review | [Engineering practices](engineering-practices.md) |

## Used in client work

These tools were used in client roles. The code belongs to the clients, so there is no project page to link. The client history is on [LinkedIn](https://www.linkedin.com/in/rafik-adiche-7aa28635).

| Layer | Tools |
|---|---|
| Frontend | Angular, Vue.js, HTML5, CSS3 |
| Backend | Express, GraphQL |
| Data | PostgreSQL, MongoDB, Redis |

## Status and gaps

- The NexusBench documentation repository is not public yet. Rows that name NexusBench link to its summary page here, to the live app and to its public API reference.
- No proficiency ratings are given. A tool is listed because it runs in a project or was used in a client role.
