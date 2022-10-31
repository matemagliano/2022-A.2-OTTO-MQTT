<div align="center">
  <h1 align="center">Bitacora</h1>
</div>

## 15 de Agosto
* Comenzamos la investigación del robot OTTO DIY. Información obtenida en la página oficial https://www.ottodiy.com/ 
* Definimos los objetivos y requerimientos.

## 20 de Agosto 
* Recolectamos la información requerida para poder comenzar con el proyecto:
  - Investigamos cómo usar un broker MQTT y como hacer imágenes en Docker.
  - Como usar Python Flask para hacer un servidor HTTP.
  - Como hacer que el robot funcione como cliente MQTT.

## 1 de Septiembre
* Buscamos cómo funciona un transistor para amplificar corriente y como conectarlo.

## 5 de Septiembre
* Se entregó el Plan de Proyecto.

## 15 de Septiembre
* Se recibe el kit otto: su impresión 3d, Nodemcu Wifi ESP8266, 4 Mini Servos Tower Pro Sg90, Hc-sr04 Sensor De Distancia Ultrasónico, 

## 20 de Septiembre
* Se desarmó el Otto para comenzar las pruebas y mediciones para alimentar a los servos.
* Compramos 4 transistores Transistor 2N2222A, Resistencia de 220Ω y Protoboard 830 Puntos.
* Comenzamos con las pruebas para alimentar un servo conectándolo con un transistor.
* Quemamos un transistor. Compramos un transistor nuevo.-.-

## 29 de Septiembre
* Realizamos pruebas para comprobar cómo deberían estar conectados los 4 transistores con los 4 servos.
* Se realizaron las medidas y se concluyó qué conexión correspondía.
* Se armó el Otto.

## 8 de Octubre

## 31 de Octubre
* Se realizo la conexion entre el broker MQTT y un cliente en el ESP8266 para que responda a un mensaje.
* Se montó el broker MQTT con el protocolo mosquitto en Docker. Se intentó con el siguiente código:
mosquitto.conf<br>
  persistence true<br>
  persistence_location /mosquitto/data/<br>
  log_dest file /mosquitto/log/mosquitto.log<br>

No se conecta, entonces lo intentamos con :<br>

allow_anonymous true<br>
listener 1883<br>
persistence true<br>
persistence_location /mosquitto/data/<br>
log_dest file /mosquitto/log/mosquitto.log<br>

* Se comprobó la comunicación con dos aplicaciones: MQTT Explorer en una computadora y con MQTT Client en un teléfono móvil.
* Se levantó un access point con la computadora.

## 10 de Octubre
* Investigamos sobre Kafka 
https://www.baeldung.com/ops/kafka-docker-setup
https://developer.confluent.io/quickstart/kafka-docker/
https://towardsdatascience.com/how-to-install-apache-kafka-using-docker-the-easy-way-4ceb00817d8b 
