Provisioning a new site
=======================

## Required packages:

* nginx
* Python 2.7
* Git
* pip
* virtualenv

eg, on Ubuntu:

    sudo apt-get install nginx git python2.7 python-pip
    sudo pip3 install virtualenv

## Nginx Virtual Host config

* see nginx.template.conf
* replace SITENAME with, eg, staging.my-domain.com

## Upstart Job

* see gunicorn-upstart.template.conf
* replace SITENAME with, eg, staging.my-domain.com

## Folder structure:
Assume we have a user account at /home/username

/home/ubuntu
└── sites
    └── SITENAME
         ├── source
         ├── static
         └── virtualenv