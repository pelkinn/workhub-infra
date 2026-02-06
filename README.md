WorkHub инфраструктура для продакшн‑развёртывания: Docker Compose со связкой PostgreSQL, Redis и backend‑сервиса.
Переменные окружения вынесены в `/opt/workhub/env/.env`.

## Зависимости

Требуется запущенный `server-infra` (создаёт сеть `proxy`).

## Запуск

```bash
# Сначала server-infra
cd /opt/server-infra && docker compose up -d

# Затем workhub
cd /opt/workhub/infra && docker compose -f docker-compose.prod.yml up -d
```
