lo que hemos añadido han sido los archivos del compose.yaml el dockerfile y requirements.txt asi de primeras.

Stage 0:

En el Requirements.txt ponemos las versiones que necesitamos:

<img width="398" height="151" alt="image" src="https://github.com/user-attachments/assets/b14588cd-775a-44f2-8a82-cff9d9d6ca75" />

Luego en el compose.yaml:

<img width="726" height="621" alt="image" src="https://github.com/user-attachments/assets/c8b1c1e9-8940-4b5e-a976-e064720b1c31" />

    En el Web:
Construimos una imagen usando el Dockerfile y guardamos archivos estaticos en un volumen compartido para que NGINX puedan acceder

    En nginx:
Es un prox Inverso, haciendo uso de una imagen liviana (importante, arranca despues del contenedor Web)
Sirve archivos media, recibe peticiones Http sirviendo a static/ y media/ 

