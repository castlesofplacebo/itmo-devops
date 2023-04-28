## Docker: Запуск nginx

Цель лабораторной: запустить в докере рабочий веб-сервер nginx

1. Образ должен быть легковесным (на базе scratch)
2. Должна быть возможность конфигурирования через файл
3. Статика должна быть внешним томом volume
4. Создать файл docker-compose для старта и сборки
5. В docker-compose должен быть сайдкар для lets encrypt

### ToDo:
- Run as Non-root User

### Comments:
- Dockerfile для stable-версии nginx

### Links:
- http://nginx.org/en/linux_packages.html#Alpine
- https://zawadidone.nl/using-docker-images-from-scratch/
- https://github.com/gunjank/docker-nginx-scratch/blob/master/Dockerfile
- https://github.com/nginxinc/docker-nginx/blob/5ce65c3efd395ee2d82d32670f233140e92dba99/Dockerfile-alpine-slim.template
- https://hub.docker.com/_/nginx
- https://github.com/nginx/nginx/blob/master/conf/nginx.conf
- https://www.programonaut.com/setup-ssl-with-docker-nginx-and-lets-encrypt/#automate-ssl-certificates-with-certbot
- https://mindsers.blog/post/https-using-nginx-certbot-docker/
