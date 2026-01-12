# API Справочник

## Версия: 1.0.0

{% note info %}

Актуальные API можно посмотреть через Swagger / OpenAPI (DEBUG=true)

{% endnote %}

---
### 1. Аутентификация
---
`POST /api/out/base/auth/`
  - Авторизация пользователя (username, password)
  - Ответ: токен доступа

`POST /api/out/base/auth/log_out`
  - Выход пользователя

`POST /api/out/base/auth/refresh`
  - Обновление access-токена по refresh-токену

---
### 2. Контакты
---
`POST /api/out/base/contacts/add`
  - Добавить контакт

---
### 3. Практики
---
`GET /api/out/base/practice/`
  - Получить список практик (фильтр по faculty)

`GET /api/out/base/practice/{id}`
  - Получить практику по id

---
### 4. Специальности
---
`GET /api/out/base/speciality/`
  - Получить список специальностей

`GET /api/out/base/speciality/{id}`
  - Получить специальность по id

`POST /api/out/base/speciality/add`
  - Добавить специальность

---
### 5. Темы
---
`GET /api/out/base/theme/`
  - Получить список тем

`GET /api/out/base/theme/{id}`
  - Получить тему по id

---
### 6. Пользователи
---
`POST /api/out/base/user/add`
  - Добавить пользователя

`GET/PATCH /api/out/base/user/company`
  - Получить/обновить компанию пользователя

`GET/POST /api/out/base/user/company/meta`
  - Получить/добавить мета-данные компании

`PATCH/DELETE /api/out/base/user/company/meta/{id}`
  - Обновить/удалить мета-данные компании

`GET/POST /api/out/base/user/contact`
  - Получить/добавить контакт пользователя

`PATCH/DELETE /api/out/base/user/contact/{id}`
  - Обновить/удалить контакт пользователя

`GET/PATCH /api/out/base/user/info`
  - Получить/обновить информацию пользователя

`GET/POST /api/out/base/user/practice`
  - Получить/добавить практику пользователя

`GET/PATCH/DELETE /api/out/base/user/practice/{id}`
  - Получить/обновить/удалить практику пользователя

`POST/DELETE /api/out/base/user/practice/{id}/contact/{contact}`
  - Добавить/удалить контакт к практике пользователя

`POST/DELETE /api/out/base/user/practice/{id}/themes/{theme}`
  - Добавить/удалить тему к практике пользователя

`GET/POST /api/out/base/user/themes`
  - Получить/добавить тему пользователя

`PATCH/DELETE /api/out/base/user/themes/{id}`
  - Обновить/удалить тему пользователя

---
### 7. Компании (legacy)
---
`GET /api/out/legacy/company/`
  - Получить список компаний

`GET /api/out/legacy/company/{id}`
  - Получить компанию по id

`POST /api/out/legacy/company/add`
  - Добавить компанию

---
### 8. Факультеты (legacy)
---
`GET /api/out/legacy/faculty/`
  - Получить список факультетов

`GET /api/out/legacy/faculty/{id}`
  - Получить факультет по id

`POST /api/out/legacy/faculty/add`
  - Добавить факультет


