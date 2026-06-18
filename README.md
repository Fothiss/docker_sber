# Docker Compose: Nginx + PostgreSQL

## Структура проекта

├── docker-compose.yml
├── .env
├── web_nginx/
│ ├── Dockerfile
│ ├── index.html
│ └── conf.d/
│ └── default.conf
└── pgdata/

## Быстрый старт

1. Клонируйте или скачайте проект

2. Запустите контейнеры:
```bash
docker-compose up -d
```

3. Проверьте работу:
Веб-сервер: 
```bash
http://localhost:8080
```

БД:
```bash
docker-compose exec db psql -U appuser -d appdb
```