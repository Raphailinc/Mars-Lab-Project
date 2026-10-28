# Mars Lab Project

[![CI](https://github.com/Raphailinc/Mars-Lab-Project/actions/workflows/ci.yml/badge.svg)](https://github.com/Raphailinc/Mars-Lab-Project/actions/workflows/ci.yml)

[English](README.md) · [Русский](README.ru.md)

A full-stack portfolio application for submitting reports and browsing previously submitted records.

## What it does

- Submit report text with an uploaded attachment.
- Persist reports in MongoDB through Mongoose.
- Check configured communication windows in the API.
- Exercise Express endpoints with Jest, Supertest and an in-memory MongoDB test server.

## Run locally

```bash
npm ci
cp .env.example .env
# Start MongoDB locally, or set MONGODB_URI to a development database.
npm run build
npm start
```

## Checks

```bash
npm test
npm run lint
```

## Scope and implementation notes

API: `http://localhost:3000/api/`. Tests may download a MongoDB test binary on their first run. The SVG in the Russian documentation is a UI illustration. Configure a deployment-specific authentication and upload policy before public use.

Requires Node.js 22.17+; use the committed npm lockfile with `npm ci`.
