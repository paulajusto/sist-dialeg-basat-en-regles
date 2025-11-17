# Sistema de Diàleg Basat en Regles per a la Recomanació d'Habitatges

Aquest projecte implementa un sistema de diàleg basat en regles capaç de recollir preferències de l’usuari, validar-les i generar recomanacions d’habitatges a partir d’un conjunt de dades. El sistema simula el comportament d’un assessor immobiliari, oferint una interacció natural, flexible i tolerant a errors.

## Característiques principals

* Diàleg progressiu amb l’usuari per recollir preferències.
* Possibilitat de sortir del sistema amb *quit* o saltar preguntes amb *any*.
* Validació de respostes, incloent rangs, formats i gestió d’errors.
* Tolerància a variacions d’escriptura mitjançant coincidència aproximada.
* Filtres avançats: lloguer/compra, ingressos, planta mínima, terrassa, ascensor, ús comercial.
* Recomanacions flexibles: mostra opcions que compleixen estrictament les preferències i també alternatives properes.
* Missatges humanitzats que fan la interacció més natural.
* Verificació final de totes les respostes abans de generar recomanacions.

## Funcionament

El sistema guia l’usuari a través d’un conjunt de preguntes relacionades amb la cerca d’habitatges: pressupost, ubicació, habitacions, banys, metres quadrats i característiques addicionals.

A partir de les respostes, el programa:

1. Normalitza i valida les dades introduïdes.
2. Aplica filtres bàsics i avançats segons les preferències.
3. Troba habitatges compatibles.
4. Mostra recomanacions estrictes i alternatives que poden aportar més valor.
5. Finalitza amb un missatge de comiat.

## Millores implementades

### Millora 1: Humanització del diàleg

Frases personalitzades per salutacions, errors, transicions i confirmacions.

### Millora 2: Tolerància i flexibilitat

* Coincidència aproximada per a ubicacions.
* Recordatori del límit del 35% en lloguer.

### Millora 3: Recomanacions flexibles

Mostra habitatges que, tot i no complir exactament els criteris, ofereixen millores rellevants (més m², més habitacions, millor preu).

## Requisits

* Python 3.10+
* Llibreries estàndard (`json`, `time`, etc.)

## Execució

1. Clona el repositori:

   ```
   git clone <url-del-repositori>
   ```
2. Accedeix a la carpeta del projecte:

   ```
   cd projecte
   ```
3. Executa el sistema:

   ```
   python main.py
   ```

## Exemple d'ús

El sistema inicia amb un missatge de benvinguda i guia l’usuari per totes les preguntes. Al final, valida totes les respostes i presenta les recomanacions disponibles.

## Autores

Paula Justo
Júlia Pedrol

Grau en Intel·ligència Artificial — FIB (UPC)
