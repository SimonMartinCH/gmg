////////////////////////////
LICENSE
///////

La version pour QuantumGIS de la légende pour la cartographie géomorphologie a été réalisée par Simon Martin, du bureau d'étude Relief, sur la base de la brochure éditée par l'Institut de Géographie et Durabilité de l'Université de Lausanne (voir https://www.unil.ch/igd/fr/home/menuinst/la-recherche/eau-et-geopatrimoine/axes-de-recherche/la-legende-geomorphologique-de-lunil.html).

La dernière version est disponible sur https://github.com/SimonMartinCH/gmg/workshop1/ressources/

The QuantumGIS key for geomorphological mapping is under licence CC BY-SA Simon Martin [bureau d'étude Relief]
(https://creativecommons.org/licenses/by-sa/3.0/deed.fr)

////////////////////////////
METADATA
////////

>>QGIS Layer Style files<<
geom_pnt.qml
geom_lin.qml
geom_pol.qml
Store symbology rules and symbols. Rules are based on our data structure (see below: Shapefiles), but can be of course modified ton match your own needs.
If stored in the same folder and with the same name as the shapefiles, styles should apply automatically.

>>Shapefiles<<
geom_pnt (punctual features)
geom_lin (linear features)
geom_pol (areal features)

The 3 shapefiles share the same data structure:

>PROCESS
Get the list of values from resources/process.csv.
Process value is only used in symbology rules when form value is redundant.

>FORM
Get the list of values from resources/forme_lin.csv and /forme_pol.csv
or load the QGIS Layer Style files.

>ANGLE
Angle value is used by some symbologies: symbol orientation for areal or punctual features.



>>resources<<
.CSV style store the key texts in UTF-8 (to be restored in Propriétés de la couche / Formulaire d'attribut)
GM_key_colors.gpl store the specific colors - one for each process (to be restored in Projet / Propriétés du projet / Style par défaut / Couleurs du projet)
!!-outdated-!! GM_key_symbols.xml store the whole symbology (to be restored in Projet / Propriétés du projet / Style par défaut)
workspace.qgs is an empty project file with the 3 layers and defaults styles and colors loaded
