# Jammer con ESP32 y módulos NRF24

En este contexto se aplica un bloqueador de señales, lo que hace este dispositivo es emitir señales que sean similares a la que un receptor recibe, de tal manera que este se confuna y no logre distinguir cual es la correcta.

Este proyecto se realiza con la placa ESP32U y modulos NRF24l01, los componentes utilizados son:

- Placa ESP32U
- Modulos NRF24l01
- cable dumper macho a hembra
- 2 Protoboard
- Cable tipo C (capaz de manejar datos y carga)
- PC
- transformador (util si el pc no entrega la coriente necesaria para que funcione el ESP32)
- 2 condensadores de $10uf$, el voltaje no deberia jugar en contra, puede ser 16V o mas, bien se sabe que el voltaje de un condensador es la tensión maxima a la que se puede exponer

Se conecta el ESP32 en el protoboard, lo que se hizo fue quitar un modulo +- del protoboard para que la placa ESP32 pueda quedar en cada pin de manera correcta sin que superpongan una con otra mediante las conexiones internas del protoboard, luego se siguieron las siguientes conexiones de señales.



Para el módulo HSPI:


<img width="367" height="262" alt="image" src="https://github.com/user-attachments/assets/610392ad-50d9-41c4-9444-b9189f9f88f0" />

Para el módulo VSPI:

<img width="367" height="262" alt="image" src="https://github.com/user-attachments/assets/1135e224-19d6-4d80-a315-e4713c66dfad" />

Siguiendo las conexiones es bastante sencillo continuar, una vez instalada las antenas, se procede a flashear la placa ESP32, en la pagina [Flasher ESP32](https://esp32-bluejammerflasher.pages.dev/)

Una vez en la pagina, conectar la placa al pc e instalar los drivers especificos para que el PC pueda reconocer la placa, la pagina es [drivers ESP32U CP210x](https://www.silabs.com/software-and-tools/usb-to-uart-bridge-vcp-drivers?tab=downloads), seleccionar el driver CP210x, luego volver a la pagina del flasher y mantener el boton BOOT de la placa hasta el 10% de la carga total del programa y luego soltar, una vez listo, desconectar y probar mediante el PC o un cargador conectado a la placa para alimentar los modulos y la misma placa.


![WhatsApp Image 2026-01-24 at 22 51 25](https://github.com/user-attachments/assets/a483fbe3-cd37-414c-8fbf-ee79973cace0)
![2](https://github.com/user-attachments/assets/f6275490-d856-40a3-8b16-bac39dcff756)
![3](https://github.com/user-attachments/assets/a75c983c-5329-427e-b1e1-72c6a046ab4a)




