# Bootstrap Prestashop app with Docker Compose

Quickly setup a Prestashop ready-to-use environment in one command.

To use the [prestashop's official container](https://hub.docker.com/r/prestashop/prestashop/), you need in addition, a MySQL container, and a network that let both last containers to communicate between them. This Docker Compose file let you do those 3 steps in one command.

## How to use

1. Clone this repo and go inside the created directory

2. If you're using ***Dotenv*** file, rename `.env.example` to `.env`

3. Replace values inside `.env` to match youre need.

4. If you're not using ***Dotenv*** file, configure [Prestashop](https://github.com/PrestaShop/docker) and [MySQL](https://hub.docker.com/_/mysql) with environment variables inside `docker-compose.yml`.

5. You can add addtionnal environment variables for MySQL and Prestashop in `docker-compose.yml` (see theire docs for available one).

6. Run bellow command

```bash
# Launch an Apache server and MySQL server inside the same network
docker-compose up -d

# Bring down the environment by removing all containers and networks associated with this environment
docker-compose down
```
