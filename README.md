# Week4UrlShortner
Side Hustle 5.0 Bootcamp Portfolio Python Team 2 - URL Shortner API project for Week 4. In collaboration with members of the Side Hustle 5.0 Portfolio Python Team 2

The following are the Endpoints;
Shortener API ListView - http://127.0.0.1:8000/api/
Shortener API CreateView - http://127.0.0.1:8000/api/create/
Swagger Graphical View - http://127.0.0.1:8000/swagger/
Redoc Documentation - http://127.0.0.1:8000/redoc/
Redirecting from the Shortened Link back to the Original Link - http://127.0.0.1:8000/shortened_link"/

This URL Shortener can be upgraded to generate only unique shortened link for one original link
It can also be upgraded to request users to register and login before using the URL Shortner

Please note that the serialization file is named serializer.py and NOT serializers.py as is the practice with most Developers

Url Shortener API
Url Shortener API with Django Rest Framework.

Project consists to allow a user to transform a long web url into a pattern-consistent (encoded) small url easy to share and remember.

At the same time the user is allowed to transform back (decode) the shortened url into the original url

It is partly tested and was developed as showcase only.

How Url Shortener API Works:

You can send (POST) a full url and retrieve a small encoded one with http://127.0.0.1:8000 as the base web service url.

Eg. POST http://localhost:8000/api/create/ with https://github.com/AdesegunAdesolaADEBOYE/Week4UrlShortner/new/main?readme=1 result: http://127.0.0.1:8000/ztjFCR (6 digits id)

You can get the original url with the encoded url on a GET request (done in previous step)

Eg. GET http://127.0.0.1:8000/ztjFCR result: https://github.com/AdesegunAdesolaADEBOYE/Week4UrlShortner/new/main?readme=1




Index:
Installation
Installing Django API App
Usage:
Available Endpoints


Installation:
1.Installing Django API App
Clone repository and go inside the repository folder "url-shortener-api"
git clone https://github.com/AdesegunAdesolaADEBOYE/Week4UrlShortner
Create you virtualenv and install the packages
pip install -r requirements.txt
Initialize database and create the database mapping used for persistance in the url shortener API.
python manage.py makemigrations
Apply the database mapping from the app to the database; migrate the database.
python manage.py migrate
Run the application.
python manage.py runserver


USAGE
1. Endpoint List
URI Example: http://localhost:8000/api/

Available Methods	URI	Example URL
Project Endpoints		
1.	POST	shorten-url/	http://localhost:8000/api/create/
2.	GET	/<short_id>	http://localhost:8000/api/


