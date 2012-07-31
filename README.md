gitoriouscli
============

Simple gitorious cli to create/delete a project on your local server

Install
-------

    pip install https://github.com/locojay/gitoriouscli.git

add the following line to environment.rb in /var/www/gitorious/config:

    config.action_controller.allow_forgery_protection = false

TODO: do some more scrapping and test why adding   authenticity_token to post data
produces an internal server error

Usage
-----

data)

*create project:

    gitoriouscli --host https://locojaydev --user locojaydev@gmail.com --pwd **** --project testproject

*delete project

    gitoriouscli --host https://locojaydev --user locojaydev@gmail.com --pwd **** --project testproject --delete

