GEO 7630 examen #1 

21 février 2023 14h00 

Salle A-4160

Chargé de cours : Clément Glogowski

Démonstratrice : Maddie Le Gall


# Micro TP FME

Vous devrez produire une couche d’index H3 qui représente la quantité de commerces vacants dans chacun des hexagones.

**INPUT **: Couches de commerces : [geojson](https://data.montreal.ca/dataset/f8582c4d-a933-4306-bb27-d883e13dd207/resource/7e736f37-c935-4028-8ffe-02e1403c1eaa/download/occupation-commerciale-2022.geojson)

**INPUT **: Couche pour créer les hexagones de remplissage : [geojson](https://data.montreal.ca/dataset/b628f1da-9dc3-4bb1-9875-1470f891afb1/resource/92cb062a-11be-4222-9ea5-867e7e64c5ff/download/limites-terrestres.geojson)

Il faudra ajouter un **vertexCreator** pour définir les coordonnées x et y (long,lat) pour la couche des commerces.

Vous devrez **filtrer **les commerces pour avoir seulement les commerces vacants

**Propriété : USAGE1**

La taille de vos hexagones doit être de résolution 9 (0.2km par segments).

**Astuces **: 54 est le nombre de commerces dans le polygone avec le plus de commerces vacants

**OUTPUT** : 

Votre WRITER devra écrire dans la base de données POSTGIS geo7630 comme ceci :

![](https://lh3.googleusercontent.com/FsUKihCYfZX7SYD-Y0XHa9js978zNkFqZJjfNyAwcvux_0xoVJXT4QK9gRl0SjP1Q8tNUmYeZnxCzJVoWsGRiQwp8b3YrqQAlUPlZQKTT7pAeDquANEzRIBz3bfmAdfH9QDuNpuhdRnbNY-Yvjm0xbk)

![](https://lh5.googleusercontent.com/H1BwZp2XawUD9Xc-FqGnKe6LrvIzGbZ7bsnhN7fZzk3CN2ZWnxv7qLhoA9XmYAKaKG45g_pb7_1Z5fuoK7dJ29nLt4hiYU4PNVCLlEm7TCD8N4FU4j5OMlMZe9KdTWpFvIENoLqa5YvQDvO4vMDC5Ms)
