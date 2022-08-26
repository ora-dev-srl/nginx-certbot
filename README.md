# Boilerplate for nginx with Let’s Encrypt on Docker Compose

`init-letsencrypt.sh` fetches and ensures the renewal of a Let’s
Encrypt certificate for one or multiple domains in a docker-compose
setup with nginx.
This is useful when you need to set up nginx as a reverse proxy for an
application.

## Installation
1. [Install docker-compose](https://docs.docker.com/compose/install/#install-compose).

2. Clone the repository.

3. Modify configuration:
- Add domains and email addresses to domains.sh (see domains.sh.example).
- Add Nginx configuration for all domains in data/nginx/$domain.conf (see data/nginx/app.conf.example).

4. Run the init script:

        ./init-letsencrypt.sh

5. Run the server:

        docker-compose up

## License
All code in this repository is licensed under the terms of the `MIT License`. For further information please refer to the `LICENSE` file.
