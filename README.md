# Docker Compose: Nginx + PostgreSQL

## Структура проекта

```bash
├── docker-compose.yml
├── .env
├── web_nginx/
│ ├── Dockerfile
│ ├── index.html
│ └── conf.d/
│ └── default.conf
└── pgdata/
```

## Быстрый старт

1. Клонируйте или скачайте проект

2. Запустите контейнеры:
```bash
docker-compose up -d
```

3. Проверьте работу веб-сервера: 
```bash
http://localhost:8080
```

4. Проверьте работу БД: 
```bash
docker-compose exec db psql -U appuser -d appdb
```

5. Остановите контейнеры
```bash
docker-compose down
```