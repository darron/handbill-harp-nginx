handbill-harp-nginx
==================

You don't need to use node to serve a harp site - you can just compile the files and use anything - `harp compile`

This is a container that has node and harp available, to compile and install the static site, that nginx serves.

You can use our container: `docker pull octohost/handbill-harp-nginx`

Or you can build your own:

```
docker build -t your-name-here/handbill-harp-nginx .
docker push your-name-here/handbill-harp-nginx
```

Then, you can add [Dockerfile.site](https://github.com/darron/handbill-harp-nginx/blob/master/Dockerfile.site) to your Harp site.

Push it to your docker server - and your server will use 4-6MB of RAM instead of 60MB.
