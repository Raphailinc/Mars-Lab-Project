# Mars Lab Project

[![CI](https://github.com/Raphailinc/Mars-Lab-Project/actions/workflows/ci.yml/badge.svg)](https://github.com/Raphailinc/Mars-Lab-Project/actions/workflows/ci.yml)

[English](README.md) · [Русский](README.ru.md)

Fullstack-проект для отправки отчётов и просмотра сохранённых записей.

## Возможности

- Отправка текста отчёта с вложением.
- Сохранение в MongoDB через Mongoose.
- Проверка настроенных временных окон связи в API.
- Тесты Express через Jest, Supertest и тестовый MongoDB.

## Локальный запуск

```bash
npm ci
cp .env.example .env
# Start MongoDB locally, or set MONGODB_URI to a development database.
npm run build
npm start
```

## Проверки

```bash
npm test
npm run lint
```

## Условия запуска и границы проекта

Требуется Node.js 22.17+. API: http://localhost:3000/api/. Запустите MongoDB или задайте MONGODB_URI для локальной БД. Первый запуск тестов может скачать тестовый бинарный файл MongoDB. SVG в docs — иллюстрация интерфейса. Перед публичным развёртыванием требуется отдельная политика аутентификации и загрузок.
