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

# Restricciones de Tecnología

## Restriccion 1

| Descripción de la Restricción                                                   | El cliente debe tener autonomia dentro del MarketPlace para decidir como quiere sus diseños, desde que fuente las desea importar y hasta con que proveedor las desea materializar. |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                                     | Gerente General                                                                                                                                                |
| Justificación para esta restricción                                                 | Agilidad y comodidad a la hora de montar una orden desde cualquier lugar.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | Se debera implementar una base de datos y modelamiento 3d o predefinido, con el fin de permitir al usuario subir sus archivos y tener una vista previa de los mismos segun la orden realizada.       |

## Restriccion 2

| Descripción de la Restricción                                                   | El cliente debe poder realizar pagos seguros en linea. |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                                     | Director de Logística                                                                                                                                                |
| Justificación para esta restricción                                                 | Agilizar procesos de entrega, reduciendo los tiempos de espera para los servicios de impresión a gran formato.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | Debe ser implementada una pasarela de pago dentro del MarketPlace para permitir a los usuarios realizar pagos con su tarjeta.       |

## Restriccion 3

| Descripción de la Restricción                                                   | El e-commerce debe contar con una aplicación complementaria. |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                                     | Director de Logística                                                                                                                                                |
| Justificación para esta restricción                                                 | Permitir a los usuarios visualizar sus impresiones en diferentes marcos.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | El usuario mediante su cuenta debe ingresar a la app movil y seleccionar aquellas ordenes que cumplan los requisitos para ser previsualizadas.       |

## Restriccion 4

| Descripción de la Restricción                                                   | Crear PhotBooks (albumes) fotográficos de manera digital y con posibilidad de impresión |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                                     | Directora de Ventas                                                                                                                                                |
| Justificación para esta restricción                                                 | Atrapar un segmento poblacional en el cual predomina el deseo de guardar y compartir recuerdos importantes de manera fisica.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | El sistema debe contar con un apartado tipo canva/PowerPoint de libre diseño, en el cual se especifique las paginas y las fotografias que iran en el PhotoBook, asi como la previsualización (versión digital). Personalización del PhotoBook, fotos, distribución, portada y tamaño para su versión fisica.       |

## Restriccion 5

| Descripción de la Restricción                                                   | El sistema debe estar interconectado con un tercero aliado para realizar entregas. |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                                     | Director de Logística                                                                                                                                                |
| Justificación para esta restricción                                                 | Agilizar procesos de entrega, reduciendo los tiempos de espera para los servicios.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | Debe ser integrado junto al sistema pricipal de FotoAlpes un servicio de un tercero como (Fedex, Servientrega, etc) que permita generar la orden de envio de manera inmediata, asi como tambien comparta su estado actual dentro del proceso de reparto.       |

## Restriccion 6

| Descripción de la Restricción                                                   | El MarketPlace debe brindar Datos estadisticos sobre las ventas. |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                                     | FotoAlpes                                                                                                                                                |
| Justificación para esta restricción                                                 | Permitir el Analisis de los datos de ventas para generar acciones que las potencien.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | Se deben alamcenar las peticiones del servidor, número de ventas confirmadas y entregadas y deben ser mostradas exclusivamente a quien corresponden.       |

## Restriccion 7

| Descripción de la Restricción                                                   | Realizar el desarrollo en Python. |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                                     | Director de Tecnología                                                                                                                                              |
| Justificación para esta restricción                                                 | El Equipo de desarrollo conoce este lenguaje.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | El desarrollo del proyecto se vera limitado en algunos aspectos, aunque se vera potenciado en temas de analitica.       |
## Restriccion 8

| Descripción de la Restricción                                                   | Realizar el desarrollo en Python. |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                                     | Director de Tecnología                                                                                                                                              |
| Justificación para esta restricción                                                 | El Equipo de desarrollo conoce este lenguaje.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | El desarrollo del proyecto se vera limitado en algunos aspectos, aunque se vera potenciado en temas de analitica ppor las librerias de Python.       |

## Restriccion 9

| Descripción de la Restricción                                                   | Número de confirmación de la orden |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                                     | FotoAlpes                                                                                                                                                |
| Justificación para esta restricción                                                 | Dar seguridad al cliente a la hora de ordenar en linea, además de servir con identificador unico para hacer el seguimiento de su pedido.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | El número del pedido debe ser mostrado en pantalla y enviado via e-mail, por ende se debe integrar una api que permita el envio automatico de estos email a los usuarios.       |

## Restriccion 10

| Descripción de la Restricción                                                   | El sistema debe permitir autoescalamiento de sus servicios para procesar un numero mayor de consultas. |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                                     | FotoAlpes                                                                                                                                                |
| Justificación para esta restricción                                                 | Evitar colapsos del sistema y sus servicios.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | El sistema debe ser alojado en un servicio como Azure, AWS o Google Cloud, el cual permita el autoescalamiento de los recursos y posteriormente su retrocesos a los valores predefinidos si es el caso.       |

## Restriccion 11

| Descripción de la Restricción                                                   | Implementación de IA. |
|----------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Usuario que expresa esta restricción                                                     | FotoAlpes                                                                                                                                               |
| Justificación para esta restricción                                                 | Agilizar procesos internos de logistica, asi como procesos de creación para los usuarios.                                                             |
| Cómo considera que pueda afectar la arquitectura del sistema esta restricción | Usando un microservicio de IA el cual permita ser flexible ante las solicitudes del cliente, la mision principal de la IA es diseñar PhotBooks apartir de las fots del cliente y seguir sus instrucciones (Número de hojas, tamaño, fotos por hoja, etc) o en el caso de la IA del lado del sistema, agilizar y predefinir rutas rapidas para agilizar las entregas de los productos.       |

