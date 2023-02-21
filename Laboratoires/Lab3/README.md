Intégration et visualisation de données 3D Lidar et tuiles 3D Vectorielles

Laboratoire 3

****

[**Étape 1 Importation et nettoyage des nuages de points**** ****2**](https://docs.google.com/document/d/1xF8N18qUkqfF3hZ3HDEm7ZyoHe9Dg7VxzgECAgMKZE4/edit#heading=h.ec8u3bf6aztu)

[**Étape 2 Importation des limites terrestres et découpage du nuage de points**** ****5**](https://docs.google.com/document/d/1xF8N18qUkqfF3hZ3HDEm7ZyoHe9Dg7VxzgECAgMKZE4/edit#heading=h.fvbp9sj6bfxr)

[**Étape 3 Simplification du nuage de points**** ****7**](https://docs.google.com/document/d/1xF8N18qUkqfF3hZ3HDEm7ZyoHe9Dg7VxzgECAgMKZE4/edit#heading=h.7ijt6xek4lo)

[**Étape 4 Ajout de rasters géoréférencés**** ****8**](https://docs.google.com/document/d/1xF8N18qUkqfF3hZ3HDEm7ZyoHe9Dg7VxzgECAgMKZE4/edit#heading=h.23l8rlxg5p8f)

[**Étape 7 Ajout des empruntes et details de bâtiments**** ****12**](https://docs.google.com/document/d/1xF8N18qUkqfF3hZ3HDEm7ZyoHe9Dg7VxzgECAgMKZE4/edit#heading=h.mtbwt3oe7v)

[**Étape 8 Jointure des propriétés du nuage de points dans les polygones**** ****14**](https://docs.google.com/document/d/1xF8N18qUkqfF3hZ3HDEm7ZyoHe9Dg7VxzgECAgMKZE4/edit#heading=h.vj3u30n7iutj)

[**Étape 9 Visualisation du résultat dans MaplibreGL**** ****18**](https://docs.google.com/document/d/1xF8N18qUkqfF3hZ3HDEm7ZyoHe9Dg7VxzgECAgMKZE4/edit#heading=h.hctb93vskptd)

****


# Étape 1 Importation et nettoyage des nuages de points

****

- Ajouter les 6 nuages de points suivante avec un **_LAS READER_**

****

<http://depot.ville.montreal.qc.ca/geomatique/lidar_aerien/2015/301-5041_2015.laz>

<http://depot.ville.montreal.qc.ca/geomatique/lidar_aerien/2015/301-5040_2015.laz>

<http://depot.ville.montreal.qc.ca/geomatique/lidar_aerien/2015/301-5039_2015.laz>

<http://depot.ville.montreal.qc.ca/geomatique/lidar_aerien/2015/300-5041_2015.laz>

<http://depot.ville.montreal.qc.ca/geomatique/lidar_aerien/2015/300-5040_2015.laz>

<http://depot.ville.montreal.qc.ca/geomatique/lidar_aerien/2015/300-5039_2015.laz>

****

![](https://lh4.googleusercontent.com/FKHkMRbo1wNbmlNNP6NFyHBuN9bB_vvEq9xcnwyfI3skTY6EM4sZrMoT8tGwo_iTwZrZ7gxh9DhUpDsLyYXyICORxwnlV46lTjPzheq7kdMkoEba2lI8Bn0UNtznWIFGFZPzQrz4Wv5sq0OnG7c8p-8)

****

- Ajoutez sur chacun des reader un **_Thinner _**avec un filtre de 30

****

![](https://lh4.googleusercontent.com/fKgDe27Tv1VEPv5AHXDkHpaiOHDDnV_Vji_0PpGK7mf4SnonTDVyjmB9e9mj1PxntqPS2LxHz8DE4AUD3RQEDukr3mnV3wo4HUPw8CgSV8K7i7ERLOegv3fSwT1BCTm1E8iegZ3p4DTFM3FFzRrleMM)

****

- Ensuite ajoutez y un **_pointcloudcombiner _**pour combiner les 6 nuages de points en 1 seul

****

![](https://lh3.googleusercontent.com/ETar2_3tOpo8VlHurIF7n1_hHvtgyLhWa0tifyNPJ76Tkr-xPyRkMNONY9I8mb-nuht5-bvQOxbLsVjdT_Jxt6zi5_YW8y1QL-oFP--_Ip1D91Gp5pE_McDgxziqkFasip-ncQpUfjecIIwVc-kqBOc)

****

- Puis un **_EsriReprojector (2950 to 3857)_**

****

![](https://lh5.googleusercontent.com/c3NBAyFftFMHyCM6D26kACT-xsJhIlMTD8SLWa1AyInz8o1EpT6Jro5YhEnoevoJzjchH8VrUBVSmuV0fYues2qvponip6Mam-pVcVlxBTvwVaqz_A5gpqqsLKZ6bRgztUQP7lkfixHO6TqwtXzoqQQ)

****

- La première étape devrait ressembler à ca

****

![](https://lh4.googleusercontent.com/9UUX_Fk1tYpazIN-huTwBEXCDJ-psKq7pDN6uYj1mlQzDRuv-2eg1Z4B4dMXkzyiJGM5uZ1FGYiCR7-ZljlKpDRKfacM5H2t9IFuWiBOqxGT-CFjb4jYOApr6bTudXfHJ9ZxXMHKXlM9AowJFEp0qDE)

![](https://lh3.googleusercontent.com/ssHzLj5RLDdYEfGK_68U1Lk4S-_oxTxb57C2JfzTDF6egZ9g6-PbQmT5ScStEEIKdHMW2T3FQgtvzUnhx77uvb_UlTXm0W0h4GiWVpgyZ9wms9YVhB3NZfOLDXu6hhhHR6TMETSk2kU1lXXfTGSVpkI)

****


# Étape 2 Importation des limites terrestres et découpage du nuage de points

****

- Ajoutez un **_GeoJSONReader (URL) _**puis un **_Reprojector 4326 vers 3857 _**

****

Datasource: 

****

<https://data.montreal.ca/dataset/b628f1da-9dc3-4bb1-9875-1470f891afb1/resource/92cb062a-11be-4222-9ea5-867e7e64c5ff/download/limites-terrestres.geojson>

****

![](https://lh6.googleusercontent.com/au8uzZNvjFFKmM_7r-xT3-zgC31tcJvE6-2-JD2j7tX40oUzn8d8GJ42_fwE0dEwA8nVppLrGToygE2c6UGhyR99wgpZHzaVZWnBe0jillWrgVtscziwptuFNdq3rgATgHdxd1dMi4N9SW1xB_Ei5Fs)

****

Ajoutez un **_Clipper _**pour découper le nuage de puis avec la limites terrestres pour enlever les points superflus qui dépasse de notre zone de travail

****

![](https://lh4.googleusercontent.com/N8oLyYUFKrDe5d40PELVs5f7ldRsfFGRXLrQFmbfyW_H9kvhoLYyjh5FyPXQsRhGKFdHN9NVIUAsRqtRr40-CR33oynozEWF1-SPqe680AupJvACIboTA70LLBNdE8ortKJRR_RUFSaJUFlCpKwW39A)

****

Cela devrait ressembler à ca

****

![](https://lh3.googleusercontent.com/LeUjh99jvbA34qlwbsm18kwZ-L9QI7qCxPSE0HOBrICqmEsdmqLwAByplA2YRFSOmHEPMOBV22RGu-dmnjA_scU6tWaEfRX7Xcn7PZEne29eDffKt8jxv6BlbM43NOyqh1wt2HlrWU413cU7_2DP1Gs)

****

Connectez le nuage de points combiné comme **_Clippee _**et les limites terrestres comme **_Clipper_**

****


# Étape 3 Simplification du nuage de points

Ensuite refaite un point **_thinner_** interval de 5 pour encore simplifier le nuage de points, normalement nous devrions effectuer un **_PointCloudSimplifier _**qui rend le nuage plus léger mais conserve sa forme, néanmoins ce processus est très gourmand en processing power, nous allons donc utiliser un thinner pour les biens de l’exercice

****

![](https://lh6.googleusercontent.com/0JvovJxzjc_j5a-ixNVWooSus8OvFoFJcU1pwy_IFuMeGWwEad-yMytU0zH3eKItQh3bLJkp_JVu0nWIP0XTrY-5H_M1hztt_EgOO1IuRIh8Qc8V7NzHFrjRdj1t_IsF3ap53sCSQO8svHH0N32u5qM)

****

![](https://lh4.googleusercontent.com/PHqKXSmVYdfUmAnuWJM1ssBYy3qjGpecD49aYxHSGALmxFRpCkBCSra8g1d4Vm2wVpFLhpNMKm2JX12NvWaiz_4hZ2fUHu1Km9gjfHUOlgzFmqcBjT-uvKfuGNXBwhUbu6xTYOrecJm9vNAuSdKboPM)

****


# Étape 4 Ajout de rasters géoréférencés 

****

Cet ajout nous permettra d’ajouter la couleur du raster à notre nuage de points

****

- Ajouter les 4 rasters d’un seul coup en sélectionnant les 4 et en faisant un drag and drop

****

![](https://lh5.googleusercontent.com/Kfz3aURKr8Zeq7xNqBIOu6jE7yuXtJTEdE9uxeXzbDjUXIdBd3Y0uyCQVxR9bRlHP09rTwlObwFBy4RrDscD7XE8N3EktebjKcc6yITKp5iePsnSMwRqEccegb8DWLuE5Cw4Uy4NUYdUQSeTUvdi_ZI)

****

- Ajoutez un **_reprojector _**3857 vers 32188 (équivalent au 2950 mais au standard de reprojection FME)

****

![](https://lh4.googleusercontent.com/h4jLIZrih5sNrzygRohFj3TVhyRI1sHRRn1VNVKlYqgBv-x5l8n_n-y9RVJ3l829hxiCoEMho1hNyU51Sk9HqC4rHggPXXvL5hhU7EL9D8JYf0UZOSwnzq_M5KDzA49UaXp7zXtHgOhsDxKq535OjrQ)

****

- Ajouter un **_rasterMosaicker_**

![](https://lh6.googleusercontent.com/HDHgUusHkrkRS5kmZnmIIn_H-aMEPcrnrZBA4y-ieSWJHPSvLc87Bz_7rLDrQK62JTXZ4EyQO2XfFez4eQhG5EvWedk65p6k9MFLh5mNVIcAoAVjwRjr7G3-ggP3aABys-dHuhOp6ztXtEWZjQmvIrU)

****

- Puis ajouter un **_RasterSelector _**pour choisir les 3 bandes RGB et supprimer la bande alpha

****

- Pour connaître sur quelle bande se situe quelle couleur vous pouvez ajouter un **_rasterPropertyExtractor _**et collez y un **_listExploder _**sur la propriété BAND

****

![](https://lh3.googleusercontent.com/-5xxjJFQvRXbtBedgC0hObvgHbT65BFbl55rueEtNOt4hu8hrD9T4ncpjmCfbGgenAcVJ5ylQ61jvPE7nXZdCzqcf_uUZX5cOK9_On1CAsxK8cNV1UuCKs2feKZSDbwSu6hRHktVilE8kaUFqTIV6yQ)

****

- Maintenant ajoutez un **_RasterSelector _**pour enlever la bande alpha

****

![](https://lh5.googleusercontent.com/orfgwNHdv4FL5IfSsgdL4lc27qMGglTuXxgxivZ86iryzBVbNLu3iPIWxm3ivJs7-hEKOlCaF9t3zqgTDb9whaYzPl5raZD-K3GqKdaIC057rSF0CKZZlip_u-aN9rZeEu4xXCG-UZuynpdc_qsiW8U)

****

Étape 6 Jointure raster et nuage de points

- Ajoutez la couleur dans votre nuage de point en ajoutant les valeur du raster avec un **_PointCloudOnRasterComponentSetter_**

****

![](https://lh3.googleusercontent.com/ZmXNh54X4zy5IRU1V6UcWym81S95G9kOoykEHUcTC6WOWygsw46uXz0nPFmljPa_D4g3HVLIiy_7YJ5GBxgdkMrKm1o_WsP7fbQ6BaO3DOGYL3DYwqL3qPvwFiLEGm_yUi5qB2MlPfPWSmlAGj4HdOQ)

****

- Ensuite on va combiner le résultat en 1 seul nuage avec un **_PointCloudCombiner_**

****

![](https://lh4.googleusercontent.com/JOMlnAojAHflxhJrp-K2IoxmEJ6SuANUe3xV_Ku6Ppl9EKQ-eMUkNsEewE4SuaXDkP9jK_fZpNqvZrN-MFOjRV9PU1fCzw0-IllZiOxvd5Rh-GqPB668pX8ud0C9zQ48LDLkUnvmV493rlXMPsSQyw8)

- Ensuite on va filtrer les valeurs du nuage de points dont le raster n’a pas donné de valeur avec un **_pointCloudFilter_**

****

![](https://lh6.googleusercontent.com/Uau9zmWvVYJfYOd9ttrG_bWqui-2rTvqSUW9BJmjEvCLD-HLQiM--6thXUW5MaIZcnBUbp4E756in6jfbVXMGOuXMQcW3G2SnN76TLf2s3VZV6BHOdlzAsqb0vi1rnxhJ9pt19onDBpsi9VFYsoMw8Y)

****

Pour filtrer on va choisir les valeurs RGB qui sont toutes à 0 avec l’expression suivante :

****

_@Component(color_red)!=0&&@Component(color_blue)!=0&&@Component(color_green) _

****

- Puis pour terminer nous allons transformer le nuage de points en couche de vecteurs ponctuels simple avec un **_PointCloudCoercer_**, en s’assurant de garder les composantes nécessaires pour la suite

****

_![](https://lh6.googleusercontent.com/_3irTWv-Zonh70yBQph08wiOQx59THPLfjS63UjeiMLqgRKDiDvrPgDPMVGeO3C7tUNhncx0wP69lMkrOPaecYMsVKFLm7iB7vo1PbuYdM6acxdFyYzZmQb_6h43a91AMCZ80GgaLR9fr9XCUAQZ9Bk)___


# Étape 7 Ajout des empruntes et details de bâtiments

****

Maintenant que le nuage de point est nettoyé et préparé, nous allons assigner le Z et la couleur aux polygones de bâtiments

****

- Ajoutez 2 **_sources shapefiles_** pour les empreintes de toits  (polygones) et les détails des toits (lignes)

****

- Reprojetez 2950 en 3857 avec un **_EsriReprojector_**

****

![](https://lh5.googleusercontent.com/6FnJroaV58ONjYarA-P7OO2ggLsoZdva1evA5FyunRHF4IhJ1Ghpr94mpJDFvV_K5iFILwVJ2Hi55PvwP0oEgs3FDvaj7aiyKqRC-V1UMSbKZGg_h_eSPivdyt46K41vg47siYfYoSTStFlexBByHUY)

- Calculez le bounding box du nuage de points avec un **_BoundingBoxAccumulator_**

****

![](https://lh3.googleusercontent.com/mvGioO0TeBFInGgGWfbc3LbkVF9xf5kmB1LhqOS5QWwWukctHu38Y7jz4lRxbAz83fWM67ivG72xclZQ_DWWMLQprOAUyoIMQcmkvf1oSwUQQP1lV5AbO5-c2dbN1GOryW87QANSVnklsdtcjlTkXrw)

****

- Ensuite on découpe avec un Clipper les polygones et les lignes

****

![](https://lh5.googleusercontent.com/jAzoPBH9F3FQ48Lw1VWDr01Fg4d6Y6xUVVWYrjl4Jg23Pk01PiYB5ckmvwwQyxYhw6LC-eQp6RZUQrRul1kRFVSgMjSiy0D66EoE0khjQv6HhY4JxU5L8YcR9E_Bsv560HdzkW1WfkVHRx63Oit5Tgk)

****

- Et on découpe les empreintes de toits avec les détails avec un **_PolygonCutter _**issue du **_FMEHub_**

****

![](https://lh4.googleusercontent.com/_acOQw06QPjX4H9vmGzcU7NT16DE4R5z3jvAqfKsIMMkxiwrX0uQnvqpeifO3n15QudAauijj1ZC2MN3EOw6B65ecGj7n7r8MoCJAlZPVwFXA9uO-syt3SYhkLdo8MDEfBq4SmkmHla8qbM-5wJ1g10)

****


# Étape 8 Jointure des propriétés du nuage de points dans les polygones

****

- Puis on vient joindre les polygones détaillés avec les points du nuages de points pour y injecter les valeurs de Z et de couleur du batiments avec un **_PointOnAreaOverlayer_**

****

![](https://lh4.googleusercontent.com/N3vX_pn6OZ8rp2ZgVLdtFa0JtOIoZQYi6tsXkeZ1mrnEMSVlHJLDhpkly73c3FTAAUXtVGcWkp5YvAJLsL_RPTLXS5iK5q-9OrGbhR-NbsZcEvaTo5iDGXPiiY_nDBdqZnx74l_JAkYCkopncsZrhuc)

****

! Attention ! ici on va accumuler les informations de Z et de couleurs pour ensuite calculer les moyennes qui nous permettront d’attribuer à chaque “bâtiments” une hauteur moyenne et une couleur

****

![](https://lh5.googleusercontent.com/v7UViwqgYeYvgivv499b_Fb9jPUtz9MIBDcj5LUBUqCQb4WObVRz1CEg4d_eG1eV4_1hUMnm-R-nnouFGb9WKYTITEKbMZ5drwQcODM9SRyuWoXVWWU3UV7GhvXiXDR-wsmENS3cj7uFaPneacegFAM)

****

- On ajoute un **_ListSummer _**

![](https://lh6.googleusercontent.com/YXZJRpHkDdfB-7sAbrB-oRXGGOdEFa_arAhZ70Ps6-Xjn31AkrodYlIvuX1fTetjCU1DPiLJ1hwq-gjzgUSH6twBZI6cLYFDiqPz7-TuHZ5Wwtaz8SeI4fGF-hSx_OeM8P1WqJ0UjS8WOh8BCGkzFuA)

****

- Ensuite on va créer un attribut pour calculer la moyenne **_AttributeCreator_**

****

_@Evaluate(@round(@Value(\_sum)/@Value(\_overlaps),4))_

****

![](https://lh5.googleusercontent.com/i60jRXVwO1FOTB2O1Bl7ho26UvhlH5-CgQDteMu_bqVlsntC_1IDziIuVcg6cW6wCCmFOoYAkqT4J-mdcez4qxCkCVOSp0N0z1ZVx5FPQmPSqvqZw9wSbTgGo8KsVHgQbmCY9PwfQUqpX62ogtG9-fc)

****

- Ensuite on fait un peu de ménage pour garder seulement les 2 propriétés qui nous intéressent avec un **_AttributeManager_**

****

![](https://lh6.googleusercontent.com/517tzLOKQGF0egSrYyA0UpUxpZIufzQ0Syotw0zZ8DdQbACvAg3dh701s15omoKz6DaB9xee1y_-gNwetxJ01ItpOhgsqtScuZJ6ELppa-I9QoZIaYd0s1oNYPBPUxio16TlORu72wI9HV9oy9wPmSY)

****

- Ensuite on transforme le FME color en RGB ou WebRGB  avec un **_ColorConverter _**(FME Hub)

![](https://lh6.googleusercontent.com/TFVzgLNFnO8Dr449LF0-UIpjiG0IhGNHBmU5lkVBHvw7JuyBCMkrRF0NzKRXGTbbzaqXJAtSISH198xDK6LC9e53r288Mw2YEH7gfvb5BTNo7stLi80n5uoBEKwqdY2d2_CAkItbdXQuNnOD_BxOWbk)

****

- Puis on exporte notre résultat avec **_GeoJSONWriter_** dans le répertoire : 

****

- _…/Lab3/results/bati3d.json_

****


# Étape 9 Visualisation du résultat dans MaplibreGL

- Ouvrez un navigateur de fichiers et allez dans le dossier Lab3

****

![](https://lh5.googleusercontent.com/nQJnYHkCM6ShugjtLf4PBwxFQFquLUSQ5ly9eLfEJNo89DJQDDCVRRB7O7OPGb4BHsh7WNkxGYgf8cSMjwcVeZs4lE_1bFZyh5mWI25vU0BxscMrQBhtK1KyA0skGQNxIU4eCZofFZAz2yc0WkFSZws)

****

- On ouvre le fichier MaplibreGL.html en double cliquant dessus dans le répertoire /Lab3/results/MaplibreGL.html

****

- Cliquez sur le bouton importer en haut à gauche et choisissez le bati3d.json, cela vous permettra de naviguer et visualiser les bâtiments à votre guise.

![](https://lh4.googleusercontent.com/-Y8hghpEeEFmWZU8o7iiyuddjGVsi4nkdD9Rdfb2n8rEkXzjVucD36Y1Rg87HloKYKegV_Q7fcx_ZLELUI3jHLnmWN9NA7WBaIaLpxTsjR1mW_RczUbhdMMhTm1_4zHlcyOu4YMY60PumSWMShbh6hI)
