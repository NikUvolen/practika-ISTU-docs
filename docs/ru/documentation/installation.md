# JOB ISTU — Backend

Бэкенд сервиса **JOB ISTU**, реализованный на **Django** и запускаемый в Docker-контейнерах.

---

## Требования

Перед запуском убедитесь, что у вас установлены:

- **Docker** (версия 20+)
- **Docker Compose** (v2+)

Проверка:

```bash
  docker --version
  docker compose version
```

---

## Настройка переменных окружения

Для запуска понадобится скачать с чата тг или создать `.env` файл путем копирования из `.env_example`

## Загрузка SQL-дампа

1.	Поместите файл дампа в папку db_dumps/
2.	Выполните команду:
```bash
  make upload-text-dump name=<your_dump>.sql 
```

## Сборка и запуск проекта

1. Сборка Docker-образов:
```bash
  make build 
```
2. Запуск всех сервисов:
```bash
  make up 
```

Будут запущены:
- Django backend 
- PostgreSQL
- pgAdmin

---

## Доступные сервисы

После успешного запуска:

- Backend API
```url
http://localhost:8000 
```
- Просмотр эндпойнотов через Swagger / OpenAPI (DEBUG=true)
```url
http://localhost:8000/api/doc/
```
- pgAdmin
```url
http://localhost:15080
```

{% note info %}

Логин и пароль — из `.env`

{% endnote %}
