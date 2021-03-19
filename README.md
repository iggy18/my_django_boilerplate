A Django Starter Template

This template has all auth included. you'll need to wire it up to suit your needs, but if you alter the templates in the complete auth acounts file your forms will change accordingly. this will allow you to customize the forms as you see fit.

this template will also include a postgress server, and be set up for deployment with Docker, NGINX, and Gunincorn. should make for easy deployment.

you'll need to install requirements.txt

you'll need to setup your own .env file and plug in variable values but the .env file should look like this:

SECRET_KEY=


DEBUG=


DATABASE_NAME=


DATABASE_USER=


DATABASE_PASSWORD=


DATABASE_HOST=


DATABASE_PORT=


you can generate a new "SECRET_KEY" from the command line:
- `python` enter 
- `from django.core.management.utils import get_random_secret_key` enter
- `print(get_random_secret_key())` this should print a new secret key that you can post into your .env file.
