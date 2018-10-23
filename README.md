

Docker Image at the Hub
------------

Fetch the public image with

    docker pull jpizarrom/freeling:dev-4.1


Test it with

    echo "Mi casa es bonita." | docker run -i jpizarrom/freeling:dev-4.1 /usr/bin/analyze -f es.cfg


There is also a Python API. Test it with

    echo "Mi casa es bonita." | docker run -i jpizarrom/freeling:dev-4.1 python3 /home/APIs/python3/sample.py



Freeling Docker Image
---------------


Besides docker the procedures depends on
- m4 (probably it's already installed)
- docker-squash
- tar GNU compatible

Squashing the image requires your local root password.


The underline OS of this image is Debian jessy 64.
If you want to build your image by yourself use:

    make build-es
    make squash-es



Debian Package
--------------

The Freeling Debian packages is:

    https://github.com/TALP-UPC/FreeLing/releases/download/4.1/freeling-4.1-stretch-amd64.deb freeling4.deb


Original code
------------
Based on https://github.com/hfoffani/docker-freeling


