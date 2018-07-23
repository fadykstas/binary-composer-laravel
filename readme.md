## Academy 2018 • .CI/CD/Docker

https://github.com/fadykstas/binary-composer-laravel

### Критерии оценивания:

- Наличие docker-compose.yml,

https://github.com/fadykstas/binary-composer-laravel/blob/master/docker-compose.yml

- Наличие Dockerfile,

https://github.com/fadykstas/binary-composer-laravel/blob/master/app.dockerfile
https://github.com/fadykstas/binary-composer-laravel/blob/master/web.dockerfile

- Наличие образа на Docker Hub

cостоит из трех образов сервисов app, web & DB:
https://hub.docker.com/r/fadykstas/binary-composer-laravel_app/
https://hub.docker.com/r/fadykstas/binary-composer-laravel_web/
https://hub.docker.com/r/fadykstas/mysql/

- Работоспособность образа (запуск проекта должен осуществляться только средствами docker cli)

Запускается через - docker-compose up и доступен по адресу http://0.0.0.0:8080/**

- Логичность использования базового образа (например, если у Вас нет серверной части, а только статические файлы можно обойтись только nginx, без всяких node`ов и так далее)

**Дополнительно можно, но не обязательно (и на оценку не влияет):**

Запустить docker-образ Jenkins + Blueocean и попробовать настроить Continuous Deployment

Попробовать использовать docker volumes.

Задеплоить проект на Heroku или любой другой сервис по Вашему усмотрению.

### Полезные ссылки

Презентация лекции: https://docs.google.com/presentation/d/1dg3-kpOmbnZUHK-ZOVp_l9dCAYNvCotesXZZNq5-Zng/edit?usp=sharing

**Репозиторий примера из лекции**: https://bitbucket.org/oleksandrkovalov/dockertest/src/master/

https://jenkins.io/doc/book/blueocean/getting-started/

https://developer.atlassian.com/blog/2016/06/common-dockerfile-mistakes/

https://blog.jez.io/2015/07/12/docker-tips-and-cheatsheet/

</div>

</div>

<div class="answer-link-wrapper"><md-input-container class="md-link-container"><label class="ng-binding" for="input_0"></label><input type="text" name="link" ng-model="hometaskInfo.lecture.githubLink" class="input-link ng-pristine ng-untouched ng-valid md-input ng-empty" id="input_0" aria-invalid="false" style=""></md-input-container></div>

<div class="answer-text-field row"><label class="answer-text-title ng-binding"></label><textarea ng-model="hometaskInfo.lecture.textAnswer" class="text-answer ng-pristine ng-untouched ng-valid ng-empty" aria-invalid="false"></textarea></div>

<button ng-click="hometaskInfo.saveHometaskAnswer(hometaskInfo)" ng-disabled="hometaskInfo.lecture.isAnswered || hometaskInfo.lecture.timeIsOver" class="button button-blue big-button ng-binding"></button></div>

<div class="hometask-result ng-scope">

<div class="hometask-description">


<div btf-markdown="hometaskInfo.lecture.hometaskId.text" class="markdown-body task-body">

## CI/CD/Docker

### Шаги выполнения:

Установить Docker CE. Если возникают проблемы в первую очередь проверьте наличие включенной виртуализации в BIOS, а также если вы используете Windows - необходимых компонент системы и т.д. (https://docs.docker.com/docker-for-windows/install/#what-to-know-before-you-install) Если ничего не помогает - установите Docker в UNIX-based виртуалке =)

Зарегистрируйтесь на Docker Hub

Выберите любой Ваш проект, которым Вы готовы поделиться с миром.


Создать образ, который будет содержать Ваш проект. Здесь имеется в виду Dockerfile с необходимыми командами.

Запушить Ваш контейнер на Docker Hub.

Создать Docker-compose файл.

Отослать docker-compose.yml и Dockerfile мне любым способом и дать ссылку на Docker-hub с вашим образом.

Получить 10 =)