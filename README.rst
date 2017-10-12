base-nginx
===========

.. |dockerbuild| image:: https://img.shields.io/docker/build/mkovac/base-nginx.svg
.. |dockerpulls| image:: https://img.shields.io/docker/pulls/mkovac/base-nginx.svg
.. |dockerstars| image:: https://img.shields.io/docker/stars/mkovac/base-nginx.svg

|dockerbuild| |dockerpulls| |dockerstars|

The NGINX `container <https://hub.docker.com/r/mkovac/base-nginx/>`_ built on top of the `base-debian <https://github.com/multicast/base-debian.git>`_ (`docker hub <https://hub.docker.com/r/mkovac/base-debian/>`_).

Usage
=====

If you clone, run::

    $ make && docker run --rm -ti mkovac/base-nginx bash

or simply::

        $ docker build --rm -t somename \
          --build-arg "ftp_proxy=${ftp_proxy}" \
          --build-arg "http_proxy=${http_proxy}" \
          --build-arg "https_proxy=${https_proxy}" \
          .

Then just::

    $ docker run --rm -ti somename bash

