# Projecte DJ_B_PARABRISAS

>**Autors:Héctor Rodriguez y MariPaz Carreño
>**Versió: V1

----------

## Objectiu

>Crear un pcb para un limpia parabrisas, la cual tendrá control a través de un microcontrolador.
EL objetivo principal es  mantener  la luna del cristal limpia, para ello tenemos un sensor de lluvia que detectará la lluvia, un calefactor para que no se empañe, y bombas de agua que permitan en todo momento limpiar la luna.


## Diagrama de blocs
![Diagrama de bloques](Diagrama%20de%20bloques%20VF.png)



### Descripció/funcionalitat de cada bloc

  *

-----------

## Requisits / Especificacions

  * Alimentació; 12V, regulada 5V
  * Microcontrolador PIC24HJ32GP302
  * ...

-----------

## Components

| Descripció | Ref | Package | Datasheet | Proveïdor | Preu | Unitats |
|---|---|---|---|---|---|---|
| Microcontrolador | PIC24HJ32GP502 | SOIC-28W | https://ww1.microchip.com/downloads/en/DeviceDoc/70293G.pdf | Mouser | ~3€ | 1x |
| Regulador buck | LM2596S-5 | TO-263-5 | https://www.ti.com/lit/ds/symlink/lm2596.pdf | Mouser | ~2€ | 1x |
| Regulador LDO | LM1117-3.3 | TO-252 | https://www.ti.com/lit/ds/symlink/lm1117.pdf | Mouser | ~0.5€ | 1x |
| Driver motor | DRV8871DDA | HTSSOP-8 | https://www.ti.com/lit/ds/symlink/drv8871.pdf | Mouser | ~2€ | 2x |
| Transceptor CAN | TJA1049TK-3 | HVSON-8 | https://www.nxp.com/docs/en/data-sheet/TJA1049.pdf | Mouser | ~1.5€ | 1x |
| Transceptor UART | MAX232 | SOIC-16 | https://www.ti.com/lit/ds/symlink/max232.pdf | Mouser | ~1€ | 1x |
| Sensor humedad/temp | HDC2080 | WSON-6 | https://www.ti.com/lit/ds/symlink/hdc2080.pdf | Mouser | ~2€ | 1x |
| Level shifter | SN74LVC2T45 | VSSOP-8 | https://www.ti.com/lit/ds/symlink/sn74lvc2t45.pdf | Mouser | ~0.8€ | 1x |
| Relé SPST | Fujitsu FTR-LYAA005x | THT | https://www.fujitsu.com/sg/imagesgig5/ftr-ly.pdf | Mouser | ~2€ | 1x |
| Relé DPDT | Omron G6K-2P | THT | https://omronfs.omron.com/en_US/ecb/products/pdf/en-g6k.pdf | Mouser | ~3€ | 1x |
| Transistor NPN | MMBT3904 | SOT-23 | https://www.onsemi.com/pdf/datasheet/mmbt3904-d.pdf | Mouser | ~0.1€ | 2x |
| Diodo TVS | SM6T24A | SMB | https://www.st.com/resource/en/datasheet/sm6t.pdf | Mouser | ~0.5€ | 1x |
| Diodo señal | Genérico | 0603 | — | Mouser | ~0.05€ | varios |
| LED verde | LED | 0805 | — | Mouser | ~0.1€ | 1x |
| Inductor | 33uH | 0603 | — | Mouser | ~0.3€ | 1x |
| Cristal | Crystal HC49-SD | THT/SMD | — | Mouser | ~0.5€ | 1x |
| Conector alimentación | Bornera 2 pin | P5.00mm | — | Mouser | ~0.3€ | 1x |
| Conector motor | Bornera 2 pin | P5.00mm | — | Mouser | ~0.3€ | 4x |
| Conector DE9 | DB9 macho | THT | — | Mouser | ~1€ | 2x |
| Header ICSP | PinHeader 1x05 | 2.54mm | — | Mouser | ~0.2€ | 1x |
| Jumper | PinHeader 1x03 | 2.54mm | — | Mouser | ~0.2€ | 1x |
| Final de carrera | XKB DM1-16UC-1 | THT | — | Mouser | ~0.5€ | 2x |
| Pulsador SMD | Push button | SMD | — | Mouser | ~0.2€ | 2x |
| Pulsador THT | Omron B3FS | THT | https://omronfs.omron.com/en_US/ecb/products/pdf/en-b3fs.pdf | Mouser | ~0.5€ | 1x |
| Resistencias | 0603 varias | 0603 | — | Mouser | ~0.01€ | varias |
| Condensadores | 0805 varias | 0805 | — | Mouser | ~0.05€ | varias |



-----------

## Software

### Eines:

  * KiCad 9.0 o superior
  * 

### Configuraci&#243; :

  * 

### Funcionalitats:

  * 

-----------


## Historial de canvis

| Data | Autor     | Branch | Versi&#243; | Descripci&#243; |
| --- | --- | --- | --- | --- |
|  28/03/2023 | mlopez | Master | initial commit | Primera versi&#243; d'esquem&#224;tic i selecci&#243; de components |
