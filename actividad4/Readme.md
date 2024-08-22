### Universidad de San Carlos de Guatemala
### Facultad de Ingeniería
### Sistemas Operativos 1


#### Kelly Mischel Herrera Espino
#### 201900716

## Comandos


#### Craecion del Script

    # Bucle
    fecha=$(date)


    while true 
        do # se agrega una line abajo del while
        echo "Saludos cordiales, hoy $fecha"
        sleep 1
    done     

#### Permisos al archivo
    chmod +x Script.sh

#### Servicio

Para crear el servicio realizamos lo sigueinte>

    sudo nano/etc/systemd/system/saludar.service

Despues de ejecutar el comando anterios se abre un editor, en donde colocamos lo siguiente:

    [Unit]

    Description=Descripcion de servicio

    [Service]
    ExecStart=/home/kelly/Documents/SistemasOperativos/Magistral/so1_actividades_201900716/actividad4/script.sh
    Restart=always

    [Install]
    WantedBy=multi-user.target


Habilitacion de el srvicio

    sudo systemctl daemon-reload

Habilitacion para que el servicio inicie:

    sudo systemctl enable saludar.service

Para poder ve el estado del servicio

    sudo systemctl start saludar.service


