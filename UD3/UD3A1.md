# UD3.A1. Simulador de xarxes i Ethernet

## Presentació de l'activitat

Què és Cisco Packet Tracer? Imagina que és com un "Minecraft" o un "SimCity" especialitzat en xarxes d'ordinadors. En lloc de construir ciutats o cases, aquí podràs muntar instal·lacions informàtiques senceres: des d'una petita xarxa domèstica fins a la infraestructura d'un gran edifici. El millor de tot és que és un entorn virtual totalment segur: pots connectar cables, configurar servidors i provar comandes sense por de trencar cap equip real ni deixar ningú sense connexió.

En aquesta primera sessió de laboratori faràs el teu primer "desplegament". Construiràs una xarxa local (LAN) bàsica formada per dos ordinadors connectats mitjançant un commutador (Switch). L'objectiu és que perdis la por al programari, aprenguis a moure't per la seva interfície, assignis les primeres adreces IP i comprovis que els equips es comuniquen correctament fent servir la comanda ping i el mode de simulació visual.

### Durada de l'activitat

La durada prevista de l'activitat és 2 hores a classe.

### Objectius específics de l'activitat

- Objectiu 1
- Objectiu 2
- Objectiu 3

### Competències treballades

e) Instal·lar i configurar xarxes locals cablejades, sense fil o mixtes, i la seva connexió a xarxes públiques, assegurant-ne el funcionament en condicions de qualitat i seguretat.

g) Realitzar les proves funcionals en sistemes microinformàtics i xarxes locals, localitzant i diagnosticant disfuncions, per comprovar i ajustar el seu funcionament.

### Resultats d'aprenentatge i criteris d'avaluació

0225.RA2. Desplega el cablejat d'una xarxa local interpretant-ne especificacions i aplicant-hi tècniques de muntatge

- 2.1 Reconeix els principis funcionals de les xarxes locals.
- 2.2 Identifica els diferents tipus de xarxes.
- 2.3 Diferencia els mitjans de transmissió.

### Continguts

- Desplegament del cablejat.
- Interconnexió d'equips en xarxes locals

### Capacitats clau treballades

- Autonomia
- Organització del treball
- Resolució de problemes
- Responsabilitat

### Semàfor ús de la IA

🟠 Aquesta activitat permet un ús parcial o restringit.

Permès per com a eina de suport en la millora de la redacció dels informes, cerca preliminar d'informació, estructuració d'idees o explicació de conceptes teòrics complexos.

**Condicions**: Cal processar, entendre i validar sempre els resultats rebuts. Està totalment prohibit copiar l'enunciat d'un exercici directament al xat de la IA i enganxar la resposta generada per al lliurament final sense treball propi ni anàlisi crítica.

## Enunciat de l'activitat

### Requisits previs

Usarem la versió 5.3.3 de Cisco Packet Tracer. A la Comuna, trobaràs un arxiu comprimit. Fes una còpia de l'arxiu al teu ordinador i descomprimeix-lo. Dins la carpeta `\bin\` hi trobaràs l'executable `PacketTracer.exe`. Fes doble clic per iniciar el programa.

A casa us recomanem que feu servir la mateixa versió per temes de compatibilitat. De tota manera, si vols descarregar una versió més recent per treballar a casa, fes-ho des de la pàgina oficial de l'[Acadèmia Oficial de Cisco](https://www.netacad.com/es/resources/lab-downloads?courseLang=es-XL) seguint les instruccions de registre i descàrrega.

### Introducció a Packet Tracer

Abans de començar a col·locar equips, dona una ullada ràpida a la pantalla principal. Quan obres els programa, tens una finestra amb aquest aspecte:

![Packet Tracer Interface](./img/packet-tracer.png)

Ara anem a descriure quines són les zones i icones que faràs servir constantment:

- **Àrea de treball (Logical Workspace)**: El gran espai en blanc central on aniràs arrossegant els dispositius i dibuixant el mapa de la teva xarxa.

- **Selector de dispositius** (Barra inferior): Aquí trobaràs tots els equips que pots utilitzar, agrupats per categories. Per exemple, hi ha ordinadors, commutadors, routers, punts d'accés i servidors. Fes clic a una categoria i després arrossega l'equip que vulguis a l'àrea de treball.

- **Selector de tipus de cable** (Dins de Connections) els principals que usarem aquest curs són:
  - Copper Straight-Through (Cable directe, línia negra contínua): S'utilitza per connectar dispositius de diferent tipus (per exemple, un PC a un Switch).
  - Copper Cross-Over (Cable creuat, línia negra discontínua): S'utilitza per connectar dispositius del mateix tipus (per exemple, dos PC directament, dos Switches o dos Routers).
  - Fiber (Línia vermella): S'utilitza per a connexions de fibra òptica.
  - Serial (línia vermella en zig-zag): S'utilitza per a connexions sèrie entre routers.
  - Console (línia blava): S'utilitza per a la connexió directa a un dispositiu per a configuració i gestió. Permet simular la configuració d'un switch o router tal com es fa a la a realitat a través del terminal d'un ordinador.

- **Mode Temps Real / Mode Simulació** (Cantonada inferior dreta):
  - Realtime (Temps Real): La xarxa funciona en viu, com en el món real.
  - Simulation (Simulació): El temps s'atura i pots veure pas a pas com viatgen els paquets de dades visualment.

- **Eina PDU Simple** (Icona del sobre tancat a la barra dreta): Et permet enviar un paquet de prova d'un equip a un altre directament amb el ratolí.

- **Eina PDU Complex** (Icona del sobre amb un engranatge a la barra dreta): Et permet enviar un paquet de prova d'un equip a un altre i veure tots els detalls del procés, com ara les adreces IP, les adreces MAC i el camí que segueix el paquet.

- **Eina d'eliminació** (Icona de la "X" o tecla Del): Serveix per esborrar qualsevol element o cable que hagis afegit per error.

### Activitat 1. Primer desplegament

1. Afegir els dos ordinadors i el Switch a l'àrea de treball:
    - Ves a la zona inferior esquerra i fes clic a la categoria End Devices.
    - Selecciona el Generic PC (PC-PT) i col·loca dos ordinadors (PC0 i PC1).
    - A continuació, selecciona la categoria Switches, escull el model 2960 i col·loca'l al centre entre els dos ordinadors.

2. Connectar els equips mitjançant cablejat directe:
    - Selecciona la icona del llamp (Connections) i agafa el cable Copper Straight-Through (línia negra contínua).
    - Connecta PC0 (port FastEthernet0) al Switch0 (port FastEthernet0/1).
    - Repeteix l'operació per connectar PC1 (port FastEthernet0) al Switch0 (port FastEthernet0/2).
    - Espera uns segons fins que els punts de connexió es tornin de color verd.

3. Configurar les adreces IP dels equips:
    - Fes clic sobre PC0, ves a la pestanya Desktop > IP Configuration.
    - Selecciona Static e introdueix:
        - IP Address: 192.168.1.10
        - Subnet Mask: 255.255.255.0
    - Repeteix el procés per a PC1 assignant-li la IP 192.168.1.20 i la màscara 255.255.255.0.

4. Comprovar la connectivitat en Temps Real (ping):
    - Fes clic sobre PC0 i obre la finestra Desktop > Command Prompt.
    - Escriu la comanda ping 192.168.1.20 i prem Enter.
    - Comprova que s'obtenen respostes correctament sense pèrdua de paquets (0% loss).

5. Visualitzar el viatge dels paquets en Mode Simulació:
    - Canvia al mode Simulation a la cantonada inferior dreta.
    - Selecciona l'eina del sobre tancat (Add Simple PDU), fes clic sobre PC0 (origen) i després sobre PC1 (destí).
    - Prem el botó Auto Capture / Play per veure com l'envolupant es mou a través del Switch.

### Activitat 2. Entenent protocol Ethernet


### :hammer_and_wrench: Resolució de problemes freqüents

- **Problema**: Els punts de connexió no es tornen verds després de connectar els cables.

  **Solució**: Assegura't d'haver utilitzat el cable Copper Straight-Through (línia negra contínua). Si has fet servir un cable d'un altre tipus o la interfície del PC està apagada, no hi haurà enllaç físic.

- **Problema**: Els punts de la connexió es queden en taronja durant molta estona.

  **Solució**: Revisa que les adreces IP i les màscares de subxarxa estiguin correctament configurades. També comprova que els cables estiguin ben connectats i que el Switch estigui funcionant.

### Què cal lliurar, on i com?

## Material de suport
