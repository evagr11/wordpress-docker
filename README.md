# Wordpress + MariaDB + Adminer

Con este `docker-compose.yml` puedes lanzar un Wordpress con MariaDB y Adminer.

Lanza el siguiente comando en la carpeta donde tengas el `docker-compose.yml`:

```bash
docker-compose up -d
```

Esto levantará los siguientes contenedores:

- `wordpress`: Wordpress en el puerto 8080
- `adminer`: Adminer en el puerto 8081
- `mariadb`: MariaDB en el puerto 3306

## Acceso a Wordpress

Accede a Wordpress en `http://localhost:8080` y sigue las instrucciones para configurar tu Wordpress.

## Acceso a Adminer

Aunque puedes conectarte al contenedor de MariaDB y usar el cliente de MariaDB, es más fácil usar Adminer para gestionar la base de datos de forma grafica.

Accede a Adminer en `http://localhost:8081` y utiliza las siguientes credenciales para conectarte a la base de datos:

- **Motor de base de datos**: `MySQL/MariaDB`
- **Servidor**: `db`

Tienes dos usuarios para conectarte a la base de datos:

- **Usuario**: `root`
- **Contraseña**: `rootpass`

- **Usuario**: `wordpress`
- **Contraseña**: `wordpress`

Puedes ajustar las credenciales en el archivo `docker-compose.yml`.

