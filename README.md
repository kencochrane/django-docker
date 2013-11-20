django-docker
=============

Demo Django App using Docker


Dockerfile
----------
Use this to build a new image

    $ sudo docker build .

With a tag for easier reuse

    $ sudo docker build  -t <your username>/django-docker .

Running the container

    $ sudo docker run -d -p :8000 <your username>/django-docker
    
Get your container's IP Address:

    sudo docker inspect <container_id> | grep IPAddress | cut -d '"' -f 4

Now go to `<your container's ip>:8000` in your browser

