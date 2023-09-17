---
layout: post
title:  "Manejando el tráfico de Kafka"
date:   2020-08-26 20:00:00 -0500
categories: jekyll update
---
En Shopify tenemos frecuentemente ráfagas masivas (2-5x) de tráfico que presionan nuestra infraestructura incluyendo nuestros clusters de Kafka. 
Hemos logrado hacer nuestros clusters más resilientes a estas oleadas regionales de tráfico redirigiendo porciones de tráfico a clusters más desocupados durante incidentes. 
En esta charla voy mostrarles nuestra infraestructura de Kafka que corre en Kubernetes sobre la plataforma de Google Cloud. 
Después voy a explicar nuestra solución para hacer failovers usando DNS y librerías de clientes personalizadas. 
Finalmente vamos a revisar escenarios reales donde este sistema nos salvó de cortes mayores.

Mira la [grabacion][grabacion] y las [slides][slides] del [meetup][meetup].

[meetup]: https://www.meetup.com/quito-lambda-meetup/events/272256532
[grabacion]: https://www.youtube.com/watch?app=desktop&v=ZgueGdxcgJ4Activa&ab_channel=QuitoLambda
[slides]: https://www.slideshare.net/VanessaVuibert/manejando-el-trafico-de-kafkapdf
