# MongoDB - Estructura dades
Tasca S2.03. Modelització de dades noSQL en MongoDB

En aquesta tasca elaborarem models en MongoDB a partir dels enunciats i enfocats a facilitar la visualització de les dades de les pantalles proposades.

## Nivell 1 - Exercici 1
Creem un model de dades per a una òptica que permet mostrar eficientment informació d'un client i de les seves compres d'ulleres, així com les seves característiques.
Per això, partim d'una col·lecció principal de client i relacionant la informació de compres i d'ulleres de forma incrustada.
En l'esquema representem també la informació del proveïdor, però no és necessària per mostrar la pantalla sol·licitada en l'enunciat.

## Nivell 1 - Exercici 2
Ara adaptem el model de dades anterior per facilitar un altre punt de vista centrat en el model d'ulleres (col·lecció) i relacionant els clients que han comprat aquest model de forma incrustada. Relacionem la informació del proveïdor directament amb les ulleres per poder mostrar-la en un clic a petició de l'usuari.
De la mateixa manera, tenim la informació del client relacionada amb cada compra per poder-la mostrar si és necessari.

## Nivell 2 - Exercici 1
En aquest exercici modelem el negoci d'una botiga de menjar amb servei de recollida o de lliurament a domicili, amb la finalitat de visualitzar les dades d'una comanda d'una botiga determinada amb els seus detalls de línia, i també el client relacionat i el bloc d'informació de lliurament a domicili. Aquest darrer només s'ha de mostrar si la comanda és de tipus "entrega a domicili". 
En aquest cas, hem optat per definir la botiga com a la col·lecció principal, ja que la pantalla mostra primer el nom d'aquesta. Però amb una altra interpretació, també podríem considerar correcte establir la comanda com a col·lecció principal, relacionant-hi la botiga.
De la botiga doncs, penja l'entitat comanda, i segon nivell la informació relacionada:
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

# Requisits tècnics

Per a dissenyar aquests models, s'ha fet servir el Moon Modeler versió 9.0.0. Es pot descarregar des del vincle https://www.datensen.com/data-modeling/moon-modeler-for-databases.html, amb una versió gratuita de prova de 14 dies.

## Instal·lació: 
1. Clonar el repositorio de Github
git clone https://github.com/g-lemoing/S2_Task3_Estructura_Dades_MongoDB.git
2. Abrir el Moon Modeler y abrir el proyecto correspondiente (.dmm)

## Contribuciones:
1. Crear un fork del repositorio: 
2. Clonar el repositorio hacia el directorio local marcado por git bash
 git clone https://github.com/YOUR-USERNAME/S2_Task3_Estructura_Dades_MongoDB.git
3. Crear una rama
git branch BRANCH-NAME
git checkout BRANCH-NAME
4. Realizar cambios o comentarios, y hacer un commit: git commit -m 'mensaje cambios'
5. Subir cambios a tu nueva rama: git push origin BRANCH-NAME
6. Hacer un pull request
