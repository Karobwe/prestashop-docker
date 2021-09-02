# Bootstrap Prestashop app with Docker Compose

Quickly setup a Prestashop ready-to-use environment in one command.

To use the [prestashop's official container](https://hub.docker.com/r/prestashop/prestashop/), you need in addition, a MySQL container, and a network that let both last containers to communicate between them. This Docker Compose file let you do those 3 steps in one command.

```bash
# Launch an Apache server and MySQL server inside the same network
docker-compose up -d

# Bring down the environment by removing all containers and networks associated with this environment
docker-compose down
```
