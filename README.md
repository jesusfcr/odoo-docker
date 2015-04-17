About this Repo
======

This is the Git repo of the official Docker image for [Odoo](https://registry.hub.docker.com/_/odoo/). See the Hub page for the full readme on how to use the Docker image and for information regarding contributing and issues.

The full readme is generated over in [docker-library/docs](https://github.com/docker-library/docs), specifically in [docker-library/docs/odoo](https://github.com/docker-library/docs/tree/master/odoo).


I've updated the information about how to launch the docker images

docker run -d -e POSTGRES_USER=odoo -e POSTGRES_PASSWORD=odoo -p 5432:5432 --name db postgres

docker run -v /path/to/config:/etc/odoo -v /path/to/addons:/mnt/extra-addons -p 8069:8069 --name odoo --link db:db -t odoo
