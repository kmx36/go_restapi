# URL Shortener REST API

Этот проект представляет собой полноценный REST API сервис для сокращения URL-адресов. Реализован с учетом лучших практик, покрыт тестами и настроен автоматический деплой через GitHub Actions.

## Функциональность
- Обработка HTTP-запросов с помощью актуального роутера
- Логирование событий
- Поддержка авторизации
- Тестирование (unit-тесты, тесты хэндлеров, функциональные тесты)
- Хранение данных в SQLite
- Автоматический деплой на виртуальный сервер через GitHub Actions

## Используемые технологии
Проект написан на языке Go и использует следующие библиотеки:
- `go-chi/chi` — HTTP-роутер
- `slog` — логирование
- `stretchr/testify` — тестирование
- `ilyakaznacheev/cleanenv` — конфигурирование
- `SQLite` — база данных

## Установка и запуск
### 1. Клонирование репозитория
```sh
git clone 
```

### 2. Установка зависимостей
```sh
go mod tidy
```

### 3. Запуск сервера
```sh
go run main.go
```

## Тестирование
Запустить тесты можно с помощью команды:
```sh
go test ./tests/...
```

## Деплой
Автоматический деплой настроен с использованием GitHub Actions. После пуша изменений в основную ветку проект будет автоматически развернут на сервере.

