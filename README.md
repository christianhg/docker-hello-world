# docker-hello-world

As learned in: https://www.youtube.com/watch?v=YFl2mCHdv24.

Build the image with the name `hello-world`:

```
docker build -t hello-world .
```

Run the image with port `80` forwarded from the host to the container:

```
docker run -p 80:80 hello-world
```

Run using a mounted volume (development mode):

```
docker run -p 80:80 -v /Users/christian/code/docker-hello-world/src/:/var/www/html/ hello-world
```

`/Users/christian/code/docker-hello-world` is the path to this folder.
