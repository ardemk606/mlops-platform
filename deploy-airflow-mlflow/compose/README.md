# Развертывание Airflow и MLflow

## Предварительные требования
- Docker и Docker Compose
- Linux/macOS (для команды id)

## Запуск

1. Создайте файл .env с ID пользователя и группы:
echo -e "AIRFLOW_UID=$(id -u)\nAIRFLOW_GID=0" > .env

2. Запустите миграцию
docker compose up airflow-init

3. Запустите сервисы
docker compose up
