# lab2-app

Навчальний репозиторій до лабораторної роботи №2 «Основи DevOps»
(конвеєр CI/CD у GitHub Actions).

| Workflow | Призначення |
| --- | --- |
| `production-pipeline.yml` | test → build (ghcr.io) → deploy-staging → deploy-production |
| `matrix.yml` | матрична збірка: 3 ОС × 3 версії Node.js − 1 виключення = 8 завдань |
| `deploy-template.yml` | reusable workflow (`workflow_call`) |
| `call-deploy.yml` | виклик reusable workflow вручну (`workflow_dispatch`) |
| `conditional.yml` | умовні завдання за зміненими каталогами `backend/`, `frontend/` |
