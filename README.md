README
======

[![Circle CI](https://circleci.com/gh/pelias/pelias-vagrant.png?style=badge)](https://circleci.com/gh/pelias/pelias-vagrant)

Notes
-----
* WORK IN PROGRESS!!!

Requirements
------------
* [VirtualBox](https://www.virtualbox.org/wiki/Downloads) >= 4.3.18
* [Vagrant](https://www.vagrantup.com/downloads.html) >= 1.6.5

Getting Started
---------------
* running `vagrant up` will:
  * boot a linux instance that you can interact with via `vagrant ssh`
  * install all the dependencies required to run Pelias:
    * elasticsearch
    * nodejs
    * required Pelias repositories
    * other system dependencies
  * create the Elasticsearch 'pelias' index
  * load Geonames data into Elasticsearch
  * load an OSM extract of New York City into Elasticsearch
  * run the Pelias API server, which you can interact with locally via your browser, curl, etc thanks to the magic of port forwarding: [API](http://localhost:3100/search?input=Empire&lat=40.7903&lon=73.9597)
