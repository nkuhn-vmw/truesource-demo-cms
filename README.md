# truesource-demo-cms

A demo marketing site for [TrueSource Viewer](https://github.com/nkuhn-vmw/truesource-viewer-hub-edition).
It is not meant to run: it pins container images on purpose.

- `bitnami/wordpress:6.4.3` and `bitnami/phpmyadmin:5.2.1`: images that bundle PHP, so they need
  rebuilt versions when PHP ships a fix such as PHP2Shell.
- `php:8.2.20-apache`: PHP 8.2 without the PHP2Shell fix (8.2.35).
- `nginx:1.25`: a release line past its end of life.
