gitoriouscli
============

Simple gitorious cli to create/delete a project on your local server

Install
-------

    pip install git+https://github.com/locojay/gitoriouscli.git

add the following line to environment.rb in /var/www/gitorious/config:

    config.action_controller.allow_forgery_protection = false

TODO: do some more scrapping and test why adding   authenticity_token to post data
produces an internal server error

Usage
-----


* create project :

    gitoriouscli --host https://locojaydev --user locojaydev@gmail.com --pwd **** --project <projectname>

This will add to project <projectname> a repository <projectname>

* create project with different reponame

    gitoriouscli --host https://locojaydev --user locojaydev@gmail.com --pwd **** --project <projectname> --repo <reponame>

* delete project

    gitoriouscli --host https://locojaydev --user locojaydev@gmail.com --pwd **** --project testproject --delete

* delete repo at project:
    Todo

* list projects
    Todo

