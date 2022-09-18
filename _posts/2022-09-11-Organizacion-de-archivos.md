---
layout: single
title: Python - Organizador de archivos
excerpt: "Este script te permite ordenar archivos ubicados en una carpeta para posteriormente agruparlos en carpetas segun su extension de archivo `[ .jpg - .png - mp3 - mp4 - .docx - .gif ]`"
date: 2022-09-11
classes: wide
header:
  teaser: /assets/images/python.png
  teaser_home_page: true
  icon: /assets/images/code.png
categories:
  - Python
  - Programacion
tags:  
  - Python
  - Archivos
  - Programacion
---



Primero que nada debemos importar la librería `os` para realizar lectura y escritura de archivos en nuestro equipo
después debemos declarar todas las carpetas que se verán involucradas, para este ejemplo ordenaremos los archivos que se encuentran en mi carpeta de descargas, las demás carpetas serán las que recibirán los archivos según su extensión, por ejemplo:
la carpeta picturesFolder almacenara todos los archivos cuya extensión sea `[.jpg, .png, .jpeg, .gif]`.

![](/assets/images/htb-writeup-delivery/delivery_logo.png)

## Carpetas

Guardamos en variables los directorios de las carpetas que vamos a usar mas adelante

```python 
import os

downloadsFolder = "/Users/brand/Downloads/"
picturesFolder = "/Users/brand/Downloads/Imag/"
videosFolder = "/Users/brand/Downloads/Videos/"
compFolder = "/Users/brand/Downloads/Comp/"
programFolder = "/Users/brand/Downloads/Programs/"
musicFolder = "/Users/brand/Downloads/Music/"
docFolder = "/Users/brand/Downloads/Docs/"

```

Posteriormente dentro de `main` utilizando la librería `os` recorremos con un **for** todos los archivos existentes dentro del directorio `downloadsFolder` previamente declarado.

```python
if __name__ == "__main__":
    for filename in os.listdir(downloadsFolder):
        name, extension = os.path.splitext(downloadsFolder + filename)
```
Dentro del **for** utilizaremos condicionales *if* para evaluar si la extensión del archivo pertenece al grupo de extensiones que queremos incluir dentro de la misma carpeta (este proceso lo podemos repetir cuantas carpetas hayamos creado para los conjuntos de archivos seleccionados)

```python
 if extension in [".jpg", ".jpeg", ".png", ".gif"]:
            os.rename(downloadsFolder + filename, picturesFolder + filename)
            print(name + ": " + extension)

        if extension in [".mp3"]: 
            os.rename(downloadsFolder + filename, musicFolder + filename)
            print(name + ": " + extension)

        if extension in [".mp4", ".3gp"]:
            os.rename(downloadsFolder + filename, videosFolder + filename)
            print(name + ": " + extension)

        if extension in [".pdf", ".docx", ".txt"]:    
            os.rename(downloadsFolder + filename, docFolder + filename)
            print(name + ": " + extension)

        if extension in [".zip"]:  
            os.rename(downloadsFolder + filename, compFolder + filename)
            print(name + ": " + extension)

        if extension in [".c", ".exe"]:   
            os.rename(downloadsFolder + filename, programFolder + filename)
            print(name + ": " + extension)
```
nota que dentro del *if* utilizamos la funcion *rename* de la libreria `os` para cambiar la ubicacion del archivo (*filename*) ubicado en la carpeta (*downloadsFolder*) para posteriormente indicarle cual será su nueva ubicacion 

#### Codigo 
Puedes encontrar todo el codigo y copiarlo o descargarlo desde- [este repositorio](https://github.com/BrandonFilth/folder-classification/blob/main/main.py)

