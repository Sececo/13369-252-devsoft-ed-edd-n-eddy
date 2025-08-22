# Restricciones de Negocio

## Restricción 1

| Descripción de la restricción                                                 | El sistema debe garantizar la disponibilidad permanente de la plataforma de reservas y compras en línea, asegurando que los usuarios puedan acceder a sus servicios en cualquier momento, sin interrupciones significativas.                             |
|-------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                          | Gerente General de FotoAlpes.                                                                                                                                                                                                                            |
| Justificación para esta restricción                                           | El modelo de negocio de FotoAlpes depende directamente de las transacciones en línea. Cualquier tiempo de inactividad podría generar pérdida de clientes potenciales, reducción de ingresos y afectar la reputación de la empresa.                       |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | La arquitectura debe diseñarse bajo un enfoque de alta disponibilidad. Esto implica incorporar servidores redundantes, balanceo de carga, sistemas de recuperación ante fallos y monitoreo continuo para garantizar que el servicio esté siempre activo. |

## Restricción 2

| Descripción de la restricción                                                 | El sistema debe asegurar la protección integral de los datos personales y financieros de los clientes, así como la confidencialidad de las fotografías y archivos cargados en la plataforma.                                                                                                      |
|-------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                          | Departamento de TI y Gerente de Operaciones.                                                                                                                                                                                                                                                      |
| Justificación para esta restricción                                           | FotoAlpes maneja información sensible como datos de pago, fotografías privadas y credenciales de acceso, por lo que es indispensable cumplir con normativas de seguridad y protección de datos para evitar riesgos legales y garantizar la confianza del cliente.                                 |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | Se requiere implementar una arquitectura segura y robusta que contemple: cifrado de datos en tránsito y en reposo, módulos de gestión de identidades y control de accesos, servidores seguros con cortafuegos y detección de intrusiones, y auditorías para detectar comportamientos sospechosos. |

## Restricción 3

| Descripción de la restricción                                                 | El sistema debe ser altamente escalable para gestionar aumentos considerables en el tráfico y las transacciones durante temporadas de alta demanda, garantizando un rendimiento óptimo.                                                                                        |
|-------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                          | Gerente Comercial y Gerente de Marketing.                                                                                                                                                                                                                                      |
| Justificación para esta restricción                                           | Durante fechas especiales, como bodas, festividades y vacaciones, FotoAlpes experimenta un incremento significativo en solicitudes de reservas y compras. Por ello, es necesario que la plataforma pueda adaptarse a estas variaciones sin afectar la experiencia del usuario. |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | Es recomendable utilizar una arquitectura modular y flexible, basada en microservicios o contenedores, con recursos desplegados en la nube. Esto permitirá escalar horizontal y verticalmente según la demanda, optimizando el rendimiento y reduciendo riesgos de saturación. |

# Objetivos de Negocio

## Objetivo 1

| Descripción del objetivo                                                      | Crear una nueva línea de negocio denominada **Contenido Digital**, que represente el 40% del total de ventas en los próximos 2 años.                                                  |
|-------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Tiempo de cumplimiento                                                        | 2 años                                                                                                                                                                                |
| Mejora esperada al negocio                                                    | Incremento significativo en los ingresos, diversificación del portafolio y posicionamiento en el mercado digital.                                                                     |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | Se requerirá desarrollar módulos para gestión y distribución de contenido digital, almacenamiento en la nube y sistemas escalables para soportar alto volumen de tráfico y descargas. |

## Objetivo 2

| Descripción del objetivo                                                   | Desarrollar una plataforma tecnológica que permita escalar el negocio a varios comercios y proveedores, operando como un mercado electrónico que represente el 20% de las ventas en el próximo año. |
|----------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Tiempo de cumplimiento                                                     | 1 año                                                                                                                                                                                               |
| Mejora esperada al negocio                                                 | Generar nuevas oportunidades comerciales, ampliar la base de clientes y proveedores, y aumentar los ingresos por comisiones y ventas.                                                               |
| Cómo considera que pueda afectar la arquitectura del sistema este objetivo | Se deberá diseñar una arquitectura modular y escalable que soporte múltiples tiendas, integración con pasarelas de pago, alta concurrencia, y funciones de seguridad robustas.                      |

## Objetivo 3

| Descripción del objetivo                                                   | Realizar una transformación digital integral que permita dar un vuelco total a la organización, adaptando procesos internos y canales de venta hacia entornos digitales. |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Tiempo de cumplimiento                                                     | Progresivo durante 2 años                                                                                                                                                |
| Mejora esperada al negocio                                                 | Mayor competitividad, modernización tecnológica, automatización de procesos y mejor experiencia del cliente.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema este objetivo | Será necesario adoptar una arquitectura flexible basada en microservicios, integración con sistemas externos, y garantizar la interoperabilidad entre plataformas.       |
