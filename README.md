# Actividad 5.3



### INSTITUTO TECNOLÓGICO DE ESTUDIOS SUPERIORES DE MONTERREY
SEDE: Santa Fe 


#### Actividad Integradora 5.3 Resaltador de sintaxis paralelo


##### Implementación de métodos computacionales



### PRESENTAN: 
                                              
#### Javier Corona Del Río                A01023063
#### Ian Seidman                               A01028650
#### Leonardo Ramírez Landa	   A01379391









### Profesores:
#### Gilberto Echeverria
### Junio 2021


## Speedup

Se midió el tiempo con “Time” en paralelo dando 36,403 milisegundos -> 36.4 segundo

![Time_paralelo](https://user-images.githubusercontent.com/75320318/120883923-b3197d80-c5a5-11eb-998e-1c4a438865d6.png)



De la misma manera se midió el tiempo real total secuencial dando un total de 34,488 milisegundos -> 34.4 segundos.

![Time_secuencial](https://user-images.githubusercontent.com/75320318/120883929-c2003000-c5a5-11eb-909f-c7f712920344.png)


Speedup resultante: 34488/36403 = 0.947

## Complejidad


La complejidad del algoritmo es O(n) al igual que lo fue en el resaltador de sintaxis original. Esto es porque el paralelismo adicional implementado con esta versión del código simplemente repite el mismo proceso con la cantidad de archivos en el directorio. En este ejemplo sería O(4n) que al tomar en cuenta la complejidad O grande simplemente resulta en una complejidad de O(n). 

## Reflexión


Se puede identificar que el proyecto de racket cumplió su funcionamiento de correrse en diferentes cores pero desafortunadamente el tiempo real fue mayor al secuencial. Se identifica que se corrió en paralelo porque se utilizan todos los cores disponibles en el sistema para revisar los archivos por cada core disponible.

Hay varias maneras de hackear una computadora, normalmente se hace para robar contenido sensible o de alta importancia. Se puede encontrar muchas maneras en donde sea vulnerable el hardware de cada dispositivo determinado. Una manera que se relaciona al trabajo que se realizó es por medio de un meltdown se logre acceder a la memoria. Se le facilita a los hackers si se tiene un procesador vulnerable, se ejecuta algún OS sin las más recientes actualizaciones que protejan al usuario. Es muy difícil de detectar y es muy común en los procesadores Intel, no se sabe bien si en AMD. Recomendamos tener el sistema operativo con las actualizaciones más recientes para detectar archivos maliciosos. A continuación pondré un video que demuestra lo fácil que se puede hacer esto:

[![Alt text](https://img.youtube.com/vi/RbHbFkh6eeE/0.jpg)](https://www.youtube.com/watch?v=RbHbFkh6eeE)

En este video se ve cómo esta persona corre un programa y desafortunadamente sus datos son expuestos. Nosotros cómo conocedores de las computadoras y sus funciones debemos ser capaces de medirnos en estos tipos de aspectos porque fácilmente podemos caer en tentaciones de hacer o saber más de lo que deberíamos con programas maliciosos o con dispositivos físicos. Se tiene que tener una ética y valores fijos para entender la severidad de nuestros actos si traspasamos esta línea porque si lo hacemos podremos encontrar información sensible que nos pudiese poner en peligro. En conclusión debemos mantenernos informados para no filtrar información sensible accidentalmente en un futuro no muy lejano y mantenernos pendientes de las miles de consecuencias que existen si hacemos un acto así. 
