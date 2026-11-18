# devops-ci-app

Учебное Flask-приложение для практической работы №10.

## Конвейер

Pylint → pytest → Docker build → smoke-test → GHCR.

Публикация образа выполняется при push в `main`.
В Pull Request выполняются проверки и пробный запуск контейнера.

## Адреса приложения

- `/health` — проверка состояния;
- `/` — сведения о службе.

## Образ

`ghcr.io/YOUR_LOGIN/devops-ci-app`

## Workflow

`.github/workflows/ci.yml`