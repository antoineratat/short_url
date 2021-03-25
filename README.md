## ShortURL

## Table of contents

-   [General info](#general-info)
-   [Technical Details](#technical-details)
-   [Screenshots](#screenshots)
-   [Classes](#classes)
-   [Technologies](#technologies)
-   [Setup](#setup)

## General info

URLs can be extremely long and not user-friendly. When people share links or even try to remember a URL, it’s difficult because most URLs are filled with more difficult characters and don’t form meaningful words. This is where the URL Shortener comes in. A URL Shortener reduces the characters or letters in a URL, making them easier to read and remember. A URL like xyz.com/wwryb78&svnhkn%sghq?sfiyh can be shortened to xyz.com/piojwr. With the URL Shortener, URLs become a joy to work with.

## Technical Details

The main objective of this project idea is to shorten URLs. The main task the application will accomplish is to shorten URLs and then redirect users to the original URL when the shortened URL is visited. In the application, the users will input the original URL, and they will get the new, shortened URL as the result. To do this, you can use a combination of the random and string modules to generate the characters for the shortened URL. Since users will visit the shortened URL days, months, or even years after, you’ll need to save the original and shortened URLs in a database. When a request comes in, the application checks if the URL exists and redirects to the original, or else it redirects to a 404 page.

## Screenshots

![Pokemon Screenshot](https://github.com/antoineratat/pokemon_python/blob/master/screenshots/screenshot_1.png?raw=false) ![Pokemon Screenshot](https://github.com/antoineratat/pokemon_python/blob/master/screenshots/screenshot_1.png?raw=false)

## Classes

1.  Pokemon (pokemon_class.py)

    -   is_active()
    -   get_status()
    -   is_alive()
    -   is_target_alive()
    -   knock_out()
    -   revive()
    -   lose_health()
    -   restore_health()
    -   damage_boost()
    -   set_name()
    -   level_up()
    -   add_xp()
    -   check_xp()
    -   attack()

2.  Trainer (trainer_class.py)

    -   show_pokelist()
    -   add_pokelist()
    -   remove_pokelist()
    -   set_active()
    -   use_potion()
    -   attack_trainer()

## Technologies

Project is created with:

-   Python v3.9.0
-   astroid v2.4.1
-   click v7.1.2
-   colorama v0.4.3
-   Flask v1.1.2
-   Flask-SQLAlchemy v2.4.3
-   Flask-WTF v0.14.3
-   isort v4.3.21
-   itsdangerous v1.1.0
-   Jinja2 v2.11.2
-   lazy-object-proxy v1.4.3
-   MarkupSafe v1.1.1
-   mccabe v0.6.1
-   pybase62 v0.4.3
-   pylint v2.5.2
-   six v1.15.0
-   SQLAlchemy v1.3.17
-   toml v0.10.1
-   Werkzeug v1.0.1
-   wrapt v1.12.1
-   WTForms v2.3.1

## Setup

To run this project, clone it and start index.html

### On Windows:

Create Environnement Variable :

```
$ SECRET_KEY = '12345678912345678912345678912312'
$ // input your own 32 digits secret key
```

Import project

```
$ git clone https://github.com/antoineratat/ShortURL.git
$ py -3 -m venv venv
$ venv\Script\Activate
$ pip install -r requirements.txt
$ cd ShortURL
$ python .\run.py
```

Initialize Database (site.db SQlite - Can be connected to other DB in [config.py](config.py) with SQLALCHEMY_DATABASE_URI)

```
$ venv\Script\Activate
$ python
$ python
$ from run import db
$ db.create_all()
$ exit()
```
