# Docker-Dev-Env

Docker-Dev is a devolempent evirement made width docker and docker compose 

## Usage

 ###### 1 . put your projects files in the right place

```
docker-dev/
┣ Back/            # put your laravel project files here 
┃ ┗ docker/
┃   ┣ Dockerfile
┃   ┗ vhost.conf
┣ Front/           # put your angular project files here
┃ ┗ Dockerfile
┣ LICENSE.md
┣ README.md
┗ docker-compose.yaml
```

###### 2 . Run With Docker Compose

```
 sudo docker-compose up
```
###### 3 . Open your browser at

```
  http://localhost:4200/  # your frontend (angular)

  http://localhost:8000/  # your backend (laravel)
 
  http://localhost:7000/  # you can access an manage your data base wdidh phpMyAdmin

```

###### 4 . To execute cli commands

if you need to exectute cli commands you must have run this commands inside the container.

so you have too ways to do that

* use the sub-command 
```
 docker-compose exec <servcie-name> <your-commande>
``` 
  example:

```
docker-compose exec back php artisan migrate
```
*  you can get an interactive prompt with :

```
docker-compose exec <service-name> sh
```
  example:
```
docker-compose exec front sh
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[licence.txt](LICENSE.md)