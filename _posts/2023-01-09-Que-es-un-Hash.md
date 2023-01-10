---
layout: single
title: Informatica - ¿Que es un Hash?
excerpt: "Entendiendo los hashes: cómo funcionan y cuál es su papel en la 
informática y la criptografía "
date: 2023-01-09
classes: wide
header:
  teaser: /assets/images/Que-es-un-Hash/hash.png
  teaser_home_page: true
  icon: /assets/images/Iconos-Tematica/informatica.png
categories:
  - Informatica
  - Blockchain
tags:  
  - Crypto
  - Blockchain
  - Informatica
---

Un *hash* es una función matemática que toma una cadena de datos de cualquier tamaño
como entrada y devuelve una cadena de datos de tamaño fijo como salida. Un hash es una
herramienta muy útil en informática, ya que se utiliza en muchas aplicaciones
diferentes.

## Usos comunes de los hashes:
<br>
- Verificar la integridad de los datos: Los hashes se utilizan a menudo para verificar
que los datos no se hayan alterado durante la transmisión o el almacenamiento. Por
ejemplo, cuando descargas un archivo de Internet, el sitio web puede proporcionar un
hash del archivo. Luego, puedes calcular el hash del archivo que has descargado y
compararlo con el hash proporcionado para asegurarte de que el archivo no se haya
dañado o alterado.
<br>
- Almacenar contraseñas: En lugar de almacenar las contraseñas en texto claro, muchos
sitios web utilizan hashes para proteger las contraseñas de los usuarios. Cuando un
usuario introduce su contraseña, el sitio web la hashea y la compara con el hash 
almacenado. Si los hashes coinciden, significa que la contraseña es correcta. Esto es 
muy útil para proteger las contraseñas de los usuarios en caso de que un atacante 
consiga acceder a la base de datos de contraseñas.
<br>
- Generar claves únicas: Los hashes se utilizan a menudo para generar claves únicas
para identificar a los usuarios o a los objetos. Por ejemplo, muchos sitios web
utilizan hashes para generar claves únicas para los enlaces de descarga, para evitar
que los usuarios compartan enlaces no autorizados.

<p align="center">
<img src="/assets/images/Que-es-un-Hash/p-hash.png">
</p>

## Algoritmos de cifrado
Hay muchos algoritmos de hash diferentes disponibles, cada uno con sus propias 
características y usos. Algunos ejemplos comunes de algoritmos de hash son:

- *MD5:* El algoritmo de hash MD5 (Message Digest Algorithm 5) es uno de los algoritmos 
más comunes y se utiliza a menudo para verificar la integridad de los datos. Toma 
cualquier cantidad de datos como entrada y devuelve una cadena de 128 bits como salida.<br> 
Por ejemplo:

```python
  import hashlib

  # Creamos un objeto de hash MD5
  md5_hash = hashlib.md5()

  # Podemos proporcionar los datos que queremos hashear como una cadena
  md5_hash.update("Hola mundo")

  # Obtenemos el hash como una cadena hexadecimal
  md5_hex = md5_hash.hexdigest()

  print(md5_hex)  # Imprime "ed076287532e86365e841e92bfc50d8c"
```

Aunque MD5 es muy utilizado, ha sido atacado y hay algunas vulnerabilidades conocidas. 
Esto significa que, aunque es muy útil para verificar la integridad de los datos, no es 
tan seguro como algunos otros algoritmos.

- *SHA-1:* El algoritmo de hash SHA-1 (Secure Hash Algorithm 1) es similar a MD5 y se 
utiliza a menudo para verificar la integridad de los datos. Toma cualquier cantidad de 
datos como entrada y devuelve una cadena de 160 bits como salida. 
<br>
Por ejemplo:

```python
  import hashlib

  # Creamos un objeto de hash SHA-1
  sha1_hash = hashlib.sha1()

  # Podemos proporcionar los datos que queremos hashear como una cadena
  sha1_hash.update("Hola mundo")

  # Obtenemos el hash como una cadena hexadecimal
  sha1_hex = sha1_hash.hexdigest()

  print(sha1_hex)  # Imprime "2ef7bde608ce5404e97d5f042f95f89f1c232871"
``` 
Aunque SHA-1 es más seguro que MD5, también ha sido atacado y hay algunas 
vulnerabilidades conocidas.

- *SHA-256:* El algoritmo de hash SHA-256 (Secure Hash Algorithm 256) es una versión más segura del algoritmo SHA y se utiliza a menudo en la criptografía. Toma cualquier 
cantidad de datos como entrada y devuelve una cadena de 256 bits como salida.
<br>
Por ejemplo:

```python
  import hashlib

  # Creamos un objeto de hash SHA-256
  sha256_hash = hashlib.sha256()

  # Podemos proporcionar los datos que queremos hashear como una cadena
  sha256_hash.update("Hola mundo")

  # Obtenemos el hash como una cadena hexadecimal
  sha256_hex = sha256_hash.hexdigest()

  print(sha256_hex)  # Imprime "185f8db32271fe25f561a6fc938b2e264306ec304eda518007d1764826381969"
```
Aunque SHA-256 es más seguro que MD5 y SHA-1, también ha sido atacado y hay algunas 
vulnerabilidades conocidas. Sin embargo, es considerado generalmente más seguro que 
otros algoritmos de hash y ses comunmente utilizado en aplicaciones de criptografía.

## Areas y sus aplicaciones 

Además de su uso en aplicaciones informáticas, los hashes también se utilizan en otras 
áreas, como la criptografía y la ciencia de la información. Por ejemplo, en la 
criptografía, los hashes se utilizan a menudo como parte de los sistemas de firma 
digital para verificar la autenticidad de los documentos y mensajes.

En la ciencia de la información, los hashes se utilizan a menudo para indexar y 
recuperar información. Por ejemplo, en un motor de búsqueda, el texto de cada página 
web se hashea y se almacena en una base de datos. Cuando un usuario realiza una 
búsqueda, el motor de búsqueda hashea la búsqueda y busca páginas web con hashes 
similares en la base de datos. Esto permite al motor de búsqueda recuperar rápidamente 
páginas web relevantes sin tener que examinar cada página web individualmente.

En conclusión, un hash es una función matemática que se utiliza en muchas aplicaciones 
informáticas y en otras áreas para realizar tareas como verificar la integridad de los 
datos, proteger contraseñas, generar claves únicas y indexar y recuperar información. 
Aunque hay muchos algoritmos de hash diferentes disponibles, es importante elegir el 
adecuado para cada aplicación para garantizar la seguridad y la eficiencia. Los hashes 
son una herramienta muy útil en informática y continúan siendo una parte importante de 
muchos sistemas y aplicaciones.

<script async src="https://www.googletagmanager.com/gtag/js?id=G-QBRV3CHHNN"></script>
<script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());

    gtag('config', 'G-QBRV3CHHNN');
</script>
