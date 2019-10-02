# Tracker

technologicals
- github
- mysql
- python
- django
- rest api
- json
- vuejs
- webpack
- yarn

study to integrate:
- Logger
- jenkins
- openshift
- ansible
- dockers/kubernets
- swagger for rest api documentation

Prerequisites
- python3.4 
- pip3.4
- venv (virtualenv)
- yarn


Running Development Servers
- mkdir django-vue
- cd django-vue
- virtualenv .
- source bin/activate
- pip3.4 install django
- django-admin startproject djangovue .
- python manage.py startapp catalog
- add this app to the list on settings.py
	- INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'catalog',
]

- python manage.py migrate
- python manage.py runserver 0:8000
- run as service
   - nohup python3 manage.py runserver 0:80 &

- sudo npm install -g vue-cli
- vue init webpack frontend
	Questions/answers:
	Project name: frontend
	Project description: A Vue.js project
	Author: Your Name your.name@somewhere.com
	Vue build: Runtime + Compiler: recommended for most users
	Install vue-router? Yes
	Use ESLint to lint your code? Yes
	Pick an ESLint preset: Standard
	Set up unit tests: No
	Setup e2e tests with Nightwatch? No
	Should we run npm install for you after the project has been created? (recommended) Yes, use NPM
- npm run dev -- --host '0'  --port 8080

Links de projectos:
- https://medium.com/quick-code/crud-app-using-vue-js-and-django-516edf4e4217
- https://github.com/gtalarico/django-vue-template
- https://medium.com/@rodrigosmaniotto/integrating-django-and-vuejs-with-vue-cli-3-and-webpack-loader-145c3b98501a
- https://auth0.com/blog/building-modern-applications-with-django-and-vuejs/#introduction-vue-js
