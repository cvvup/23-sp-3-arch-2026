# Архитектурирование

Репозиторий с лабораторными работами по дисциплине "Архитектурирование"

## Выполнила
Хайдукова Мария Игоревна  
Группа: БИВТ-23-СП-3

## Docker Hub
`cvvup/23-sp-3-hm:latest`

## Структура репозитория
- [laba1](https://github.com/cvvup/23-sp-3-arch-2026/tree/main/laba1) - лабораторная работа 1, контейнеризация приложения с помощью Docker и Docker Compose
- [laba2](https://github.com/cvvup/23-sp-3-arch-2026/tree/main/laba2) - лабораторная работа 2, кеширование с использованием KeyDB/Redis и стратегия `cache-aside`
- [laba3](https://github.com/cvvup/23-sp-3-arch-2026/tree/main/laba3) - лабораторные работы 3, 4 и 5 на базе многомодульного приложения `archapp`

## Кратко по лабораторным

### Лабораторная работа 1 - Docker
- Поднято клиент-серверное приложение в контейнерах
- Настроен `docker-compose` для запуска приложения и инфраструктуры
- Подготовлены скриншоты и материалы для защиты

### Лабораторная работа 2 - Кеширование
- Реализовано кеширование пользователей с использованием `KeyDB`
- В приложении применена стратегия `cache-aside`
- Настроено взаимодействие `user-service` с Postgres и KeyDB

### Лабораторная работа 3 - Event-Driven Architecture
- Подключен `RabbitMQ` для асинхронного взаимодействия между сервисами
- Реализована публикация и обработка событий между `user-service` и `notification-service`
- Настроены exchange, queue, bindings и демонстрация роутинга сообщений

### Лабораторная работа 4 - Observability
- Подняты `Prometheus`, `Grafana`, `Alertmanager` и `Mailpit`
- Добавлены кастомные метрики приложения через `Spring Boot Actuator` и `Micrometer`
- Настроены дашборды, алерты и отправка уведомлений по SMTP

### Лабораторная работа 5 - CQRS и Event Sourcing
- Добавлен `balance-service`, реализованный по паттерну `CQRS`
- Для хранения изменений используется `Event Sourcing` на базе `Axon Server`
- Реализованы команды, события, агрегат и read-модели для работы с балансом пользователя

## Основные технологии
- Java 17
- Spring Boot
- Maven
- Docker / Docker Compose
- PostgreSQL
- KeyDB / Redis
- RabbitMQ
- Prometheus
- Grafana
- Alertmanager
- Axon Framework