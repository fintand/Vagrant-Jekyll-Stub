# Vagrant Jekyll Stub

Use this Vagrant setup for developing with Jekyll. The base box is "scotch/box".
Learn more here: <https://box.scotch.io/>

## Installation
> vagrant up

Note this can take some time

## Running
> vagrant ssh

Check that jekyll has been installed:
> jekyll

## Quickstart

> `jekyll new myblog`

> `cd myblog`

> `jekyll serve --port 8000 --host 0.0.0.0 --detach`

## Building
> `kill -9 pid`, for stopping detached serve.
> Go to browser on <http://192.168.33.10:8000> or http://vagrant.me:8000/ [after changing hosts file]
