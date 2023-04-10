## Docker: докеризация приложения

Цель лабораторной: собрать из исходного когда и запустить в докере рабочее приложение (любое опенсорс - java, python/django/flask).

1. Образ должен быть легковесным
2. Вся конфигурация выполняется через переменные окружения
3. Статика (зависимости) должна быть внешним томом `volume`
4. Создать файл `docker-compose` для старта и сборки
5. В `docker-compose` должна быть база данных
6. При старте приложения должно быть учтено выполнение миграций
7. При старте приложения должно быть учтено создание супер-пользователя (если возможно)

### Links:
- https://docs.docker.com/language/java/