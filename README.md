# Partkeepr Docker

[![Build Status](https://github.com/maksimstojkovic/docker-partkeepr/actions/workflows/docker-build.yml/badge.svg)](https://github.com/maksimstojkovic/docker-partkeepr)
[![Docker Pulls](https://img.shields.io/docker/pulls/maksimstojkovic/partkeepr)](https://hub.docker.com/repository/docker/maksimstojkovic/partkeepr)
[![Docker Stars](https://img.shields.io/docker/stars/maksimstojkovic/partkeepr)](https://hub.docker.com/repository/docker/maksimstojkovic/partkeepr)
[![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/maksimstojkovic/partkeepr)](https://hub.docker.com/repository/docker/maksimstojkovic/partkeepr)
[![Docker Image Version (latest by date)](https://img.shields.io/docker/v/maksimstojkovic/partkeepr)](https://hub.docker.com/repository/docker/maksimstojkovic/partkeepr)

Image of Partkeepr built using PHP7.1 and Nginx-fpm. Running the included `docker-compose.yml` creates a Partkeepr stack using MariaDB 10.0, with default database settings preconfigured in the Partkeepr setup page available at http://localhost:8080/setup (connect using hostname `database` in Partkeepr setup).

## Volumes

* `/partkeepr/app/config`: Partkeepr configuration folder.
* `/partkeepr/data`: Partkeepr data folder.
* `/partkeepr/web`: Partkeepr website root folder.

The authentication key generated during setup can be retrieved using:

```shell
docker exec partkeepr cat app/authkey.php
```
