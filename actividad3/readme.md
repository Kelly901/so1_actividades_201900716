### Universidad de San Carlos de Guatemala
### Facultad de Ingeniería
### Sistemas Operativos 1


#### Kelly Mischel Herrera Espino
#### 201900716

## Comandos


### Creaciòn de usuarios:

#### Usuario 1

    sudo useradd usuario1

#### Usuario 2

    sudo useradd usuario2
#### Usuario 3

    sudo useradd usuario3

<img src="Imagenes/creacionUsuarios.png" alt="Texto alternativo" width="400" height="auto">

### Asignaciòn de contrasenas

    sudo passwd usuario1
    1234

    
    sudo passwd usuario2
    123
    
    sudo passwd usuario3
    123

<img src="Imagenes/asignacionPassword.png" alt="Texto alternativo" width="400" height="auto">

### Informaciòn de Usuario
 
#### Usuario 1
    id usuario1

<img src="Imagenes/infoUsuario1.png" alt="Texto alternativo" width="400" height="auto">


### Eliminación de Usuario
 
#### Usuario 3
    userdel usuario3
    
<img src="Imagenes/eliminarUsuario3.png" alt="Texto alternativo" width="400" height="auto">

#### Comnando para verificar que ya no esta el usuario

    cat /etc/passwd

<img src="Imagenes/verUsuarios.png" alt="Texto alternativo" width="400" height="auto">


### Creaciòn de grupos:

#### Grupo1

    sudo groupadd grupo1

    sudo groupadd grupo2

<img src="Imagenes/crearGrupos.png" alt="Texto alternativo" width="400" height="auto">

### Agregar Usuarios a los grupos

#### Uusario1 al grupo1

    sudo usermod -a -G grupo1 usuario1


#### Uusario2 al grupo2

    sudo groupadd grupo2

<img src="Imagenes/usuarioAgrupo.png" alt="Texto alternativo" width="400" height="auto">

### Verificar Membresìa
    groups usuario1
    groups usuario2
### Eliminar grupo2
    sudo groupdel grupo2

<img src="Imagenes/eliminarGrupo2.png" alt="Texto alternativo" width="400" height="auto">


### Gestionar Permisos

Inicio de sesiòn con el usuario:

    su -usuario1

### Creaciòn del archivo

    echo "Hola mundo, archivo1" > ~/archivo1.txt

Direcctorio y archivo:

    mkdir ~/directorio1

    echo "Hola mundo2" > ~/directorio1/archivo1.txt

###  ¿Por qué es importante gestionar correctamente los usuarios y permisos en un sistema operativo?

Es importante debido a que de esta forma se puede mantener la seguirda y privacidad de los datos en uns SO.
