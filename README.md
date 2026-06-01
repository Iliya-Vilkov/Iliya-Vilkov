# Ilia Vilkov — Python Developer

[![Python](https://img.shields.io/badge/Python-3.12+-blue.svg)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.115-009688.svg)](https://fastapi.tiangolo.com)
[![Django](https://img.shields.io/badge/Django-6.x-green.svg)](https://djangoproject.com)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16+-blue.svg)](https://postgresql.org)
[![Docker](https://img.shields.io/badge/Docker-✓-2496ED.svg)](https://docker.com)
[![RabbitMQ](https://img.shields.io/badge/RabbitMQ-✓-FF6600.svg)](https://rabbitmq.com)
[![Celery](https://img.shields.io/badge/Celery-5.x-37814A.svg)](https://docs.celeryq.dev)

Python Backend Developer with commercial experience in a product team and a production SaaS project.

## About

- **Location**: Nizhny Novgorod, Russia (open to relocation: Moscow, Saint Petersburg)
- **Email**: iliyavilkov@gmail.com
- **Telegram**: [@EnotDD](https://t.me/EnotDD)
- **LinkedIn**: [ilia-vilkov](https://www.linkedin.com/in/ilia-vilkov-52806a391/)
- **Status**: Open to work — Python Backend Developer

## Tech Stack

| Category | Technologies |
|---|---|
| **Languages** | Python 3.12+ |
| **Frameworks** | FastAPI, Django, Django REST Framework |
| **DB & ORM** | PostgreSQL, SQLAlchemy, Alembic, Django ORM |
| **Queues / Events** | RabbitMQ (aio-pika), Celery, Flower |
| **Cache** | Redis |
| **Auth** | JWT, Djoser |
| **DevOps** | Docker, Docker Compose, Nginx, GitHub Actions (CI/CD) |
| **Testing** | pytest, pytest-django, pytest-asyncio, unittest |
| **Tools** | Git, Linux, Pydantic v2, Sentry, Loguru |

## Projects

### Equilic — SaaS Productivity Platform

Fullstack SaaS application with diary, tasks, finance and calendar modules. Designed architecture from scratch and brought to production-ready state.

**Stack:** Django 6, DRF, PostgreSQL, Celery, Redis, Docker, pytest, Sentry

**Key decisions:**
- 26 Django models with GIN indexes (PostgreSQL full-text search) and DB-level constraints
- 40+ REST endpoints with OpenAPI docs (drf-spectacular / Swagger UI)
- Async tasks on Celery + Redis: reports, reminders with quiet hours, trial subscription management
- Signal-driven cache invalidation: changes instantly flush Redis cache for the specific user
- Billing: trial → active → past_due → cancelled with webhook handler and feature flags
- 75 tests (pytest-django), CI with migration checks, Sentry in production

**Links:** [Demo](http://77.91.84.94/) | Project is undergoing legal registration, preparing for release

---

### BookingSeats — Cafe Seat Booking System (team project)

Event-driven REST API for managing table reservations in cafes.

**Stack:** FastAPI, PostgreSQL, SQLAlchemy, Alembic, RabbitMQ, Celery, Flower, Docker, JWT, Pydantic v2

**Key decisions:**
- Event-driven architecture: Outbox Pattern → RabbitMQ → Celery
- REST API: cafes, tables, time slots, dishes, promotions, bookings, media
- Outbox Pattern — reliable event delivery without loss on broker failure
- Email notifications via Celery + task monitoring via Flower (basic auth)
- End-to-end request tracing via correlation_id (X-Request-ID) from API to Celery

**Links:** [GitHub](https://github.com/Iliya-Vilkov/BOOKING_SEATS) | [API Docs](https://booking-seat.ru/docs)

---

### Foodgram — Recipe Social Network

Full-featured backend with REST API, authentication, subscriptions, favourites, shopping list and tag filtering.

**Stack:** Python, Django, DRF, PostgreSQL, Docker, Nginx, GitHub Actions

**Links:** [GitHub](https://github.com/Iliya-Vilkov/foodgram) | [Production](http://foodgrambest.sytes.net)

---

### MovieHub — Movie Exchange Platform

Complex models: movies, genres, actors, ratings, comments. Favourites, subscriptions, watchlist, search by genres and actors.

**Stack:** Python, Django, DRF, PostgreSQL, Docker

**Links:** [GitHub](https://github.com/Iliya-Vilkov/MovieHub)

---

## Work Experience

**Python Developer** | Equilic | November 2025 — Present
- Designed SaaS platform from scratch: 26 Django models, 40+ REST endpoints, billing system
- Celery + Redis: async tasks, signal-driven cache invalidation
- 75 tests (pytest-django), CI with migration checks, Sentry in production
- Docker Compose for local and production environments

**Python Developer** | [PRODUCTLAB](https://tablecrm.com) | June 2025 — November 2025
- REST API on FastAPI, payment integration with online cash register
- Image uploads via AWS S3
- Refactoring: fixed 1000+ linter errors, reduced technical debt
- Team of 16–18 engineers, Scrum, code review, pytest

**Python Developer** | Personal Projects | February 2023 — May 2025
- Foodgram, MovieHub, BookingSeats (team project)

## Education

- **2026** — Yandex Practicum, Python Developer (advanced level)
- **2019** — NSUEE, Bachelor's degree, Information Technologies and Communication Systems
- **2018** — IT Academy, Python Developer

## Repositories

| Project | Stack | Links |
|---|---|---|
| **Equilic** | Django, DRF, Celery, Redis, PostgreSQL | [Demo](http://77.91.84.94/) |
| **BookingSeats** | FastAPI, RabbitMQ, Celery, SQLAlchemy | [GitHub](https://github.com/Iliya-Vilkov/BOOKING_SEATS) · [Docs](https://booking-seat.ru/docs) |
| **Foodgram** | Django, DRF, Docker, Nginx, CI/CD | [GitHub](https://github.com/Iliya-Vilkov/foodgram) · [Demo](http://foodgrambest.sytes.net) |
| **MovieHub** | Django, DRF, PostgreSQL, Docker | [GitHub](https://github.com/Iliya-Vilkov/MovieHub) |

---

**Last updated**: June 2026
