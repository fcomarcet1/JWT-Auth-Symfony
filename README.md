# docker-symfony-skeleton

## Getting Started

1. Clona el repositorio.
2. Renombrar `docker-compose.yml.dist` a `docker-compose.yml` y configura tus parámetros.
3. Ejecuta `cd ~/symfony-docker-skeleton` && `make run` para levantar los contenedores(nginx + php8.0 + MySQL8)
4. Ejecuta `make ssh-be` para entrar al container.
5. Ejecuta `composer create-project symfony/skeleton my_project_name` para construir un nuevo proyecto de microservicios o aplicacion de consola. 
6. Ejecuta `composer create-project symfony/website-skeleton my_project_name` para contruir un nuevo proyecto web tradicional.
7. Accede el servidor local de desarrollo para comprobar que funciona correctamente: `http://localhost:250`.
8. DB MySQL 8.0 for testing.
7.Happy codding!

### Scripts
*Using **Makefile***: https://makefiletutorial.com/

Installs composer dependencies

```shell
make prepare
```

Build the containers

```shell
make build
```

Start the containers

```shell
make run
```

Stop the containers

```shell
make stop
```

Restart the containers

```shell
make restart
```

### Steps to follow

Init the bash shell into the **Backend container**

```shell
make ssh-be
```

Update packages

```shell
composer update
```

Install packages

```shell
composer install
```


### Optional
*Use dry to manage docker*: https://github.com/moncho/dry#installation

```shell
curl -sSf https://moncho.github.io/dry/dryup.sh | sudo sh
sudo chmod 755 /usr/local/bin/dry
```

Listen docker containers

```shell
dry
```
## Authors

Contributors names and contact info

- Francisco Marcet Prieto  
  [Linkedin](https://www.linkedin.com/in/fcomarcetprieto/)

## Version History

* 0.1
    * Initial Release

## License

This project is licensed under the [MIT] License - see the LICENSE.md file for details# JWT-Auth-Symfony
