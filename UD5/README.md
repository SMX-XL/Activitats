# UD3. Elements de la xarxa local

## Presentació de l'activitat

Hola a tots i totes! Us heu trobat mai amb una xarxa informàtica que sembla un plat d'espaguis? Cables de tots els colors penjant per la paret, rosetes despenjades, servidors apilats a sobre d'una taula i ningú sap quin cable va a quin ordinador... Quin desastre, oi? Quan falla una connexió en una xarxa així, trobar l'avaria pot convertir-se en un autèntic malson i fer perdre hores de feina a una empresa.

Per evitar aquest caos, els tècnics i tècniques en Sistemes Microinformàtics i Xarxes (SMX) utilitzem el cablatge estructurat: un mètode organitzat, normalitzat i professional per dissenyar i desplegar la infraestructura física d'una xarxa local.

En aquesta pràctica us posareu la llanterna al cap, agafareu la crimpadora i el provador de cables, i actuareu com a equip de tècnics encarregats d'equipar una nova oficina corporativa (TechNova). Aprendreu a dissenyar el rack de comunicacions, muntar cables de xarxa amb el codi de colors oficial T568B, instal·lar preses de paret (keystones), etiquetar la instal·lació seguint la norma i certificar que les connexions funcionen a la perfecció. ÉS hora de posar-hi mans a la obra!

### Durada de l'activitat

La durada prevista de l'activitat és 4 hores a classe.

### Objectius específics de l'activitat

- Dimensionar i organitzar els equips d'un armari de comunicacions (Rack de 19") calculant la seva alçada en unitats de rack (U) i respectant la reserva d'espai del 30% per a futures ampliacions.
- Connectoritzar de forma precisa un cable de xarxa directe UTP Cat 6 amb connectors RJ-45 mascle aplicant l'estàndard de colors T568B.
- Muntar una presa de xarxa femella d'usuari (keystone RJ-45) i la seva connexió corresponent al panell de connexions (patch panel).
- Validar la continuïtat i el correcte patillatge de la instal·lació utilitzant un tester o mesurador de cablejat.
- Diagnosticar i resoldre avaries físiques habituals en les línies de comunicació.

### Competències treballades

d) Replantejar el cablejat i l’electrònica de xarxes locals en petits entorns i la seva connexió amb xarxes d’àrea extensa, canalitzant a un nivell superior els supòsits que així ho requereixin.

e) Instal·lar i configurar xarxes locals cablejades, sense fil o mixtes, i la seva connexió a xarxes públiques, assegurant-ne el funcionament en condicions de qualitat i seguretat.

g) Realitzar les proves funcionals en sistemes microinformàtics i xarxes locals, localitzant i diagnosticant disfuncions, per comprovar i ajustar el seu funcionament.

### Resultats d'aprenentatge i criteris d'avaluació

RA2. Desplega el cablejat d'una xarxa local interpretant-ne especificacions i aplicant-hi tècniques de muntatge.

- Reconeix els principis funcionals de les xarxes locals.
- Diferencia els mitjans de transmissió.
- Reconeix els detalls del cablejat de la instal·lació i el seu desplegament (categoria del cablejat, espais pels quals discorre, suport per a les canalitzacions, entre altres).
- Munta els armaris de comunicacions i els seus accessoris.
- Munta i estableix connexió les preses d'usuari i panells de connexions.
- Prova les línies de comunicació entre les preses d'usuari i panells de connexions.
- Etiqueta els cables i preses d'usuari.
- Treballa amb la qualitat i seguretat requerides.

RA3. Interconnecta equips en xarxes locals cablejades descrivint estàndards de cablejat i aplicant tècniques de muntatge de connectors.

- Interpreta el pla de muntatge lògic de la xarxa.
- Munta connectors sobre cables (coure i fibra) de xarxa.
- Munta els equips de commutació en els armaris de comunicacions.
- Connecta els equips de commutació als panells de connexions.
- Verifica la connectivitat de la instal·lació.
- Treballa amb la qualitat requerida.

### Continguts

- Cablatge estructurat: concepte, objectius, subsistemes (horitzontal i vertical) i normatives d'aplicació (ISO/IEC 11801, EN 50173, ANSI/TIA-568).
- Categories i classes de cablejat: parell trenat UTP/FTP Cat 6 / Cat 6A, velocitats i amplada de banda.
- Armaris i repartidors de comunicacions: Racks de 19", unitats de rack (U), panells de patch (patch panels), guies de cablejat i sais.
- Elements d'interconnexió i preses: connectors RJ-45 mascle, preses femella (keystones autocrimpables o punch-down), rosetes de paret.
- Tècniques de muntatge: pelat de cable, ordenació segons estàndard T568B, grimpat amb crimpadora i fixació de keystones.
- Comprovació i verificació: ús del provador/tester de cablejat RJ-45, identificació de parells enllaçats, oberts, encurtcircuits o creuats.

### Capacitats clau treballades

- Autonomia
- Organització del treball
- Treball en equip
- Innovació
- Resolució de problemes
- Responsabilitat

### Semàfor ús de la IA

🟠 Aquesta activitat permet un ús parcial o restringit.

Permès: Com a eina de suport per consultar conceptes teòrics (diferències entre categories Cat 6/6A, significat dels paràmetres de certificació), revisar la codificació de colors T568B o demanar consell per redactar les conclusions de la memòria.

**Condicions**: Cal processar, entendre i validar sempre els resultats rebuts. Està totalment prohibit copiar l'enunciat d'un exercici directament al xat de la IA i enganxar la resposta generada per al lliurament final sense treball propi ni anàlisi crítica.

Aquesta activitat inclou un punt d'ús obligatori de la IA per generar un esquema del Rack de Comunicacions.

## Enunciat de l'activitat

L'empresa de serveis digitals TechNova està reformant la seva seu i us ha encarregat el desplegament del cablatge estructurat de la seva nova oficina a la Planta 1. La instal·lació ha de donar servei a 12 punts de treball d'alta velocitat (Gigabit Ethernet) i ha de complir estrictament la normativa vigent.

Realitzareu el treball en divereses fases, algunes individuals i d'altres que haureu de fer en grup.

- **Fase 1**: Dimensionament i disseny del Rack (individual).

    A la sala tècnica de la Planta 1 cal instal·lar un armari repartidor (Rack de 19") que albergarà l'electrònica i els panells de connexió per als 12 punts de treball existents, amb una previsió de creixement futur.

    1. Calcula l'espai necessari en Unitats de Rack (U), sabent que els equips que cal instal·lar inicialment són:

       - 1 Switch de xarxa de 24 ports (1U).
       - 1 Router de xarxa (1U).
       - 1 Panell de patch (Patch Panel) de 24 ports RJ-45 (1U).
       - 1 Guia/passacables horitzontal amb tapa (1U).
       - 1 Panell de distribució d'alimentació / regleta de saix (PDU) (1U).
       - 1 Sistema d'Alimentació Ininterrompuda (SAI) en format rack (2U).

    2. Aplica la reserva del 30% per a futurs creixements:

       - Suma les Unitats de Rack (U) totals ocupades pels equips inicials.
       - Aplica el coeficient del 30% d'espai lliure de reserva ($U_{\text{mínimes}} = U_{\text{actuals}} / 0,7$).

    3. Dibuixa usant un programa de disseny (per exemple Visio) l'esquema del Rack de Comunicacions amb els equips inicials i l'espai reservat per a futurs creixements.

    4. Pots provar a demanar que l'IA et dibuixi l'esquema. Pensa que li hauràs dir clarament el que cal incloure i en quin ordre. Inclou el prompte que has fet servir per generar el dibuix amb l'IA. Comenta quin dels dos dissenys està més ben resolt i per què.

- **Fase 2**: Pressupost de la instal·lació (individual).

   Cal elaborar un pressupost detallat de la instal·lació del cablatge estructurat, tenint en compte els següents elements:

  - 12 preses de paret RJ-45 Cat 6 (keystones).
  - 12 metres de cable UTP Cat 6 per a cada presa (valor mitjà).
  - 1 Panell de patch (Patch Panel) de 24 ports RJ-45.
  - 1 Switch de xarxa de 16 o 24 ports no gestionable.
  - 1 Guia/passacables horitzontal amb tapa.
  - 1 Panell de distribució d'alimentació.
  - 12 tirants de xarxa (patchcords) de 1,5 metres de longitud per connectar els ordinadors.
  - 12 tirants de xarxa (patchcords) de 1 metre de longitud per unir els panells de connexió amb el switch.
  - 1 Rack de 19" de la mida calculada a la Fase 1.

En aquest pressupost no cal incloure el cost de la mà d'obra, ni del router ni tampoc del SAI, ja que aquests equips ja estan disponibles a l'empresa.

Indiqueu clarament la denominació de cada element, la quantitat, el preu unitari i el preu total. Finalment, calculeu el cost total de la instal·lació.

- **Fase 3**: Muntatge d'un tirant de xarxa (parelles)

En aquesta fase treballareu en parelles. Cada parella muntarà un tirant de xarxa amb connectors RJ-45 mascle aplicant l'estàndard de colors T568B. Un cop muntat, cada parella provarà la correcció del tirant amb un comprovador de cablejat.

Feu fotografies del procés de muntatge i de la prova amb el comprovador. Amb aquestes fotografies, redacteu una petita guia explicativa del procediment de muntatge i comprovació del tirant de xarxa. Aquesta guia ha de ser clara i concisa, de manera que qualsevol persona pugui seguir els passos per muntar correctament un tirant de xarxa.

### Què cal lliurar, on i com?

Memòria descriptiva que inclogui les tres fases de l'activitat, incloent els diagrames, el pressupost i la guia de muntatge del tirant de xarxa.

## Material de suport

- Material propi. [UD5. Instal·lació física de la xarxa local](smx-xl.github.io/Materials/UD5).