# devops-diplom-app-nginx

Данный репозиторий является вспомогательным проектом для выпускной работы.

Основной проект инфраструктуры находится здесь:  
https://github.com/ysatii/devops-diplom-app-nginx/tree/main

## Назначение

В репозитории размещено простое веб-приложение на базе **Nginx**, используемое для демонстрации:

- сборки Docker-образа
- публикации образа в Yandex Container Registry
- автоматического деплоя в Kubernetes
- работы CI/CD пайплайна

## Технологии

- Docker
- Nginx
- GitLab CI/CD
- Yandex Container Registry
- Kubernetes

## Логика работы CI/CD

Каждый коммит в ветку `main`:

1. Запускает сборку Docker-образа  
2. Публикует образ в Container Registry  
3. Выполняет обновление Deployment в Kubernetes  
4. Производит rolling update подов  

Проект используется для демонстрации CI/CD процессов в рамках выпускной квалификационной работы.
