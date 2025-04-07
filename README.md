# FreeSamples-MicroFPGAs,Nota estan enviando muestras este 2025.
   Indicar direcciones correctas para obtener MicroFPGAs

---
# PROGRAMA EUROPEO DE INTEL PARA LA INTRODUCCIÓN DE 3 MODELOS DIFERENTES DE MICROFPGAS CYC1000 MAX1000 Y PLACA MAX10 DE CONTROL ALIMENTACIÓN:
# EUROPEAN PROGRAM INTEL:

---
# NOVEDAD DEL 2025 APARECE CALYPSO DIY:
Diseño de una minimist "llamada Calypso FPGA" con la filosofía házlo tu mismo "Do it yourself DIY".
Caractesrísticas tiene casi todos los micros de la plataforma MistFPGA:
El mantenedor de la misma es Manuel Teira:
![Manuel Teira minimist Calypso]
(https://github.com/teiram/)



Todas las características: 
Salida VGA444 mediante un conector VGA DB15 estándar
Salida AV opcional mediante un conector RCA. Tanto VGA como AV comparten pines FPGA.
Conector DB9 para joystick con hasta dos botones de disparo
Tarjeta SD
Dos conectores PS/2
Botón de encendido
Botón de reinicio
Entrada de auricular
Salida de audio I2S
Mini USB para alimentación principal
Conector AUX para extensión, que expone pines libres tanto en el Cyc1000 como en el RP2040.

Comentando la placa Calypso:
El microcontrolador RP2040 usa todo el marco de trabajo de la MiST Fpga diseño inicial previo de ZXMicojack.
![ZXMicroJack MiST Fpga rp2040](https://github.com/ZXMicroJack/mist-firmware-rp2040)

Tiene soporte USB, Teclado,Ratón y Mandos de juego USB, actualmente ampliando el número de conexiones medinate un concentrador USB exáctamente el "HS8836A USB 2.0 hub".
![Minimist Calypso Fpga USB](https://github.com/teiram/calypso-usb-addon)

Tiene soporte de sonido por i2s usando una versión de Texas Instruments capaz de sacar 32Bits estéreo y una frecuencia de .

Tiene una profundidad de color de 4 bit por componente RGB es decir 12bits, y compartido también una salida video compuesto.

Es una buena opción para quien quiera portar implementaciones de retroinformática con una profundidad de color de al menos 4096colores, que es el máximo alcanzable por la placa de Manuel Teira, la Calypso.

En cuanto a poder usar un mandod de juegos DB9 tiene que estar accesible el pin del microntrolador GPIO23 rp2040.

Aclaración en español sobre el pin usado en el conector DB9:
La placa es compatible con clones del RP2040, conocidos como YD-2040 del estudio VCC-GND. Un RP2040 oficial no funcionará correctamente debido a:
El conector SWD del RP2040 oficial tiene 3 pines en lugar de 4, por lo que no se puede aprovechar el conector SWD/UART, pero sí se puede conectar el dispositivo SWD directamente al RP2040.
El YD-2040 expone el GPIO 23 en el pin 37, a diferencia del RP2040 oficial. Desafortunadamente, el GPIO 23 se utiliza para una de las direcciones del joystick DB9, por lo que un joystick DB9 no funcionará correctamente con un RP2040 oficial.
El YD-2040 no expone el VBUS en los pines de la placa base, por lo que los dispositivos USB solo se pueden usar si son autoalimentados o están conectados a través de un concentrador USB autoalimentado. El RP2040 oficial expone VBUS y, por lo tanto, sería posible alimentar el bus sin necesidad de un concentrador alimentado. Sin embargo, dado que el diseño se basó en el YD-2040, no se prevé esta opción. Esto podría solucionarse en futuras versiones.

Actualmente los miembros de esta nueva placa miniMiST Calypso están pidiendo muestras:
## https://t.me/calypsofpga
---

![Free samples from Intel](https://github.com/AtlasFPGA/FreeSamples_MicroFPGAs/raw/main/FOTOS/European%20Program%20Micro-FPGAS.png)

---
These is the link of Arrow Europe:
https://www.arrow.com/en/family/intel-solutions-europe

   Para el proceso de petición a Intel hay que redactar un buen proyecto en la solicitud, el envío de las placas de muestras enviadas, vienen franqueadas desde Alemania y no confirman que has pasado el corte, suerte en la redacción de los proyectos que entreguéis.

   Explicamos un poco en Español las 3 placas, que ofrece este programa Europeo de Intel:

   Numeramos según la posición en la fotografía:

1. MAX1000 -> 8Kles y 8Mbytes integrados, 2 cores se pueden almacenar en su interior, 31 pines libres, Nota importante tiene Conversores Analógicos a digital.
2. CYC1000 -> 25Kles, y 8MBytes de ram a 166Mhz la cual puede alcanzar 233Mhz. 31 Señales,2Mbytes spi, acelerómetro, más dos pull programables en K1 y L1.
3. MAX10    -> para gestión de control de alimentación de circuitos.

La mayoría de los cores estan portados a la CYC1000 por ser más prioritaria la cantidad de Kles que lleva la CYC1000 -> 25Kles.

# PETICIÓN TRADICIONAL DE MUESTRAS EN UTMEL PARA LA PLACA CYC1000:
# FREE SAMPLES AT UTMEL:
   Os comunicamos que la empresa UTMEL ha habilitado otra forma de pedir muestras gratuitas, es una peticion de muestras más tradicional, En el formulario se pueden pedir unidades de muestra de CYC1000: 

https://www.utmel.com/productdetail/trenzelectronic-cyc1000-31981466?gclid=EAIaIQobChMIv9Gv472L_wIVTvN3Ch20fwNuEAMYASAAEgKpy_D_BwE

![CYC1000](http://www.forofpga.es/download/file.php?id=761)

# LA CARTA ENVIADA SI LA SOLICITUD SUPERA EL CORTE DEL DESARROLLO PROPUESTO:
# THE SENDED CARD WITH CYC1000 IF A RESOLUTION IS A POSITIVE:

![Carta afirmativa muestras gratuitas de intel](https://github.com/AtlasFPGA/FreeSamples_MicroFPGAs/blob/main/FOTOS/Carta_franqueada_desde_alemania_trenz_arrow_intel_european_program_IMG_20230208_195306.jpg)

# PODÉIS VER COMO LA ANALIZÓ TRASTERLABS MIRANDO ESQUEMA Y DOCUMENTACIÓN:
# YOU CAN SEE A FUNNY DESCRIPTION OF CYC1000 IN TRASTERLABS :

   En él nos analizan que un componente relacionado con la conversión de tensiones, encargado de alimentar la placa; esta en fase-out... o en roman paladino, se dejó de producir.

[![TRASTERLABS CON CYC1000](https://img.youtube.com/vi/0bHM3NtVle0/0.jpg)](https://www.youtube.com/watch?v=0bHM3NtVle0)

