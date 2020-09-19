# Installation Guide

There are several types of installation available.

## Requirements

* 32-bit or 64-bit operating system
* Python 2.6 or 2.7
* Urban Terror 4.1, 4.2 or 4.3 in the latest version

!!! note ""
    Spunky Bot is running 'out of the box', there are no other software dependencies.

## Download

Download the latest version of Spunky Bot from the download section:
```
$ wget https://spunkybot.de/download/spunkybot-x.x.x.tar.gz
```
Extract the archive:
```
$ tar -xzvf spunkybot-x.x.x.tar.gz
```
Move the extracted folder to the location you want to place your files to:
```
$ sudo mv spunkybot-x.x.x /opt/spunkybot
```
Set the ownership of this folder to the same user and group running your Urban Terror server:
```
$ sudo chown -R q3ut4:q3ut4 /opt/spunkybot
```

## APT package repository

You can also install Spunky Bot via our APT package repository:

```bash
$ wget -qO- https://apt.spunkybot.de/key.asc | sudo apt-key add -
$ echo "deb http://apt.spunkybot.de/ stable main" | sudo tee /etc/apt/sources.list.d/spunkybot.list
$ sudo apt-get update
$ sudo apt-get install spunkybot
```

!!! tip "Hint"
    For more details, please check: [https://apt.spunkybot.de](https://apt.spunkybot.de)

## Ubuntu PPA

It is also possible to install Spunky Bot via our Ubuntu PPA (Personal Package Archive):

```bash
$ sudo add-apt-repository ppa:alexanderkress/spunkybot
$ sudo apt-get update
$ sudo apt-get install spunkybot
```

That’s it!

## Python and source tarball

If you have pip installed, the easiest way of getting Spunky Bot is to use:

```
$ pip install spunkybot
```

!!! tip "Hint"
    PyPI - the Python Package Index: [https://pypi.org](https://pypi.org)

If you have downloaded a source tarball you can install it by doing the following:

```
$ python setup.py install
```

## Development version

You can also test against our git repository using the development branch as follows:

```bash
$ git clone https://github.com/SpunkyBot/spunkybot.git
$ cd spunkybot
$ git checkout develop
```

!!! note "Note"
    Development builds are not officially supported. If you have problems, please try to use the stable version of Spunky Bot.
