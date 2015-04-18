# Documentación Senior OS

Los teléfonos móviles actuales son demasiado complicados para ser utilizados por algunas personas mayores. Senior OS es un **sistema operativo móvil basado en Firefox OS accesible para nuestros mayores**. Senior OS puede ser gestionado íntegramente por un tercero de forma remota, e integra utilidades como conocer la localización de la persona o un sistema de alertas y recordatorios.

## Arquitectura

* **Sistema operativo móvil**: basado en Firefox OS pero simplificado con el doble fin de alargar la vida de la batería y simplificar su uso (eliminando toda posibilidad de configuración).

* **Portal de gestión + API**: es el portal a través del cual se gestiona de forma remota el dispositivo. Es "responsive" para que se pueda utilizar desde móviles, navegadores de escritorio o tablets.

* **Servidor de notificaciones Push**: envía notificaciones al teléfono sin necesidad de mantener una conexión móvil-servidor establecida, así se alarga la vida de la batería a varios días.

## Tecnologías utilizadas

La solución está desarrollada utilizando software libre.

* Servidor de notificaciones Push: https://github.com/telefonicaid/notification_server (GNU AGPLv3) utiliza nodejs, mongodb y rabbitmq.

* Portal de gestión + API: https://github.com/senioros/senior utiliza Twitter Bootstrap (frontend), nodejs+express+mongodb (backend).

* Sistema operativo móvil basado en Firefox OS: https://github.com/mozilla-b2g, https://github.com/mozilla-b2g/gaia (Apache 2).

## Recursos

* [Presentación HackForGood 2015](http://slides.com/guidogarcia/senior-os-hackforgood)
* [Video promocional HackForGood 2015](https://vimeo.com/125320155) (50 seg)
* [Video demo HackForGood 2015](https://vimeo.com/125320156) (2 min)
