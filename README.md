tweetwall
=========

A simple tweetwall in python using django

The app is base on https://github.com/ryanmcgrath/twython-django and use twython


To make the app work you need to register an app on twitter website
and add the following elements in "settings.py":

TWITTER_KEY = 'your_key'
TWITTER_SECRET = 'your_secret'

Before running the app

pip install django
pip install twython

python manage.py syncdb


