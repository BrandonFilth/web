---
layout: single
title: Cripto - ¿Que es la tecnologia Blockchain?
excerpt: "Aqui entenderas que es y como funciona la tecnologia blockchain, sus tipos y de que esta conformada [Bloques, Mineros y Nodos]"
date: 2022-11-02
classes: wide
header:
  teaser: /assets/images/blockchain.png
  teaser_home_page: true
  icon: /assets/images/Iconos-Tematica/Cripto.png
categories:
  - Crypto
  - Blockchain
tags:  
  - Crypto
  - Blockchain
---

La *blockchain* es un libro público compartido y duplicado en varios dispositivos, los cuales
se vuelven validadores de la red al tener una copia de esta misma, procesando cada 
transacción, la cual genera un `hash` único que es añadido en el bloque más reciente, una
vez que el bloque está completo se acopla a la cadena de bloques. Llevando así un  
seguimiento histórico de todas las transacciones hechas de cualquier activo que se opere dentro de esa red.

Al convertirte en validador de la red o *"minero"* estás prestando tu poder de cómputo y 
resolución de algoritmos a cambio de una comisión, de esta forma estas aportando 
seguridad a la red, haciendo que sea imposible realizar algún registro o bloque fraudulento
(a menos de que tengas el 51% de poder de *minado* o procesamiento de dicha *blockchain*)
<p align="center">
<img src="/assets/images/Tecnologia-Blockchain/FakeTransac.gif">
</p>
Como te conté antes, al convertirte en validador de la red estas gastando electricidad y prestando tu poder de cómputo para hacer la red más segura. Resolviendo problemas matemáticos
mayormente basados en el algoritmo de cifrado SHA256.

A diferencia de una red centralizada o servidores de almacén de datos, una *blockchain* 
corre en múltiples dispositivos alrededor del mundo, lo que la hace descentralizada y difícil
de censurar, ya que no depende de una entidad o gobierno que la pueda regular tan fácilmente.

## Elementos principales

### Bloques:
Un *bloque* está constituido por transacciones las cuales se conforman en 3 partes:
remitente (entidad que envía), destinatario (entidad que recibe) y `hash` el cual es generado
para esa transacción conteniendo sus datos únicos
<p align="center">
<img src="/assets/images/Tecnologia-Blockchain/bloques.gif">
</p>

### Mineros:
Los *mineros* son ordenadores dedicados a procesar y validar las transacciones, al 
completar un *bloque* de transacciones el *minero* recibirá una recompensa en forma de la 
`cripto` nativa de esa red, por ejemplo `Bitcoin`.
<p align="center">
<img src="/assets/images/Tecnologia-Blockchain/miner.gif">
</p>

### Nodo:
Un *nodo* es un ordenador dedicado a almacenar y distribuir una copia con cada nuevo 
*bloque* que se confirma. Los *nodos* están comunicados entre sí, por lo que este nuevo
*bloque* será distribuido a todos los demás *nodos* que estén en dicha red.
<p align="left">
<img src="/assets/images/Tecnologia-Blockchain/PoW.gif">
</p>

## Tipos de blockchain

### Pública 
Una *blockchain* pública puede ser accesible a cualquier usuario del mundo, el cual puede 
crear un *nodo* con solo un ordenador y conexión al internet, el punto bueno y malo de una
blockchain pública es que a mayor número de validadores la red es más segura, pero en 
contraparte al tener pocos la red se hace vulnerable a ataques o a transacciones fraudulentas.
Aunque existen varios protocolos de consenso y medidas de seguridad como
el `PoW` *(proof of work)* o prueba de trabajo y el `PoS` *(Proof of Stake)* o prueba de participación
Teniendo como ejemplo  a `Bitcoin` en `Pow` y a `Ethereum` en `PoS` el cual antes, al igual que `Bitcoin` 
era `PoW` pero con el Merge en este 2022 cambió a PoS para ser más amigable con el medio ambiente

### Publica 
Una *blockchain* privada a diferencia de una pública depende y solo da acceso a una entidad centralizada 
(empresa, organización o individuo). Aunque contiene los mismos elementos que una *blockchain* pública.
Una de las más conocidas es [Hyperledger](https://www.hyperledger.org/)

### Híbrida
Una *blockchain* híbrida combina las dos anteriores haciéndola personalizable, donde los miembros de esta 
pueden elegir quienes participan en la red o qué transacciones se harán públicas, garantizando transparencia 
y privacidad al mismo tiempo. ya que así información delicada no será publicada ni se podrá saber quienes 
son los integrantes de la red si no tienes acceso a ella. Como ejemplo de *blockchain* híbrida tenemos a [XinFin](https://xinfin.org/) 

