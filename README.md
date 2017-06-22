# Introducción

El objetivo de este desarrollo es de proporcionar un HMI (Human-Machine Interface, o interfaz hombre-máquina) para un robot autónomo del tipo AGV (Automatic Guided Vehicle, o vehículo de guiado automático).

Para ello, se contará con un simulador de funcionamiento del AGV totalmente compatible con un robot real en funcionamiento en circuito cerrado ubicado en el exterior del evento GaliciaTIC.

El robot está configurado para realizar un circuito en forma de óvalo, con dos paradas (estaciones) en las que dejar/recoger carga. En el propio robot (real o mediante simulador) se ejecuta un proceso servidor que, a través de un sencillo protocolo basado en JSON permite interaccionar con el robot (obtener información, actuar, etc.).
 
El robot recibe órdenes de movimiento en forma de "goals" (o puntos de destino, que son las estaciones), así como órdenes de marcha/paro. Además, proporciona información periódica acerca de su estado y posición (coordenadas y orientación).

# Descripción de la funcionalidad objetivo

El interfaz hombre-máquina deberá estar desarrollado en AngujarJS o Angular 2 - 4 y el objetivo es que cuente con las siguientes funcionalidades (ordenadas de mayor a menor interés):

* Visualización en tiempo real de la posición (localización y orientación) del robot en la planta industrial. Para ello, como base se proporciona una imagen de la planta que incluye las estaciones preconfiguradas.
* Visualización sobre el mapa de los puntos de destino.
* Visualización continua del estado del robot y destino actual.
* Envío sencillo de puntos de destino al robot.
* Envío de comandos de marcha y paro.
* Visualización de Avisos y Alarmas
* Consulta del listado de estaciones de destino del robot. 

A modo de ejemplo se incluye un mockup del HMI a desarrollar:

# Recursos proporcionados

* Documentación del protocolo de comunicaciones JSON a utilizar contra el servidor embarcado en el robot.
* Imagen con el plano del circuito que recorre el robot y las estaciones preconfiguradas.
* Imagen representativa del robot (vista en planta)
* Capturas de pantalla de una aplicación básica de ejemplo

