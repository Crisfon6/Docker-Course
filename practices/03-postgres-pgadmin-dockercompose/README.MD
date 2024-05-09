# Solucion del problema de pgadmin permisos

Para solucionar el problema de permisos del pgadmin la solucion que encontre fue correr el docker compose como root:

    `sudo docker compose up`
In the moment you try make the connection of pgadmin4 to postgresql, the name of the host is the name of the service in the docker-compose file, in this case is `db`:

    `host: db`
![Example Here]('../../../../resources/img/hostname.png)