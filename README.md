# HOST-DJANGO-PROJECT-ON-HEROKU
HOST DJANGO PROJECT ON HEROKU




hello, directory was created to help all those who have difficulty
hosting their django project on heroku.
follow each of the following steps and everything should be fine.

step 0:
install git
install heroku cli

Step 1:
create an empty folder on your desktop and move your project inside

2nd step:
create a new virtual environment and install django there.

steps 3: 
make a python manage.py runserver,
normally it should fail.
don't worry that's the goal


step 4: 
install each of the required packages and restart your server.

if your application launches normally in the new environment stop the server and now we can go to the next step


step 5:
create a file named Procfile without extension and inside this file add the following line:

web: gunicorn the_name_of_your_project.wsgi
