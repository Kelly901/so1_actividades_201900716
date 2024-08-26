### Universidad de San Carlos de Guatemala
### Facultad de Ingeniería
### Sistemas Operativos 1
### Actividad 5

#### Kelly Mischel Herrera Espino
#### 201900716


[Tipos de Kernel y sus diferencias](#tipoKernel)

[User vs Kernel Mode](#userVsKernel)

[Interruptions vs traps](#IntVsTraps)


## Tipos de Kernel y sus diferencias <a id="tipoKernel"></a>
### ¿Què es el Kernel?
<p style="text-align:justify; ">
El Kernel es la parte que se encarga de la organziaciòn de los procesos y datos en cada ordenador. Es la interfaz que comunica el software y el hardware. 
</p>

### Tipos de Kernel
#### Kernel monolìtico
<p style="text-align:justify; ">Este tipo de kernel puede gestionar todas la tares, debido a su tamaño. Gestion ala memoria y procesos, asì como la comunicaciòn entre los proceso y el soporte de las diferentes funciones de los drivers y el hardware.
</p>

#### Microkernel
<p style="text-align:justify; ">Es un kernel con un tamaño pequeño, el cual evita el colpaso total del sistema en caso de un fallo. 
</p>

#### Kernel hìbrido
<p style="text-align:justify; ">Este es la combianciòn entre el microkernel y el kernel monolìtico. Este tipo de kernel puede ser modulado y otras partes del kernel pueden cargarse de manera dinamica.
</p>

### Diferencias 
<p style="text-align:justify; ">La diferencia entre los tipos de kernel radica en la forma en que se manejan las fucnionalidades del sistema, los tamaños dle kernel y en el caso de algunos la modularidad.
</p>

## User vs Kernel Mode <a id="userVsKernel"></a>
<p style="text-align:justify; ">
En el caso de User, se tiene un menor nivel de acceso con respecto a los privilegios. Debido a la restriccion de los recursos del sistema y no se pueden ejecutar opereaciones crìtica del sistema o un contacto directo al hardware. Tambien hace un ailamiento de las aplicaciones de usuario del sistema opeativo, protegiendo el sistema de fallos o errores en aplicaciones. Por otro lado el Kernel Mode brinda un mayor nivel de privilegios, el còdigo tiene un acceso completo a los recursos del sistema y se pued eejecutar y manipular el hardware directamente.
</p>


## Interruptions vs traps <a id="IntVsTraps"></a>
<p style="text-align:justify; ">Las Interrupciones son señales las cuales se envian al procesador desde el hardware o el softeare que dietenen de forma temporal la ejecuciòn actual y desvìan el control a una rutina especial. Cabe mencionar que cuando ocurre una interrupciòn, la CPU detiene su tarea actual, guarda su estado y ejecuta el manejador de itnerupciones.
Ahora en el caso de los Traps, son un tipo de inturcciòn que ocurre cuando hay un aexcepciòn o condiciòn especial dentro de la ejecuciòn del programa. Este realiza un manejo de erroes que requieren de atenciòn inmeidante. 

</p>