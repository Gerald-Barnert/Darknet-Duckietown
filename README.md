# DeepLearning-Duckietown
En este proyecto se utilizaron herramientas de Deep Learning para implementar un sistema de detección de objetos en tiempo real. Especificamente se trabajo con YOLO.
## YOLO
YOLO es un sistema para detectar objetos. Este utiliza localizadores o clasificadores para la detección. Se aplica el modelo a una imagen en multiples lugares y a distintas escalas. Las regiones con alto nivel de puntuación se consideran detecciones.
## Darknet
Darknet es el framework de redes neuronales con la que se implementa YOLO.
## Proyecto
Buscamos detectar objetos con la camara del duckiebot. En este caso se trabajara con 2 clases: duckiebots y patos. Lo primero es tomar fotos de los objetos a detectar. Una vez hecho esto, se procede a etiquetar las imagenes:

>1) Insertar la imagenes en **main/input**
>2) Insertar las clases en **class_list.txt**
>3) Ejecutar: ```python run.py```



https://github.com/pjreddie/darknet

https://github.com/leggedrobotics/darknet_ros

https://github.com/Cartucho/OpenLabeling
