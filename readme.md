
# Coursive
zigbee2mqtt/0x00158d0002d7ef5b => sensor coursive


# Salle de bains
zigbee2mqtt/0x00158d0002fb495f => sensor sdb


# Grande chambre
zigbee2mqtt/0x00158d0002d7eed8 => sensor chambre


# Balcon
zigbee2mqtt/0x00158d00022887e1 => sensor balcon

# Cuisine
0x90fd9ffffe714213 => Lumière cuisine
0x90fd9ffffed6afd0 => Interrupteur cuisine


# Salon 
0x000b57fffeb9e279 => lumiére canapé
0x000b57fffec48303 => lumiére meuble télé
0x00124b0003493db5 => jieldé
0x000b57fffe2c0fd7 => Dimmer
0x00158d0001e5c360 => Xiaomi switch
0x000b57fffe39459b => lumiére piano
0x00158d0001641b31 => Double switch

# Chambre de Lison
0x0017880100e1340b => lumiére chambre de Lison
0x00178801040839c3 => interrupteur Lison
0x00158d0001fd8d82 => Sensor Lison

# Chambre d'Emma
0x00124b000338764c => lumiére chambre d'Emma
zigbee2mqtt/0x00158d0002273da9 => sensor emma

# ui Calaos Installer
1 - Liste des End devices detectés sous forme d'arbre ?

# TODO

[ ] Config d'exaempl MQTT pour test unitaires (IO de type string, analog, ..)
[ ] Passer les lights en dimmer lights
[ ] Gestion des lampes non connectées
[ ] Gestion du retour d'état des lampes
[I] Pas d'update de température tant que pas de remontée mqtt ?
[X] Pourquoi des fois humidité/pression sont présent au démarrage, des fois non ?
    * Un des sensor ne contient pas l'information pressure (dans la chambre de Lison ?)
[ ] Ajouter certaines lampes en mode RGB
[I] Utilisation d'un extern process ?
    [x] 14/12/2019 => branch /dev/nae/mqtt_ext_process 
    [x] probleme de remontée des données de stdio dans les logs. lié a la version de libuv trop récente, utiliser 1.9.2 
    [x] Probleme de remontée des données liée au subscribe => a priori correct
    
[ ] Cabler le Analong IN sur les lampes
[ ] Retour d'état sur les lampes
[x] Ajout de différents gui_style => raoul
[ ] Ajout d'un nouveau type light pour différencier light et switch => Utilisation des gui_style

## Ajout UI

[ ] Thermostat
[ ] Groupes de lampes
[ ] Eteindre toutes les lampes présent sur l'ui mobile mais pas sur l'app home ? 
    [ ] Eteindre toutes les lampes d'une piece
    [ ] Fermer tous les volets d'une piece
[ ] Affichage des pictos humidité, pression
[?] Soleil avec intensité dépendant du brightness ?
[ ] Graphes de températures
[ ] Ajout des lampes avec niveau de blanc


## Homekit

[ ] Reprendre les accessories/services en fonction du gui_style

## ZWave

[ ] Intégration de OpenZwave dans calaos ou utilisation de zwave2mqtt

## Intégration

[?] Recompilation pour calaos-os 
[?] Utilisation en local sur pc ?
[?] Intégration de zigbee2mqtt
[?] Intégration de linky

## Calaos-Installer

[ ] Ajout de toutes les IO Mqtt
[ ] Ajout d'un "Wizard" Zigbee2Mqtt avec auto discovery

## hardware

[ ] Ajout consommation compteur
[ ] Ajout consommation linky
[ ] Ajout consommation Gaz
[ ] Ajout consommation Eau

[ ] Pilotage lumiére cuisine
[ ] Pilotage lumiére bar
[ ] Pilotage tous volets roulants

## Screen

[ ] Planche en bois 260x175
[ ] cable HDMI
[ ] cable USB
[ ] Alimentation 5V/3A
[ ]

## Intégration zigbee

[X] installation zigbee2mqtt
[X] Script systemd pour démarrage zigbee2mqtt au démarrage
[X] Appairage lights
    [ ] Light Emma
[ ] Appairage sensors
[ ] Appairage buttons
