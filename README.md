lo que hemos añadido han sido los archivos del compose.yaml el dockerfile y requirements.txt asi de primeras.

Stage 0:

El compose.yaml:

<img width="726" height="621" alt="image" src="https://github.com/user-attachments/assets/c8b1c1e9-8940-4b5e-a976-e064720b1c31" />

    En el Web:
Construimos una imagen usando el Dockerfile y guardamos archivos estaticos en un volumen compartido para que NGINX puedan acceder

    En nginx:
Es un prox Inverso, haciendo uso de una imagen liviana (importante, arranca despues del contenedor Web)
Sirve archivos media, recibe peticiones Http sirviendo a static/ y media/ 

Dockerfile:

<img width="832" height="178" alt="image" src="https://github.com/user-attachments/assets/8a8cbd68-4a66-47d4-90d1-a1d8ea369add" />

En el Requirements.txt ponemos las versiones que necesitamos:

<img width="398" height="151" alt="image" src="https://github.com/user-attachments/assets/b14588cd-775a-44f2-8a82-cff9d9d6ca75" />


Stage 1:
Primero que nada tuvimos que eliminar "django browser reload" que se encontraban de la carpeta Principal(en mi caso personalblog)
en urls.py y teniendose que qeudar asi:

<img width="720" height="212" alt="image" src="https://github.com/user-attachments/assets/253b864a-5078-4302-b017-68e83944e9b0" />

En settings.py (en dos sitios) teniendose que quedar asi:

<img width="406" height="328" alt="image" src="https://github.com/user-attachments/assets/8d312c7a-2e01-428a-87c5-174780afc72e" />

<img width="670" height="218" alt="image" src="https://github.com/user-attachments/assets/bb423c32-6626-4ce4-bdba-907ef51056b9" />






