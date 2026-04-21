# Resumen-curso-concepto-b-sico-de-redes

# Capitulo 5
En este capitulo nos habla sobre la naturaleza de los protocolos, la función de los estándares y el papel de las organizaciones reguladoras. Encontramos los siguientes protocolos:

# 1. Protocolos de Comunicación: El Lenguaje de la Red
Al igual que en las interacciones humanas, la comunicación digital requiere de acuerdos previos para que el intercambio de información sea exitoso para eso se requiere lo siguiente:

# Identificación y Método: 
Es indispensable contar con un emisor y un receptor claramente identificados, además de acordar el medio a través del cual se enviará el mensaje (por ejemplo, cableado, señales inalámbricas o, en analogías humanas, una carta o llamada telefónica)

# Codificación y Reglas Comunes:
Se debe utilizar un idioma y gramática comunes para que el receptor pueda interpretar los datos. Esto incluye la velocidad a la que se envía la información y el momento exacto de la entrega para evitar colisiones o pérdida de datos

# Confirmación de Entrega: 
Los protocolos establecen requisitos de acuse de recibo para garantizar que el mensaje no solo llegó, sino que fue comprendido correctamente

# 2. Estándares de Internet: Garantía de Interoperabilidad
Un estándar es un conjunto de reglas que asegura que diferentes dispositivos, fabricados por distintas empresas, puedan "hablar" entre sí de manera confiable
Compatibilidad Multiplataforma: Los estándares permiten, por ejemplo, que un correo electrónico enviado desde una computadora personal sea recibido y leído perfectamente en un teléfono celular. Esto es posible porque ambos dispositivos implementan el mismo conjunto de reglas para formatear, enviar y recibir la informacion
Confiabilidad: Con la evolución constante de la tecnología y el aumento de dispositivos conectados, los estándares son los que permiten que servicios críticos, como el correo electrónico, sigan funcionando sin interrupciones a pesar de los cambios tecnológicos

# 3. Organizaciones y el Proceso de Estandarización
Los estándares no aparecen de forma espontánea; son el resultado de un ciclo riguroso de discusión, resolución de problemas y pruebas
El Proceso RFC (Request for Comments): Cuando se propone un nuevo estándar o se busca mejorar uno existente, cada etapa del proceso se registra en documentos numerados llamados RFC. Estos documentos permiten seguir la evolución técnica del protocolo desde su propuesta hasta su aprobación final
Existen organizaciones adicionales que regulan aspectos específicos, tales como:
IEEE: Enfocada en estándares de ingeniería eléctrica y electrónica.
IANA e ICANN: Relacionadas con la asignación de direcciones IP y nombres de dominio.
ITU y TIA: Enfocadas en estándares de telecomunicaciones y comunicaciones industriales

# Capitulo 6

En el capitulo 6 nos habla sobre lo tres tipos de medios utilizados en las redes modernas, y la necesidad de entender cómo cada uno de ellos codifica y transporta los datos a través del canal de comunicación que conecta un origen con un destino
Para entenderlo mejor, se detalla la composición y el funcionamiento de estos pilares según las fuentes:

# 1. Hilos metálicos (Cables de cobre)
En este tipo de medio, los datos se transmiten como impulsos eléctricos, esta el cable de Par Trenzado:
Es el tipo de cableado más común, ya que la tecnología Ethernet (base de la mayoría de las redes locales) lo utiliza para interconectar dispositivos
Para su identificación se utiliza un código de colores (cables de color sólido y cables con rayas sobre fondo blanco) para que los técnicos puedan identificar correctamente los extremos del cable

# Cable Coaxial: 
Fue uno de los primeros en utilizarse y hoy es común en sistemas de televisión y comunicaciones satelitales

# 2. Fibra Óptica (Vidrio o Plástico)
Este medio utiliza hilos de fibra de vidrio o de plástico extremadamente delgados para transmitir información

# 3. Transmisión Inalámbrica
Este pilar prescinde de los cables físicos para la conexión de dispositivos, utilizando el espectro electromagnético
Función: Permite la interconexión en redes modernas donde la movilidad es un factor clave, utilizando el aire como medio de transporte en lugar de conductores físicos

# Capitulo 7

En el capitulo 7 nos explican el proceso de encapsulación y el concepto de tramas en las redes de computadoras, se detalla cómo se estructuran y procesan los mensajes.
# 1. El Concepto de Encapsulación y Desencapsulación
La comunicación en red requiere que los datos sigan reglas de formato específicas para ser entregados y procesados correctamente
Encapsulamiento: Es el proceso de colocar un formato de mensaje (como una carta) dentro de otro formato de mensaje (como un sobre)
Desencapsulamiento: Es el proceso inverso, realizado por el destinatario, al retirar el mensaje del "sobre" para leer su contenido

# 2. La Trama (Frame) como "Sobre" Digital
Antes de enviarse a través de una red, cada mensaje de computadora se encapsula en un formato específico llamado trama
El formato exacto y el contenido de esta trama varían según el tipo de mensaje y el canal de comunicación utilizado

# 3. Anatomía Detallada de una Trama 
Una trama de red se compone de varios elementos críticos que permiten que el mensaje llegue a su destino y sea interpretado

# Identificadores de Ubicación (Direccionamiento de Red):
Dirección de destino: La ubicación física o lógica hacia donde se dirige el mensaje (ej. la dirección en el sobre)
Dirección de origen: La ubicación de quien envía el mensaje para permitir respuestas o devoluciones
# Control de Mensaje:
Indicador de inicio (Saludo): Un marcador que señala dónde comienza la información relevante del mensaje
Indicador de fin de trama: Un elemento que señala el final del mensaje (en la analogía se compara con el sello de la carta) para que el receptor sepa que la transmisión ha terminado

# 4. Importancia del Formato Correcto
El cumplimiento de estas reglas es fundamental: si un mensaje no tiene el formato correcto, no podrá ser enviado al host de destino o, si llega, el destinatario no tendrá la capacidad de procesarlo.

# Capitulo 8
En este capitulo pudimos ver la explicacion de una dirección IPv4 es una dirección de red lógica de 32 bits esencial para que un host participe en Internet y en las redes de área local (LAN)  Para permitir la comunicación, esta dirección debe ser unica dentro de la red local y, para la comunicación remota, única a nivel mundial
# Funcionamiento: 

# 1. Estructura y Notación
Aunque las direcciones IPv4 son originalmente secuencias de 32 bits binarios (difíciles de leer y configurar), se organizan de forma jerárquica para facilitar su uso:
Octetos: Los 32 bits se agrupan en cuatro bytes de 8 bits llamados octetos
Notación decimal con puntos: Cada octeto se convierte a su valor decimal y se separa por un punto. Por ejemplo, la dirección binaria 11010001.10100101.11001000.00000001 se convierte en 209.165.200.1

# 2. Composición Jerárquica: Red y Host
Una dirección IPv4 se divide en dos partes fundamentales, lo que permite un direccionamiento jerárquico
Porción de red: Identifica la red específica a la que pertenece el host. 
Porción de host: Identifica al dispositivo específico dentro de esa red
Máscara de subred: Es el componente que define dónde termina la porción de red y dónde comienza la de host. Por ejemplo, con una máscara 255.255.255.0, los primeros tres octetos representan la red y el último el host
Analogía: Este sistema es similar al telefónico, donde el código de país y de área representan la "red", y los dígitos restantes son el número local o "host"

# 3. Asignación y Comunicación
Interfaces de Red: La dirección se asigna a la tarjeta de interfaz de red (NIC) de un dispositivo
