# Clarify

![Next.js](https://img.shields.io/badge/Next.js%2016-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React%2019-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind%20v4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![Vercel AI SDK](https://img.shields.io/badge/Vercel%20AI%20SDK-000000?style=flat-square&logo=vercel&logoColor=white)

AI Business Analyst agent. Drop in a project brief, get back a full BA artifact pack: requirements with unique IDs, a Requirements Traceability Matrix, test cases, and a RACI stakeholder register.

The agent refuses to invent details. If the brief is ambiguous on scope, users, success metrics, integrations, or constraints, it asks clarifying questions before generating anything.

## Stack

- Next.js 16 (App Router) + React 19
- TypeScript, Tailwind v4, shadcn/ui
- Vercel AI SDK with OpenRouter (free model, swap via `CLARIFY_MODEL` env)

## Local development

```bash
cp .env.example .env.local
# fill in OPENROUTER_API_KEY
npm install
npm run dev
```

Open `http://localhost:3000`.

## Deploy

Deploys to Vercel as a standard Next.js app. Set `OPENROUTER_API_KEY` in the Vercel project env vars. Optionally override the default model with `CLARIFY_MODEL`.

## Status

Early MVP. Brief in, clarifying questions or first artifact pack out. Structured artifact rendering, export, and durable multi-step workflow are next.

---

<sub>Built by **Mansi** · [github.com/Mansi2221](https://github.com/Mansi2221)</sub>
