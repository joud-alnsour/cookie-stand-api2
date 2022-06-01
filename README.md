# Getting started
- Check the app remotely
     - This Django API app is deployed in the AWS.
     - Database is deployed in the Elephantsql.
     - Check the app at http://18.208.134.116:8000/api/cookie_stand/
- Check the app in the local machine

note: Database is deployed in the Elephantsql. Your local app will be connected to this remote database.

     - Clone down the repo.
     - Download .env file and add it under cookie_stand_project folder. Make sure rename the file to .env.
     - Run command docker-compose up --build -d to start docker container.
     - Run command docker-compose run web python manage.py makemigrations and docker-compose run web python manage.py migrate to migrate.
     - Run command docker-compose run web python manage.py createsuperuser and follow the prompt to create a super user.
     - Run command docker-compose run web python manage.py collectstatic to create static files.
     - Check out the app at http://0.0.0.0:8000/api/cookie_stand/.
     - Run command docker-compose down to shot down the container.
