# Interfață Analogică de Achiziție Semnale

## Descriere Proiect

Proiect realizat pentru disciplina Sisteme de Culegere și Interfațare a Analogiilor, anul III, ETTI UTCN.
Sistemul reprezintă un lanț de condiționare a semnalului, conceput pentru a prelua semnale analogice mici și a le pregăti pentru conversie numerică, oferind filtrare, amplificare programabilă și redresare de precizie.

## Arhitectura Sistemului

Proiectul este implementat ierarhic în LTspice și validat hardware cu ADALM2000. 

Etajele sunt:
1. Amplificator de Instrumentație (AI): Extracția semnalului diferențial.
2. Filtru Low-Pass KHN: Filtru biquad de ordinul 2 (Kerwin-Huelsman-Newcomb).
3. PGA (Programmable Gain Amplifier): Amplificator cu câștig controlat digital prin rezistențe în paralel.
4. Redresor de Precizie: Extragerea modulului semnalului (full-wave rectifier).

## Detalii Tehnice & Configurare

Software utilizat:

* LTspice: Pentru simulări circuital (fișierele .asc se află în folderul /Simulari).
* Scopy: Pentru vizualizarea măsurătorilor reale.

Configurare LTspice:
* Pentru a rula simularea principală, asigurați-vă că fișierele .asy (simbolurile) sunt în același folder cu schema de top.

* Modele de componente utilizate: OP482, AD820, NE5532, 2N7000.

## Structura Repository-ului

* /Simulations - Fișierele LTspice (scheme și simboluri ierarhice).
* /Docs - Raportul complet al proiectului în format PDF.

## Autor
Târnovean Andrei Gabriel Universitatea Tehnică din Cluj-Napoca 
Facultatea de Electronică, Telecomunicații și Tehnologia Informației