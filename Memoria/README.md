# Seguridad en la integración continua de la metodología ágil y la filosofía DevOps
====================================================================================

## Resumen

En los últimos tiempos de las empresas dedicadas al desarrollo de software como servicio (SaaS), los conceptos de metodología ágil y la filosofía Development and Operations (DevOps) están cobrando, cada vez más, un papel fundamental para el desarrollo de las mismas. Según un estudio de alcance mundial realizado recientemente por CA Technologies, más del 75 por ciento de las organizaciones españolas coinciden en que las metodologías ágiles y DevOps son cruciales para el éxito de la transformación digital.

Este nuevo modo de entender el mundo del desarrollo de software (SW) posee una serie de elementos comunes, cada uno de ellos implementado con herramientas cada vez más conocidas y populares para las empresas que lo llevan a la práctica:

* Plataformas de desarrollo colaborativo y control de versiones de SW (por ejemplo GitHub), donde se almacena el código desarrollado por las mismas.
* Diferentes entornos o infraestructuras de trabajo para los desarrolladores, que van a permitir un desarrollo y despliegue continuo para las mejoras del producto: entornos de desarrollo, entornos de seguro de calidad o Quality Assurance (QA), preproducción, producción o entorno final, etc. 
* Fundamentos de Integración continua (IC) y Despliegue Continuo (DC).
* Desarrollo y de aplicaciones inmutables que utilizan contenedores de imágenes (generalmente de Docker) para incrementar la protabilidad, reusabilidad y escalabilidad de la aplicación. Estas aplicaciones suelen mantener sus plataformas soportadas en Proveedores Cloud tales como Amazon Web Service (AWS), Microsoft Azure o Google Cloud Engine (GCE). 

El presente Trabajo Fin de Máster (TFM) pretende exponer un proceso automatizado de análisis estático de aplicaciones en varios niveles. El resultado de la ejecución periódica de estos procedimientos genera informes de seguridad que podrán ser utilizados para prevenir amenazas durante las fases más tempranas del Ciclo de Desarrollo Seguro (CDS) del software, advirtiendo de aspectos tales como:

1. Si la aplicación creada tiene Vulnerabilidades (Common Vulnerabilities and Exposures (CVE)) en las librerías de dependencias de código utilizadas.
2. Si la imagen que se va a emplear para desplegar el contenedor de dicho SW contiene vulnerabilidades conocidas al nivel de Sistema Operativo (SO).