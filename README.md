# Postgres en Docker

> IMPORTANTE: esta no es ni por cerca una configuración recomendada para producción.

Esta es una configuración para levantar una instancia de Postgres con Adminer para administrarla de un solo comando.

Modificar el archivo `.env` con los datos propios.

Para instalarla por primera vez:

> Debemos estar siempre dentro de esta carpeta, para que docker-compose reconozca la imagen con la que tratamos

```bash
docker-compose up
```

Luego para detener simplemente corremos el siguiente comando:

```bash
docker-compose stop
```

Para iniciar el contenedor una vez ya estando instalada:

```bash
docker-compose start
```

Para quitar la imagen o reiniciarla:

```bash
docker-compose stop # para detener los contenedores

docker-compose rm # removemos la imagen contestamos con "y"

docker-commpose down # damos de baja a la imagen y redes configuradas

docker-compose down --volumes # damos de baja las imagenes persistentes
```
