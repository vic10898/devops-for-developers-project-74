# JS Fastify Blog

[![Actions Status](https://github.com/vic10898/devops-for-developers-project-74/actions/workflows/push.yml/badge.svg)](https://github.com/vic10898/devops-for-developers-project-74/actions)

## Требования к системе

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)
- Make

## Установка

Подготовьте файл переменных окружения:

```bash
cp app/.env.example app/.env
```

Установите зависимости и выполните миграции базы данных:

```bash
make setup
```

## Запуск в режиме разработки

```bash
make dev
```

Приложение доступно по адресам:
- http://localhost — перенаправляет на HTTPS
- https://localhost — основной адрес

## Тесты

```bash
make test
```

## CI (запуск тестов внутри Docker)

```bash
make ci
```

## Сборка и публикация production-образа

```bash
make build
make push
```

## Docker Hub

Образ приложения: [winnypoox/devops-for-developers-project-74](https://hub.docker.com/r/winnypoox/devops-for-developers-project-74)
