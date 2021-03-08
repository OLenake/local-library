<p align="center">
  <p align="center">
    <a href="https://demos.lenake.co.za/" target="_blank">
      <img src="https://lenake.co.za/services/fs/static/images/brand/visiondream/logo.svg" alt="VisionDream" height="72">
    </a>
  </p>
  <p align="center">
      Your Vision, Your Dream.
  </p>
</p>

# Python Django: Local Library Website

A barebones Python Django app, which can easily be deployed to Heroku.

## Running Locally

Make sure you have Python 3.9 [installed locally](http://install.python-guide.org). To push to Heroku, you'll need to install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli), as well as [Postgres](https://devcenter.heroku.com/articles/heroku-postgresql#local-setup).

```sh
$ git clone https://github.com/OLenake/local-library.git
$ cd local-library

$ mkvirtualenv env
$ pip3 install -r requirements.txt

$ createdb local_library

$ py -3 manage.py migrate
$ py -3 manage.py collectstatic

$ heroku local
```

Your app should now be running on [127.0.0.1:8000](http://127.0.0.1:8000/).

## Deploying to Heroku

```sh
$ heroku create
$ git push heroku main

$ heroku run python manage.py migrate
$ heroku open
```
or

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)

## Documentation

For more information about using Python on Heroku, see these Dev Center articles:

- [Python on Heroku](https://devcenter.heroku.com/categories/python)
