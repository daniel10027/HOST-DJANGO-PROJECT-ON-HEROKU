# HOST-DJANGO-PROJECT-ON-HEROKU
![images](https://github.com/daniel10027/HOST-DJANGO-PROJECT-ON-HEROKU/blob/master/download%20(1).jpeg)



```console
hello, directory was created to help all those who have difficulty
hosting their django project on heroku.
follow each of the following steps and everything should be fine.
```

### step 0:
```console
install git
install heroku cli
```
### Step 1:
```console
create an empty folder on your desktop and move your project inside
```
### 2nd step:
```console
create a new virtual environment and install django there.
```
### steps 3: 
```console
make a python manage.py runserver,
normally it should fail.
don't worry that's the goal

```
### step 4: 
```console
install each of the required packages and restart your server.

if your application launches normally in the new environment 
stop the server and now we can go to the next step
```

### step 5:
```console
create a file named Procfile without extension and inside this 
file add the following line:
```
```js
web: gunicorn the_name_of_your_project.wsgi
```
### step 6: install some package

- [x] psycopg2==2.7.5
- [x] pip install gunicorn
- [x] pip install django-heroku


### step 7

add ```import django_heroku```  on te top of your settings.py

add ```django_heroku.settings(locals())```  on the bottom of your settings.py

### step 8 
```console
in the same directory of manage.py make :
```
```js
pip freeze > requirements.txt
```
### step 9
```console
I assume that you have created a heroku account and that you have installed heroku cli
in your terminal do :
```
```js
heroku login
```
```console
you have a prompt order you follow the steps by entering email and password 
from your heroku account
now you are connected.
```
### step 10:
```console
create your apps on heroku with : heroku create the_name_of_your_app
make :
```
```js
git status
git add --all
git commit -m "commit name"
heroku git:remote -a the_name_of_your_app
git push heroku master
heroku run bash
python manage.py migrate
python manage.py createsuperuser
```



go to [the_name_of_your_app.herokuaoo.com]() ..............................it's Work

- [x] Congratitulations




