## Raspberry Pi Wiegand Reader

### Descripción
Codigo para la lectura de tags/tarjetas RFID mediante una lectora de RFID conectada a una Raspberry Pi con Pigpio.

### Requisitos 
* Python 2.7
* [Pigpio](http://abyz.me.uk/rpi/pigpio/download.html)

### Instalación de Pigpio
    $ sudo apt-get update
    $ sudo apt-get install pigpio python-pigpio python3-pigpio


### Instrucciones de uso 

    $ sudo pigpiod
    $ git clone https://github.com/alxsmora1/rasberrypi_wiegand.git
    $ cd raspberrypi_wiegand
    $ python wiegand.py


### Metodo de conexión 
* GPIO (BCM)
* Se necesita conectar el cable verde (D0) en el GPIO 14 y el cable blanco (D1) en el GPIO 15.
* Tambien es requerido conectar la tierra (GND) de la lectora a la Raspberry en un pin GND, de lo contrario esto genera que haya ruido durante la lectura y los datos no puedan ser interpretados correcatmente.   