# codeigniter4-docker-compose
Initial configuration for a project using Code Igniter 4 and Docker

## What the repository has

* Code Igniter 4 - v4.0.0-rc.3  
* Docker-compose start file
* PHP 7
* Nginx
* PhpMyAdmin
* MySQL
* Nginx Reverse Proxy

## Getting start

First make the clone of this repository
```html
$ git clone https://github.com/mathmed/codeigniter4-docker-compose.git
```

With the repository ready, open the file `.env` located at the root and configure it according to your database host.


Go to `codeigniter4-docker-compose/web/app/app/Config` and open the file `Database.php`. Change the database fields for them used in the `.env` file.

After configuring the files, go to the root of the project and execute  
```html
$ sudo docker-compose up -d
```

done, the application is ready for use.


## Accessing

To access your project, type in your browser  
```html
http://localhost:8080
```

To access the phpmyadmin, type in your browser  
```html
http://localhost:9191
```

### Container shell

To access a container shell, type in your terminal

```html
$ sudo docker exec -ti <container_name> /bin/sh/
```


### Code Igniter 4 docs

For details on how to use Code Igniter 4, visit the [documentation](https://codeigniter4.github.io/userguide/).
