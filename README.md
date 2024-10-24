# MongoDB - Estructura dades
Tasca S2.03. Modelització de dades noSQL en MongoDB

En aquesta tasca elaborarem models en MongoDB a partir dels enunciats i enfocats a facilitar la visualització de les dades de les pantalles proposades.

## Nivell 1 - Exercici 1
Creem un model de dades per a una òptica que permet mostrar eficientment informació d'un client i de les seves compres d'ulleres, així com les seves característiques.
Per això, partim d'una col·lecció principal de client i relacionant la informació de compres i d'ulleres de forma incrustada.

## Nivell 1 - Exercici 2
Ara adaptem el model de dades anterior per facilitar un altre punt de vista centrat en el model d'ulleres (col·lecció) i relacionant els clients que han comprat aquest model de forma incrustada.

## Nivell 2 - Exercici 1
En aquest exercici modelem el negoci d'una botiga de menjar amb servei de recollida o de lliurament a domicili, amb la finalitat de visualitzar les dades d'una comanda d'una botiga determinada amb els seus detalls de línia, i també el client relacionat i el bloc d'informació de lliurament a domicili. Aquest darrer només s'ha de mostrar si la comanda és de tipus "entrega a domicili". La col·lecció principal és la botiga de la qual pengen l'entitat comanda, i segon nivell la informació relacionada:
- Detalls de la comanda i en cascada, la informació dels productes demanats
- Dades del client
- Informació de l'entrega a domicili si correspon

## Nivell 3 - Exercici 1
Tractem de modelar una base de dades similar a la plataforma YouTube, pensada per mostrar per pantalla informació centrada en un video determinat amb els seus atributs:
- Likes i dislikes
- Nombre de reproduccions
- Autor, del qual penja un document de playlists, amb els videos que conté.
- Tags
- Comentaris: de la pantalla s'intueix que els comentaris poden tenir rèplica, per tant introduïm un concepte de fil de conversa (thread), que agrupi tots els comentaris d'una mateixa conversa
