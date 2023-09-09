# Laboratorio Robótica Industrial No. 1
#### Por Guillermo Alejandro Cano Rodrigues y Sergio Andres Gerena Gomez

## Descripción de la solución planteada
La solución propuesta implica la utilización de una herramienta con un ángulo de 45° para evitar problemas de alineamiento de ejes al mover el brazo robótico. Para lograrlo, se ha creado un modelo de las letras en Autodesk Inventor y se ha exportado al entorno virtual de Robot Studio.

Adicionalmente, se ha llevado el brazo robótico a una posición cercana a las letras mencionadas anteriormente mediante un movimiento de las articulaciones, con el fin de prevenir problemas de alineamiento o singularidad durante el proceso de aproximación. Las trayectorias diseñadas para las letras consisten en un desplazamiento desde su posición inicial, seguido de una trayectoria que rodea las letras, y finalmente, se retorna al punto de partida para dirigirse a la siguiente letra sin causar daños en la superficie.

Se ha diseñado una rutina de movimiento en el plano de la torta para generar las letras y la figura en forma horizontal, cumpliendo con las restricciones del proyecto, que incluyen el tamaño de la torta para 20 personas, la velocidad de movimiento en un rango de 100 a 1000 unidades, una tolerancia máxima de error de 10 unidades, y la partida y llegada del movimiento en una posición especificada, que puede ser la posición inicial del robot.

Además, se ha considerado que la decoración de la torta se lleva a cabo sobre papel, que puede estar fijado en una superficie horizontal o en un plano inclinado, y se ha asegurado que los nombres estén separados adecuadamente.

## Diagrama de flujo de acciones del robot
![image](https://github.com/sagerenag/lab1_robotica/assets/144469847/98e5528d-39e1-4444-8be5-c8dadef594f3)

## Plano de planta de la ubicación de cada uno de los elementos
A continuacion se muestra el esquema de la planta, con cada una de las partes en ella y su ubicacion espacial tomando como centro del eje coordenado el centro inferior del robot, con base en ello es que se muestran las diversas posiciones.

![image](https://github.com/sagerenag/lab1_robotica/assets/144469847/ad972b63-61eb-4138-8d78-505e04ee942c)

Aca se encuentran las partes fisicas que constituyen la pplanta como lo es el brazo robotico, la herramienta diseñada de la cual se hablara mas adelante la cual se coloca en el portaherramienta del brazo ABB y la torta simulada, en la cual se hace la decoracion y los nombres que se piden en el laboratorio.

![image](https://github.com/sagerenag/lab1_robotica/assets/144469847/6e2454e8-60cf-46ec-943a-4c2a02983129)

Aca encontramos la ubucacion del centro de la torta respecto a la base del robot. Las distancias, como lo indica la imagen, se encuentran en milimetros
## Descripción de las funciones utilizadas

## Diseño de la herramienta
Para el diseño de la herramienta, primero se elaboraron las piezas en inventor, luego se imprimieron las piezas en 3D y se realizo el ensamble final.

![image](https://github.com/sagerenag/lab1_robotica/assets/144469847/f78e6c44-390b-484c-b5c3-ff3a90e0689b)
![image](https://github.com/sagerenag/lab1_robotica/assets/144469847/9bca63c5-093d-40e2-b5e3-01a628fb042f)

Por partes inciamos con la base que va al portaherramienta del robot, esta base se diseño siguiendo las dimensiones y forma que se evidencian en el manual del robot, asi tenemos una pieza con 4 perforaciones de 6mm donde se posicionan los tornillos para fijar la herramienta al brazo robotico, tambien cuenta con un orificio central roscado de 28,9mm de diametro en el cual, se ensamblara el resto de la herramienta.
![image](https://github.com/sagerenag/lab1_robotica/assets/144469847/2ec41ee9-a1b7-414b-a272-338849e4bc4c)

la siguiente pieza del ensamble es un codo el cual sirve en la herramienta para dar apertura y cierta distancia dentre la punta de la herramienta y el brazo robotico, este codo tiene un angulo principal de 135° y una altura de 60,64mm, tambien las dos partes que conecta tienen diferente radio, es el puente entre la rosca de la base y el soporte del marcador.
![image](https://github.com/sagerenag/lab1_robotica/assets/144469847/a3eaf72d-9070-444b-b687-5feaa93c292d)

por ultimo se encuentra el soporte del marcador, este es simplemente una t custom donde se aloja el marcador, esta internamente ajusta al marcador permitiendo que este pueda inclinarse, voltearse y demas sin que pierda su posicion o modifique la posicion de la punta del marcador como se muestra a continuacion
![image](https://github.com/sagerenag/lab1_robotica/assets/144469847/71a88352-0ff8-431d-b923-fbf12287f695)

## Código en RAPID del módulo utilizado para el desarrollo de la práctica
El codigo RAPID se encuentra en la carpeta RAPID de este mismo repositorio

## Videos
### Simulacion 
https://www.youtube.com/watch?v=-XPKKv97MK0&ab_channel=JuanDicaprio-GuillermoDelToroProfesores 
