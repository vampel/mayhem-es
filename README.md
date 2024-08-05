## MAYHEM en español
### Tutorial basico de como usar MAYHEM en español

#
Introduccion y comparacion del por que personalmente prefiero el ESP32-CAM

Si cuentas con la Devboard original de Flipper Zero te daras cuenta que tiene wifi y bluetooth (es una ESP32-S2) y al igual que en todas puedes usar los firmwares del Wifi Marauder / Evil Portal.

![esp32](pics/FZfull.jpeg)
(por el Hype compre el Flipper Zero junto con la Wifi Devboard, el Video Game Module y las protobards)
#

Aqui la lista de ESP32 compatibles (ESP-8266 podria entrar en la lista para hacer deauther pero solo es Wifi):

- Flipper Zero WiFi Devboard
- ESP32-S2 (El mismo chip ESP32 que viene en el WiFi Devboard)
- ESP32-S2-WROVER
- ESP32-WROOM
- ESP32 Marauder Mini
- ESP32-S3
- Todas las AWOK ESP32 Boards

Nota: todos los Wifi son 2.4, si hay ESP32 con wifi 5.0(ESP32-C6) pero aun nadie saca un firmware para utilizarlo en el FZ.

#

A diferencia de los ESP32 mencionados el CAM tiene mas opciones:

- Wifi
- Bluetooth
- Camara
- Ranura SD
- Led (flash para la camara)

Por ende a alguien se le ocurrio hacer el firmware ya mencionado MAYHEM que hace mas cosas que solo deauther

![menu](pics/MAYHEMmenu.jpg)

Al abrir cualquiera de esos saldra este mensaje si no detecta rapido el ESP32-CAM:

![wESP32](pics/wESP32-CAM.jpg)

Nota: si se queda pegado toca reiniciar o quitar y volver a insertar la board

#

Que hace cada una de ellas:

- [MAYHEM] Camera: hace que en tu pantalla se vea la camara(como camara de gameboy).
  ![](pics/Mcamera.jpg)
  
- [MAYHEM] Marauder: hace lo mismo que el wifi marauder(deauther a redes Wifi).
  ![](pics/MMarauder.jpg)
  
- [MAYHEM] Morse Flash: Codigo Morse usando el Led Flash, Por default trae el ensaje SOS, ET Call Home, pero si permite escribir nuevos mensajes.
  ![](pics/MMorse.jpg)
  
- [MAYHEM] Motion Detection: Deteccion de movimiento.
  ![](pics/Mdetect.jpg)
  
- [MAYHEM] Nanny Camera: es una camara que puedes accedes a ella por IP (te da una IP fija, usuario y contraseña)
  ![](pics/MIPCamera.jpg)
- [MAYHEM] QR Code: lectos de codigos QR (este ultimo no lo eh hecho funcionar)
  ![](pics/MQR.jpg)

    Hasta aqui seria el firmware mayhem sobre el ESP32-CAM pero la Board MAYHEM que hay en el mercado (incluido la que diseñe) se llaman MAYHEM porque en teoria hacen todo, que vendria siendo la descripcion de la palabra MAYHEM.

#

En internet hay varias versiones pero los precios si se me hacen altos..

  ![MAYHEM en el mercado](pics/Mayhemsale.jpg)
(Eried 115 dlls pero tu soldas todo y la cyber-bros la ultima vez que vi estaban en 85 dlls)

aqui precios tomados el dia 04/08/2024

La Mayhem de Eryed (ya soldada y testeada):
![](pics/Meryed.jpg)

Orange Dragon(la descripcion dice solo la Board):
![](pics/Morange.jpg)
Nota: las letras en la imagen dicen: Bring your own modules = tengas tus propios modulos osea que si, es solo la board.

#

Los precios estan altos como ya mencione y si, si hay una forma economica de hacerlo.. que ocupas? 
Pues solo los modulos:

Esta fue las pruebas que hice(salgo en la pantalla Xd):
![](pics/ESP32-CAM-solo.jpg)

Aqui te dejo como debe de ir conectado el ESP32-CAM si quieres hacer pruebas tu mismo:
![](pics/ESP32wiring.png)

Aqui el nrf24l01:
![](pics/nrf24l01wiring.png)

Nota: El nrf24l01 y el CC1101 van conectados igual

#

Despues de probar que funciono opte por soldar todo en las Protoboards originales del Flipper Zero:
![](pics/mayhem1.0.jpeg)
![](pics/mayhem1.1.jpeg)

Si, en la v1.0(solo ESP32-CAM) y v1.1(ESP32-CAM y nrf24l01)  solde todo.. por eso las siguientes versiones les agregue que se pudieran quitar(modular).






 
