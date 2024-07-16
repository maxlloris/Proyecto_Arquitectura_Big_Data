# **Big Data Architecture** - Proyecto



### Objetivo
Este trabajo tiene como objetivo definir la arquitectura necesaria para la elaboración de un servicio de emails diarios informando sobre noticas de caracter financiero.
El cliente sobre el que centro mi servicio son los Day traders que operan en FOREX.

Forex (Foreign Exchange) es el mercado financiero del mundo con un volumen medio de 4 billones de dólares al día. Este mercado se basa en pares de divisas que cotizan, tales con el EURUSD o GBPUSD.
Es un mercado muy popular entre los inversores y day traders retails por el fácil acceso y la posibilidad de operar sin tener en cuenta noticias, twits o comunicados de empresas específicas. El Forex responde más a la situación macroeconómica y a la actitud de ciertos organismos gubernamentales que son los que toman decisiones a nivel mundial.

A pesar de ello, el Forex, como cualquier mercado, no esta exento de tener reacciones por noticas muy concretas (NFP, IPC, Decisiones de tipos de interés de la reserva Federal…). Hay ciertos días claves del mes que requieren de una atención mayor en determinados momentos del día.

Este servicio, avisará a los day traders a diario de las noticias que vaya a producirse a lo largo de las sesiones de operativa.
Todo trader, antes de operar se prepara la sesión y revisas las noticas para la jornada pero, un despiste en un momento de concentración máxima suele ser habitual y desastroso en muchos casos.

Para atender esta necesidad he diseñado un tipo de arquitectura que parte de un Crawler a una web de noticias llamada [investing.com](https://es.investing.com/economic-calendar/).

De esta página extraigo las noticias de la jornada y apoyandome en los servicios que ofrece Google Cloud, gestiono los datos y los modificos para poder culminar con el envío de un correo diario a los traders.


