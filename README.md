# DeepLearning-Duckietown
En este proyecto se utilizaron herramientas de Deep Learning para implementar un sistema de detección de objetos en tiempo real. Especificamente se trabajo con YOLO.
## YOLO
YOLO es un sistema para detectar objetos. Este utiliza localizadores o clasificadores para la detección. Se aplica el modelo a una imagen en multiples lugares y a distintas escalas. Las regiones con alto nivel de puntuación se consideran detecciones.
## Darknet
Darknet es el framework de redes neuronales con la que se implementa YOLO. Su instalacion queda detallada en la siguiente guia: [Installing Darknet](https://pjreddie.com/darknet/install/). Ademas sera necesario implementarlo junto con Ros: [YOLO ROS: Real-Time Object Detection for ROS](https://github.com/leggedrobotics/darknet_ros)
## Proyecto
Buscamos detectar objetos con la camara del duckiebot. En este caso se trabajara con 2 clases: duckiebots y patos. Lo primero es tomar fotos de los objetos a detectar. Una vez hecho esto, se procede a etiquetar las imagenes:

>1) Insertar la imagenes en **main/input**
>2) Insertar las clases en **class_list.txt**
>3) Ejecutar: ```python run.py```

Esto generara un archivo .txt. Luego ejecutar: ```python process.py``` para procesar los archivos y poder entrenarlos en YOLO.
#### Entrenamiento
Para entrenar, seguimos los pasos dichos en esta guia: [How to train YOLOv3 to detect custom objects](https://medium.com/@manivannan_data/how-to-train-yolov3-to-detect-custom-objects-ccbcafeb13d2). 





https://github.com/pjreddie/darknet

https://github.com/leggedrobotics/darknet_ros

https://github.com/Cartucho/OpenLabeling
