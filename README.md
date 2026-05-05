# Илья Вилков — Python Developer

[![Python](https://img.shields.io/badge/Python-3.12+-blue.svg)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.115-009688.svg)](https://fastapi.tiangolo.com)
[![Django](https://img.shields.io/badge/Django-6.x-green.svg)](https://djangoproject.com)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16+-blue.svg)](https://postgresql.org)
[![Docker](https://img.shields.io/badge/Docker-✓-2496ED.svg)](https://docker.com)
[![RabbitMQ](https://img.shields.io/badge/RabbitMQ-✓-FF6600.svg)](https://rabbitmq.com)
[![Celery](https://img.shields.io/badge/Celery-5.x-37814A.svg)](https://docs.celeryq.dev)

Backend Python-разработчик с коммерческим опытом в продуктовой команде и собственным SaaS-проектом в продакшене.

## Обо мне

- **Местоположение**: Нижний Новгород (готов к переезду в Москву, СПб, Казань)
- **Email**: enot19vilkov@yandex.ru
- **Telegram**: [@EnotDD](https://t.me/EnotDD)
- **LinkedIn**: [ilia-vilkov](https://www.linkedin.com/in/ilia-vilkov-52806a391/)
- **Статус**: в поиске работы — Python Backend Developer

## Технологический стек

| Категория | Технологии |
|---|---|
| **Языки** | Python 3.12+ |
| **Фреймворки** | FastAPI, Django, Django REST Framework |
| **БД и ORM** | PostgreSQL, SQLAlchemy, Alembic, django ORM |
| **Очереди / события** | RabbitMQ (aio-pika), Celery, Flower |
| **Кэш** | Redis |
| **Аутентификация** | JWT, Djoser |
| **DevOps** | Docker, Docker Compose, Nginx, GitHub Actions (CI/CD) |
| **Тестирование** | pytest, pytest-django, pytest-asyncio, unittest |
| **Инструменты** | Git, Linux, Pydantic v2, Sentry, Loguru |

## Проекты

### Equilic — SaaS-платформа для управления продуктивностью

Fullstack SaaS-приложение с модулями дневника, задач, финансов и календаря. Разработал архитектуру с нуля и довёл до production-ready состояния.

**Стек:** Django 6, DRF, PostgreSQL, Celery, Redis, Docker, pytest, Sentry

**Ключевые решения:**
- 26 Django-моделей с GIN-индексами (PostgreSQL full-text search) и DB-level constraints
- 40+ REST-эндпоинтов с OpenAPI-документацией (drf-spectacular / Swagger UI)
- Асинхронные задачи на Celery + Redis: отчёты, напоминания с quiet hours, управление trial-подписками
- Signal-driven инвалидация кэша: изменения мгновенно сбрасывают Redis-кэш конкретного пользователя
- Биллинг: trial → active → past_due → cancelled с webhook-обработчиком и feature flags
- 75 тестов (pytest-django), CI с проверкой миграций, Sentry в production

**Ссылки:** [Демо](http://77.91.84.94/) | Проект проходит юридическую регистрацию, готовится к релизу

---

### BookingSeats — Система бронирования мест в кафе (командный проект)

Event-driven REST API для управления бронированием столов в кафе.

**Стек:** FastAPI, PostgreSQL, SQLAlchemy, Alembic, RabbitMQ, Celery, Flower, Docker, JWT, Pydantic v2

**Ключевые решения:**
- Event-driven архитектура: Outbox Pattern → RabbitMQ → Celery
- REST API: кафе, столы, временные слоты, блюда, акции, бронирования, медиа
- Outbox Pattern — надёжная доставка событий без потерь при сбоях брокера
- Email-нотификации через Celery + мониторинг задач через Flower (basic auth)
- Сквозная трассировка запросов через correlation_id (X-Request-ID) от API до Celery

**Ссылки:** [GitHub](https://github.com/Iliya-Vilkov/BOOKING_SEATS) | [Документация API](https://booking-seat.ru/docs)

---

### Foodgram — Социальная сеть для рецептов

Полноценный backend с REST API, системой аутентификации, подписками, избранным, списком покупок и фильтрацией по тегам.

**Стек:** Python, Django, DRF, PostgreSQL, Docker, Nginx, GitHub Actions

**Ссылки:** [GitHub](https://github.com/Iliya-Vilkov/foodgram) | [Продакшен](http://foodgrambest.sytes.net)

---

### MovieHub — Платформа для обмена фильмами

Сложные модели: фильмы, жанры, актёры, рейтинги, комментарии. Избранное, подписки, watchlist, поиск по жанрам и актёрам.

**Стек:** Python, Django, DRF, PostgreSQL, Docker

**Ссылки:** [GitHub](https://github.com/Iliya-Vilkov/MovieHub)

---

## Опыт работы

**Python Developer** | [PRODUCTLAB](https://tablecrm.com) | Июнь 2025 — Ноябрь 2025
- REST API на FastAPI, интеграция с Т-Банком и онлайн-кассой
- Загрузка изображений через AWS S3
- Рефакторинг: устранил 1000+ ошибок линтера, снизил технический долг
- Команда 16–18 человек, Scrum, code review, pytest

**Python-разработчик** | Проектная работа | Февраль 2023 — Май 2025
- Foodgram, MovieHub, BookingSeats, Telegram-боты

## Образование

- **2026** — Яндекс Практикум, Python-разработчик (расширенный уровень)
- **2019** — НГИЭУ, Бакалавр, Инфокоммуникационные технологии
- **2018** — Академия Айти, Python-разработчик

## GitHub статистика

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Iliya-Vilkov&show_icons=true&theme=radical)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Iliya-Vilkov&layout=compact&theme=radical)

---

**Последнее обновление**: Май 2026
