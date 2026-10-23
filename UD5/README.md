# UD5. Instal·lació física de la xarxa: cablatge estructurat

## Presentació de l'activitat

Hola a tots i totes! Us heu trobat mai amb una xarxa informàtica que sembla un plat d'espaguis? Cables de tots els colors penjant per la paret, rosetes despenjades, servidors apilats a sobre d'una taula i ningú sap quin cable va a quin ordinador... Quin desastre, oi? Quan falla una connexió en una xarxa així, trobar l'avaria pot convertir-se en un autèntic malson i fer perdre hores de feina a una empresa.

Per evitar aquest caos, els tècnics i tècniques en Sistemes Microinformàtics i Xarxes (SMX) utilitzem el cablatge estructurat: un mètode organitzat, normalitzat i professional per dissenyar i desplegar la infraestructura física d'una xarxa local.

En aquesta pràctica us posareu a planificar el desplegament de la xarxa. Abans de començar a tirar cables, instal·lar rosetes i muntar equips, haureu de calcular l'espai necessari per a l'armari de comunicacions (Rack), dissenyar el seu esquema.

### Durada de l'activitat

La durada prevista de l'activitat és 4 hores a classe.

### Objectius específics de l'activitat

- Representar en un mapa físic l'espai, els punts de xarxa i el recorregut del cablejat a partir d'un cas pràctic.
- Dimensionar un armari de comunicacions de 19" en unitats de rack (U), reservant com a mínim un 30% de l'espai per a ampliacions.
- Dibuixar la distribució dels equips i de l'espai de reserva dins del rack.
- Calcular i pressupostar el material passiu necessari per a la instal·lació, sense incloure l'electrònica de xarxa.

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

## Enunciat de l'activitat

L'empresa TechNova obrirà una oficina nova i us encarrega el disseny de la seva xarxa local cablejada. Heu de preparar una proposta tècnica abans que comencin les obres. Aquesta activitat és de planificació: es resol amb plànols, càlculs i eines digitals o de dibuix.

L'oficina és una sala diàfana rectangular de 12 m d'est a oest i 8 m de sud a nord, amb una porta d'accés a la paret sud. Hi haurà sis taules de treball, cadascuna amb una presa doble RJ-45 Cat 6 per donar servei a un ordinador i a un telèfon IP; en total calen 12 connexions. Heu de proposar una distribució adequada de les taules, les preses i el rack dins l'espai disponible. La ubicació dels elements no està predeterminada: decidiu-la tenint en compte l'accés a la sala, la comoditat dels llocs de treball, la seguretat i l'organització del cablejat.

Dissenyeu també el recorregut de les canaletes des del rack fins a les preses. Cada port RJ-45 tindrà un cable dedicat des del rack fins a la presa corresponent (topologia en estrella). Calculeu les longituds a partir del vostre disseny, indicant els trams i els criteris de mesura. Afegiu un marge del 15% al cable de xarxa per absorbir desviacions i reserva de servei; arrodoniu la compra a metres sencers.

### Fase 1. Mapa físic de la instal·lació

Dissenyeu una distribució adequada i dibuixeu el mapa físic de l'oficina a escala. Podeu fer-lo amb una aplicació de disseny com Visio o similars. Justifiqueu breument les decisions de distribució i incloeu al plànol:

- Les dimensions de la sala, la porta, la ubicació de les sis taules i la ubicació proposada del rack.
- Les 12 connexions de xarxa, identificades amb codis (per exemple, P01-P12) i agrupades en sis preses dobles.
- El recorregut proposat de les canaletes i dels cables, amb les distàncies de cada tram indicades.
- Una llegenda clara que diferenciï les preses, el rack i les canalitzacions.

### Fase 2. Dimensionament i esquema del rack

Al rack de 19" s'hi preveu instal·lar aquests elements:

- 1 switch de 24 ports (1U).
- 1 router (1U).
- 1 panell de connexions de 24 ports RJ-45 (1U).
- 1 guia/passacables horitzontal (1U).
- 1 panell de distribució d'alimentació (PDU) (1U).
- 1 sistema d'alimentació ininterrompuda (SAI) en format rack (2U).

Calculeu les unitats de rack ocupades i la capacitat mínima total per mantenir un 30% d'espai lliure per a ampliacions. Feu servir la fórmula $U_{\\text{mínimes}} = U_{\\text{ocupades}} / 0,7$ i trieu una mida comercial de rack igual o superior al resultat.

Dibuixeu la vista frontal del rack i indiqueu l'ordre dels elements, l'alçada en U de cadascun i les U que queden lliures. L'esquema ha de mostrar també els equips electrònics, encara que no s'hagin d'incloure al pressupost.

### Fase 3. Pressupost del material

Elaboreu un pressupost del material passiu i dels elements físics de la instal·lació. Calculeu les quantitats a partir del mapa i de l'esquema del rack. Incloeu, com a mínim:

- Cable UTP Cat 6 i canaleta per als recorreguts dibuixats, amb el marge de reserva indicat.
- 12 connectors femella RJ-45 Cat 6 (keystones) i 6 marcs o caixes dobles per a les preses.
- 1 panell de connexions de 24 ports RJ-45.
- 12 patchcords d'1 m per al rack i 12 patchcords d'1,5 m per als llocs de treball.
- 1 rack de 19" de la mida triada i 1 guia/passacables horitzontal.
- 1 PDU per al rack.

**No inclogueu l'electrònica de xarxa** (switch, router o punts d'accés), el SAI ni la mà d'obra. Per a cada material, indiqueu la descripció, la quantitat, el preu unitari, l'import i l'enllaç o la font consultada. Calculeu el subtotal, l'IVA i el total. Si algun element no té un preu verificable, indiqueu el criteri emprat per estimar-lo.

### Què cal lliurar, on i com?

Lliureu individualment una memòria en PDF que contingui:

- El mapa físic de la instal·lació, a escala i amb llegenda.
- Els càlculs del dimensionament del rack i el seu esquema frontal.
- El pressupost desglossat del material, amb fonts de preus i total amb IVA.

Tota l'activitat es pot completar sense accedir al taller ni utilitzar material físic.

## Material de suport

- Material propi. [UD5. Instal·lació física de la xarxa local](https://smx-xl.github.io/Materials/UD5).
