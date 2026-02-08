# devops-diplom-app-nginx

Тестовое приложение для дипломного проекта DevOps.

Приложение представляет собой простой веб-сервис на базе **nginx**, который
отдаёт статическую HTML-страницу.  
Используется для демонстрации сборки Docker-образа и дальнейшего деплоя в Kubernetes.

---

## Состав репозитория

- `Dockerfile` — сборка Docker-образа с nginx
- `nginx.conf` — конфигурация nginx
- `index.html` — тестовая HTML-страница
- `README.md` — описание проекта

---

## Сборка Docker-образа

```bash
docker build -t devops-diplom-app-nginx:local .
```

## Проверка локально:
docker run --rm -p 8080:80 devops-diplom-app-nginx:local

## После запуска приложение доступно по адресу:
http://localhost:8080
