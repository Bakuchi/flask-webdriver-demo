Flaskr - a minimal blog application with extra Sauce [![Sauce Test Status](https://saucelabs.com/buildstatus/flask-webdriver-demo)](https://saucelabs.com/u/flask-webdriver-demo) [![Build Status](https://travis-ci.org/christian-bromann/flask-webdriver-demo.svg?branch=master)](https://travis-ci.org/christian-bromann/flask-webdriver-demo)
====================================================

[![Sauce Test Status](https://saucelabs.com/browser-matrix/flask-webdriver-demo.svg)](https://saucelabs.com/u/flask-webdriver-demo)

## What is Flaskr?

A sqlite powered thumble blog application based on [Flask](http://flask.readthedocs.org/en/latest/).

## Installation

Clone the repo first

```sh
$ git clone git@github.com:christian-bromann/flask-webdriver-demo.git
$ cd flask-webdriver-demo
```

Virtualenv is probably what you want to use during development, and if
you have shell access to your production machines, you’ll probably want
to use it there, too.

```sh
$ sudo easy_install virtualenv
```

or

```sh
sudo pip install virtualenv
```

Now, whenever you want to work on a project, you only have to activate
the corresponding environment. On OS X and Linux, do the following:

```sh
. venv/bin/activate
```

Then install all requirements:

```sh
$ pip install -r requirements.txt
```

## Run tests

Replace the existing Sauce Labs credentials in the `.travis.yml` with
yours by executing

```sh
$ travis encrypt SAUCE_USERNAME=YOUR_USERNAME --add
$ travis encrypt SAUCE_ACCESS_KEY=YOUR_ACCESS_KEY --add
```

Run the test via

```sh
nosetests --processes=30
```