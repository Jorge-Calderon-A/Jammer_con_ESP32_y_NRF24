# Jammer con ESP32 y módulos NRF24

En este contexto se aplica un blqueador de señales, lo que hace este dispositivo es emitir señales que sean similares a la que un receptor recibe, de tal manera que este se confuna y no logre distinguir cual es la correcta.

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



