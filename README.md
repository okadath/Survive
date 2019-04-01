# Comandos ridiculamente utiles:
```
tree
sudo ap-get install tree
```
opciones:
+ `-a` archivos invisibles
+ `-d` solo folders
+ `-f` ruta full
+ `-L 2` limita la profundidad del arbol
+ `-I *palabra` despliega los archivos que no tengan esa palabra
+ `--matchdirs` desploega solo los que coincidan con ese nombre(para solo imprimir una carpeta sin ir a ella)
+ `-Q` pone los nombres entre comillas
+ `-p` imprime permisos
+ `-F` añade un `/`  para directorios, un `=` para archivos de socket, un `*` 'para archivos ejecutables, un `>` para puertas (Solaris) y un ` |` para FIFO's.
+ `--noreport` asi no imprime el conteo de archivos

``tree -I *.pyc``
``tree -I nombre_folder_a_evitar``


```shell 
.
├── blog_project
│   ├── __init__.py
│   ├── __pycache__
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── manage.py
├── posts
│   ├── admin.py
│   ├── apps.py
│   ├── __init__.py
│   ├── migrations
│   │   └── __init__.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
└── README.md

4 directories, 15 files
```
```
  756  pip install django
  757  django-admin startproject blog_project
  758  ls
```

history
imprime los comandos anteriormente usados:
```shell
history 10
history | grep git #imprime los que posean esa cadena
history | more #imprime todo el archivo
```
imprime el ultimo comando
```shell
!!#ultimo usado
sudo !!
echo "!!" > script.sh
!pyth #ultimo usado conesa cadena
```

imprime los ultimos comandos usados de la consola en un archivo eliminando los numeros de history
```
 history 10 | awk '{$1 = ""; print}' >>file2
```

