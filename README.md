tweetwall
=========

A simple tweetwall in python using django

The app is base on https://github.com/ryanmcgrath/twython-django and use twython


To make the app work you need to register an app on twitter website
and add the following elements in "settings.py":

TWITTER_KEY = 'your_key'
TWITTER_SECRET = 'your_secret'

Note:
Twitter does not recognize localhost callback url for registering an app
Using a url minifier like bit.ly does the trick for testing in dev environment

Before running the app

pip install django
pip install twython

python manage.py syncdb


TODO

Automatic update of the wall:
using ajax call (or investigate streaming feature of the API)

Send a tweet from the wall:
Function ready but not tested (because of write authorization of the twitter app)

Share the tweetwall:
Send an automated tweet with a link to the wall (cannot be implemented without write authorization for the app)

Front-end:
Use bootstrap to make the app less painful for the eyes

Security:
Use csrf token for the form to send a tweet
check length of the tweet on server side before sending to the api

Read config from env variable:
recommendation of 12factor apps
