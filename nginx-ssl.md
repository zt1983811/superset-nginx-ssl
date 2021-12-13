# How to setup SSL with nginx

* get ssl certificate and private key and copy them to
  nginx/ssl/crt.pem and nginx/ssl/private.pem
* replace domain in nginx/nginx.conf under server_name section
* build:
    ```sh
      docker-compose -f docker-compose-non-dev-nginx.yml build --no-cache
    ```
* start:
    ```sh
      docker-compose -f docker-compose-non-dev-nginx.yml up --force-recreate
    ```
