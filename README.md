<div align="justify" style="margin-right:25px;margin-left:25px">

# SYL_Labo4

## Machine d'état

### Analyse des entrées

Le circuit original comprend les entrées `ready_i`, `color_i`, `clk_i` et `reset_i`.
- `ready_i` : Arrive seulement lorsque le bras est en position initiale pour dire qu'il peut procéder au scan d'une boîte. 
- `color_i` : Arrive une fois qu'un scan a été effectué et défini la couleur de la boîte.
  - 00 : Couleur indéterminé
  - 01 : Rouge
  - 10 : Bleu
  - 11 : Erreur
- `clk_i` : Horloge
- `reset_i` : Reset asynchrone de tout le système.

Ces entrées à elles seules ne nous permettent pas de faire tous les changements d'états de la façon demandée. Pour ça il nous faudra une entrée supplémentaire `compteur_done` qui servira à nous dire si le bras à fini de se déplacer car celui-ci prend 3 coups d'horloge pour se déplacer.
Cette entrée fonctionne en utilisant un décompteur qui renvoi `1` quand il arrive à `0`.

### Analyse des sorties

### Graphe des états

### Table des états

### Création des équations