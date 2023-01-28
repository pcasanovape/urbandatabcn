# PRÀCTICA 2. M2.959 Visualització de dades

## Descripció
**Pràctica 2 de l'assignatura Tipologia i cicle de vida de les dades del Màster de Ciència de dades de la UOC.**

Amb aquesta segona pràctica s’ha volgut analitzar i descriure amb dades la realitat urbana de la ciutat de Barcelona des de diferents perspectives, aprofitant l’enorme varietat i riquesa de conjunts de dades disponibles a la web OpenData de l’Ajuntament. Totes aquestes dades s’han processat amb llenguatge Python per generar mapes interactius i altres tipus de visualitzacions, que ens permeten tenir una visió més ampla de com està conformada la ciutat.


## Autor
Activitat realitzada per **Pau Casanova Pedrol**.


## Introducció
S’ha enfocat l’anàlisi des de quatre punts de vista principals: la densitat, el preu de l’habitatge, la vegetació urbana i la parcel·lació. Per això, s’han creuat dades d’una selecció variada de datasets del portal de dades de l’Ajuntament.

Per la realització de la pràctica hem decidit treballar a nivell de barri com unitat administrativa de referència, analitzant les diferents mètriques pels 73 barris que conformen el municipi de Barcelona, ja que això ens permetia establir una unitat comú per poder combinar tots els conjunts de dades i alhora donar una visio ampla i prou variada de la naturalesa de les diferents parts de la ciutat.

Tots els conjunts de dades utilitzats tenen llicència Creative Commons Attribution 4.0, el que en permet el seu ús lliure i la seva difusió.

### Eines emprades
La totalitat de la pràctica ha estat realitzada amb Python, tant el preprocessament de les dades com la generació de visualitzacions. Per a la generació de mapes interactius a partir dels polígons de coordenades, s’ha treballat amb la llibreria Folium, que permet visualitzar dades geogràfiques de manera interactiva sobre un mapa base OpenStreetMap, representant les dades tant per punts com per àrees, a partir de la geometria introduïda en polígons de coordenades.
Per les visualitzacions no cartogràfiques hem utilitzat la llibreria plotly, que permet generar tota mena de gràfiques interactives, com per exemple els clàssics gràfics de barres, de pastís o de dispersió, amb una gran varietat d’opcions per adaptar-les a voluntat.
A banda d’això, tots els arxius utilitzats o generats per al desenvolupament de la pràctica estan disponibles públicament al repositori Github de la pràctica, que podeu trobar en l’enllaç que veieu en pantalla.

 
## Descripció dels fitxers
### Datasets/
* **TAULA_MAP_ILLA.csv**: – conté dades urbanístiques de parcel·lació i usos de totes les illes de Barcelona
* **/shapefiles/geom/2.json**: – conté dades geomètriques formades per polígons de coordenades de totes les unitats administratives de Barcelona, tant de barris com de districtes
* **2021_densitat.csv**: – conté dades sobre la densitat de població de Barcelona de l’any 2021
* **2022_comp_vend_preu_trim.csv**: – conté dades de preus mitjans de compravenda d’habitatges per trimestres i per barris de l’any 2022
* **2022_lloguer_preu_trim.csv**: – conté dades de preus mitjans de lloguer d’habitatge per trimestres i per barris de l’any 2022.
* **OD_Arbrat_Viari_BCN.csv**: – conté una gran varietat de dades sobre tots els arbres de viari de la ciutat de Barcelona, com coordenades, espècie, any de plantació, tipus de reg, i barri, entre d’altres.
* **OD_Arbrat_Zona_BCN.csv**: – és el mateix que el cas anterior però referit als arbres que es troben en places, parterres i espais enjardinats.
* **OD_Arbrat_Parcs_BCN.csv**: – arbrat situat en parcs urbans.

### Source/
* **PRA2-VD_pcasanovape.ipynb**: Fitxer Jupyter Notebook que conté el codi emprat per al desenvolupament de la pràctica, incloent preprocessat i generació de visualitzacions, amb comentaris.
* **PRA2-VD4_pcasanovape.html**: Fitxer HTML que conté el codi emprat per al desenvolupament de la pràctica, incloent preprocessat i generació de visualitzacions, amb comentaris.


