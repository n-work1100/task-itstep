# WordPress Docker Project

## Опис проєкту

Проєкт призначений для розгортання WordPress за допомогою Docker Compose.

Проєкт складається з трьох сервісів:

- **WordPress** — система керування вмістом вебсайту.
- **MySQL 8.0** — база даних для WordPress.
- **phpMyAdmin** — вебінтерфейс для керування базою даних.

## Використані технології

- Docker
- Docker Compose
- WordPress
- MySQL 8.0
- phpMyAdmin

## Порти доступу

| Сервіс | Порт |
|---|---|
| WordPress | 8080 |
| phpMyAdmin | 8081 |

## Запуск проєкту

1. Встановити Docker та Docker Compose.
2. Створити файл `.env` із власними параметрами підключення до бази даних.
3. Запустити проєкт:

```bash
docker compose up -d
```

4. Перевірити стан контейнерів:

```bash
docker compose ps
```

## Доступ до сервісів

- WordPress: http://localhost:8080
- phpMyAdmin: http://localhost:8081

## Зупинка проєкту

Для зупинки контейнерів виконайте команду:

```bash
docker compose down
```

Для видалення контейнерів разом із даними:

```bash
docker compose down -v
```

## Безпека

**Важливо:** файл `.env` містить конфіденційні дані (паролі) та виключений із Git за допомогою `.gitignore`.
