# Projecte DJ_B_PARABRISAS

>**Autors:Héctor Rodriguez y MariPaz Carreño
>**Versió: VFinal

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

* Alimentació: 12V d’entrada, regulada a 5V i 3.3V
* Microcontrolador: PIC24HJ64GP504
* Regulador buck: LM2596S-5 per obtenir 5V
* Regulador LDO: LM1117DT-3.3 per obtenir 3.3V
* Protecció d’entrada: díode TVS SM6T24A
* Díodes de protecció: D4, D5 i D6 per protegir contra pics inductius
* Comunicació CAN: transceptor TJA1049TK-3
* Comunicació RS232: MAX232
* Oscil·lador: cristall Y1 
* Condensadors de desacoblament: 100nF i 1uF
* Condensadors de filtratge: 680uF, 220uF, 100uF i 10uF
* Resistències: valors diversos per polarització, pull-up, pull-down i limitació de corrent
* Punts de test: TP1, TP2 i TP3

-----------

## Components

| Descripció | Ref | Package | Datasheet | Proveïdor | Preu | Unitats |
|---|---|---|---|---|---|---|
| Capacitor 100nF | C1,C2,C10,C16 | 0805 | ~ | Mouser | — | 4 |
| Capacitor 20pF | C3,C4 | 0805 | ~ | Mouser | — | 2 |
| Capacitor 1uF | C5,C6,C7,C8,C9 | 0805 | ~ | Mouser | — | 5 |
| Capacitor 680uF | C11 | 0805 | ~ | Mouser | — | 1 |
| Capacitor 220uF | C12 | 0805 | ~ | Mouser | — | 1 |
| Capacitor 10uF | C13,C14 | CP Radial D5.0mm P2.50mm | — | Mouser | — | 2 |
| Capacitor 100uF | C15 | CP Radial D5.0mm P2.50mm | — | Mouser | — | 1 |
| Capacitor 10pF | C17 | 0805 | ~ | Mouser | — | 1 |
| Capacitor 100pF | C19 | 0805 | ~ | Mouser | — | 1 |
| LED | D2 | LED 0805 | ~ | Mouser | — | 1 |
| Diodo TVS SM6T24A | D3 | SMB | https://www.st.com/resource/en/datasheet/sm6t.pdf | Mouser | — | 1 |
| Diodo genérico | D4,D5,D6 | 0201 | ~ | Mouser | — | 3 |
| Ferrita | FB1 | LairdTech 28C0236-0JW-10 | ~ | Mouser | — | 1 |
| Final de carrera SPDT | FINALCARRERA1,FINALCARRERA2 | XKB DM1-16UC-1 | ~ | Mouser | — | 2 |
| Conector 1x05 | J1 | PinHeader 1x05 2.54mm | ~ | Mouser | — | 1 |
| Conector DE9 | J2,J3 | DSUB-9 Horizontal | ~ | Mouser | — | 2 |
| Conector 1x02 | J4 | PinHeader 1x02 2.54mm | ~ | Mouser | — | 1 |
| Jumper 3 pines | JP1 | PinHeader 1x03 2.54mm | ~ | Mouser | — | 1 |
| Relé SPST-NO Fujitsu FTR-LYAA005x | K2,K3,K4 | Relay THT Vertical | https://www.fujitsu.com/sg/imagesgig5/ftr-ly.pdf | Mouser | — | 3 |
| Inductor 33uH | L1 | 0603 | ~ | Mouser | — | 1 |
| Motor DC / Bornera salida | M1,M2,M3,M5 | TerminalBlock 2P P5.00mm | ~ | Mouser | — | 4 |
| Transistor NPN MMBT3904 | Q2,Q3,Q4 | SOT-23 | https://www.onsemi.com/pdf/datasheet/pzt3904-d.pdf | Mouser | — | 3 |
| Resistencia 1k | R2,R3,R7,R8 | 0603 | ~ | Mouser | — | 4 |
| Resistencia 4.7k | R4,R13,R14 | 0603 | ~ | Mouser | — | 3 |
| Resistencia 121Ω | R5 | 0603 | ~ | Mouser | — | 1 |
| Resistencia 200Ω | R6 | 0603 | ~ | Mouser | — | 1 |
| Resistencia 10k | R9 | 0603 | ~ | Mouser | — | 1 |
| Resistencia 4.7k | R10 | 0603 | ~ | Mouser | — | 1 |
| Resistencia calefactor | R11 | 2512 | ~ | Mouser | — | 1 |
| Resistencia 60Ω | R12,R17 | 0201 | ~ | Mouser | — | 2 |
| Resistencia 10k | R15,R16 | 0603 | ~ | Mouser | — | 2 |
| Resistencia 7.6k | R18,R22,R23 | 0603 | ~ | Mouser | — | 3 |
| Resistencia 10k | R19,R20,R21 | 0201 | ~ | Mouser | — | 3 |
| Pulsador calefactor | SW1 | Alps SKRK SMD | ~ | Mouser | — | 1 |
| Pulsador bombas | SW2 | Alps SKRK SMD | ~ | Mouser | — | 1 |
| Pulsador | SW3 | Alps SKRK SMD | ~ | Mouser | — | 1 |
| Selector rotativo SP3T | SW5 | NKK NR01 THT | https://www.nkkswitches.com/pdf/NR01%20Rotaries.pdf | Mouser | — | 1 |
| Test point | TP1,TP2,TP3 | Keystone 5015 Micro Mini | ~ | Mouser | — | 3 |
| Regulador LDO 3.3V LM1117DT-3.3 | U1 | TO-252-3 | http://www.ti.com/lit/ds/symlink/lm1117.pdf | Mouser | — | 1 |
| Regulador buck 5V LM2596S-5 | U2 | TO-263-5 | http://www.ti.com/lit/ds/symlink/lm2596.pdf | Mouser | — | 1 |
| Driver motor DRV8871DDA | U3,U7 | HTSOP-8 PowerPAD | http://www.ti.com/lit/ds/symlink/drv8871.pdf | Mouser | — | 2 |
| Microcontrolador PIC24HJ64GP504 | U4 | QFN-44 7x7mm | — | Mouser | — | 1 |
| Sensor humedad/temperatura HDC2080 | U6 | Texas S-PWSON-N6 | http://www.ti.com/lit/ds/symlink/hdc2080.pdf | Mouser | — | 1 |
| Transceptor CAN TJA1049TK-3 | U8 | HVSON-8 | https://www.nxp.com/docs/en/data-sheet/TJA1049.pdf | Mouser | — | 1 |
| Transceptor RS232 MAX232 | U9 | SOIC-16 | http://www.ti.com/lit/ds/symlink/max232.pdf | Mouser | — | 1 |
| Cristal | Y1 | SMD EuroQuartz EQ161 2Pin | ~ | Mouser | — | 1 |



-----------

## Software

### Eines:

  * KiCad 9.0 o superior
  * 

### Configuraci&#243; :

  * 

### Funcionalitats:

  Gestionar el movimiento de las escobillas, el rociado del líquido limpiador mediante dos bombas y el calentamiento del sistema mediante un calefactor.
Cuando el usuario activa el mando, la PCB recibe la señal y enciende el motor del limpiaparabrisas en el modo seleccionado. También puede activar una de las dos bombas, por ejemplo una para el parabrisas delantero y otra para el cristal trasero, enviando líquido limpiador antes o durante el movimiento de las escobillas.
Además, la PCB controla el calefactor, que sirve para calentar el líquido o la zona del sistema de lavado, evitando congelación y mejorando el funcionamiento en bajas temperaturas.


-----------


## Historial de canvis

| Data | Autor     | Branch | Versi&#243; | Descripci&#243; |
| --- | --- | --- | --- | --- |
|  28/03/2023 | mlopez | Master | initial commit | Primera versi&#243; d'esquem&#224;tic i selecci&#243; de components |
