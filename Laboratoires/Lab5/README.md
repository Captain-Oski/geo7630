## Laboratoire #5 (cours 8) 

# ArcGIS Online, Dashboard et Experience Builder et intégration de données

[**Import dans AGOL**** ****2**](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.obevib9yx6mf)

[CSV Reader 2](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.j7ityrx72w9k)

[AttributeFilter 2](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.qqurfanc4ilv)

[StatisticsCalculator 3](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.eic7z1m2romu)

[AttributeManager 4](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.ehpp8heg86oj)

[FeatureJoiner 5](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.onmraas8odt0)

[AttributeManager 7](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.cb4tjxg1ufhp)

[Writer 8](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.69efvtz164xk)

[**Visualisation dans AGOL**** ****9**](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.dqstqds7kjjb)

[Création dossier 9](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.aayizmqhxfyo)

[Mapviewer 11](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.suq8myuqhmb)

[**ESRI Dashboard**** ****16**](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.qv1fefk9hkpg)

[**ESRI Experience Builder**** ****31**](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.snf7ukc56jh9)

[**Mise à jour des données avec FME**** ****46**](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.14qyickzd8g4)

[CSV Reader 46](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.hmedi9fwzw22)

[AGOL Reader 46](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.srjjyuumq9cx)

[ChangeDetector 48](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.8xnmfix0o0jl)

[AttributeManager 48](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.9e72ikq2mal)

[AGOL Writer 49](https://docs.google.com/document/d/1YyRCHBF2Hnsxj9undJGvuv2Y3CrUJ2muZf9nCIN0cCo/edit#heading=h.hx15v63ygt0x)


# Import dans AGOL


## CSV Reader

1. Créer un nouveau WB FME


2. Ajouter un nouveau CSV Reader


3. Utilisez l’url suivante pour le CSV :

<https://sitewebbixi.s3.amazonaws.com/uploads/docs/20220107-donnees-ouvertes-8aa623.zip>


## AttributeFilter

1. Ajoutez-y un attributeFilter comme ceci 

   1. Ajoutez -1 pour filtrer les stations qui ont des mauvaises coordonnées

![](https://lh3.googleusercontent.com/DERi6aPrc6BIeztoN_rOub4ptzticjJuoouvqlZ_G4B3Qoe6U-BbTqRaUTKlmC-gjXliSUXCdxYeM7aIQzHT_NyVf2v9Ul0jeYyrA6OnGONYD5CKLlBbHmNEF8oaMhyWfT99UDgAVl1KPRH4-l6_kWM)


## StatisticsCalculator

1. Ajoutez y un statisticsCalculator sur le port “missing”

![](https://lh5.googleusercontent.com/N523RTKPPKAjr59cdcErKnx08QrmDjrSVPeUjNNUtjFOme7bSttgWiIS2YYr50Nj2QXkFSq2ejLZxwIz3G8mCOq423xJjDFVawvQqQ-UVw6LEzrfSAz62FpiKBHtxCCVMenlw8zuGG3UK_EwUK9KwFI)

1. Puis un autre sur le port : “missing”

![](https://lh5.googleusercontent.com/YAloEAB6JSkgNgZkXz4Un2X8QPmMLNPCu8rOQQH0x7i2G9hAXpjqrRYletaKssfAyzkyCLzVL91nUoCBh5C5MQVbBJaMxklZ85zxgw5p1EP4k4AHpQl84S-EXhC5khvJ0S2i8fwTLXUQ45r8LZSEn8k)







## AttributeManager

1. Puis un attributeManager sur le port : Unfiltered

![](https://lh4.googleusercontent.com/L36y6RyU9nv2I8XQiQFwQ-kuj2bGurPBV_uZXOPlWqifjuCq5b4x2Bgo-0oHxtQlKAtAbXlcQkEGbUtYuhsgxpHxm0JpcymQyB1fNInfaLiCdVYODoIccdrHY61kddMSMOWY7A_eAm0kNBtwwpcnalY)

Rendu après quelques étapes

![](https://lh5.googleusercontent.com/vtEhyxX53XYV_6UmTsJ8dZ6joU68EG4pcwAOoA8RYloq7JTEaswmdlcTM896Y5CXvqptNxE55dnVbg5x-sSIPw6HO7H4gc1S_sX_pUXITQ0FS-EbAPMcVn8CuEpGOCrWT7W1xNqLj8dYINVqbHD1jck)




## FeatureJoiner

1. Ajoutez y un featureJoiner

![](https://lh6.googleusercontent.com/erMjGbnJnPYEP6dh-Bk3EejAY0HGPLvtiSEeCZD1RRHCXGlxaK1ftc3pj-KPjN9xVzxw3gG_bXvDlL9qQQwU_ZhNo_9tZnoKzIM5QU0ReLWS7G5nczEOYCoEjB2FY0k9UH56iSHk1Ku3IRBu3wEFK0U)

1. Puis un autre featureJoiner enchaîné

![](https://lh3.googleusercontent.com/NEFFkISw5lnwpqtWitenm6rlhf7DIjm6WTFp1rOmx1JEFQlsVZz6kIkE9Jhi0S3teGxA0HOlhGQtznCq6NldV8POaOlJD-1Cv9ZYBwW52GLUTwzTJYb54tIpsO6tdbmBO6mpv1VrKWeQ2NW7FDxh3ds)


## AttributeManager

Puis un attribute manager

![](https://lh3.googleusercontent.com/QBqFjKYTTUQKUrXQMq-0k69FBhauTlGIDd8Olqk_I_Zsum51Vaw-7BvkjH6NFHfnt_M78P9nRvxQ1_bar7xyC2vkofjmNT7eBMtHmLbylaoVGWm3AeOeRzDr8bhRS43FUhQJBj1NcRfHbFoCzpauhz4)

Rendu après quelques étapes

![](https://lh4.googleusercontent.com/uLIEy4U9ZHNHvyZgrRJ-ljYFUSG1ENtrfmJOI1zVmmQF5sE-3eLgF05ubp8XzKE2I9_uvwmuW2uRHYS7M81W6wlVDvf3X3_sRitWPTdZBF3Nzdl_wiRDbaoXKPDGNlD6ff04Fnh2CTa3S4aHEvexs0M)


## Writer

  


![](https://lh5.googleusercontent.com/nqnx2o6oEIyd8HYAKbNsH-KUr0MVeckO7ChqmfWLV57X7Bmv6AryG38VOuYcq04kEfMXoMtJ3maCU8WXNK1GVdhXTJzY9TR_L7YEOv5f92afprb1chivFJgYtRHADdZr4tVKOcuNkT8wN7y4yuQspYQ)

1. Avec connexion avec votre compte AGOL

![](https://lh5.googleusercontent.com/UG9eVBxhiBYB3SPPibrS6HuF99GsAfcvZrcK_RS9J12N8MtK69qyMpaQmxZAFrkziIWEI-bvBb58hQnI848XgzhdSCSsHFxXqik9HfZ-oBzGRnsBOZdhv9LqCjw3cRWJbDXYRqf5KAFbRUkDkg1X8L0)


# Visualisation dans AGOL


## Création dossier

1. Allez dans votre page de contenu AGOL et créer un nouveau DOSSIER GEO7630

<https://www.arcgis.com/index.html>

  


![](https://lh6.googleusercontent.com/uLuiYGl6LG5-5TSCIkY5StLflcglZoKwVM37OH8ek0cOc-3SKs_jhrXOQYmcV_BwycYdLF6Q-SBqi6X9-N3vD15Gh4fbf1ItIa4B3laDEQHB3M_UtvwUV6YyzrDByCXPqJbCqYQrcJrhgpTiNWMY-bg)

1. Déplacer votre nouveau FEATURE SERVICE dans le dossier

![](https://lh3.googleusercontent.com/MTaD6UJxBSO9_tZfvtfyIv3Fhr7jzdGQ06bvX_JTJj0NFn20mI8dMujOD41_A1N3b8KaYxFWyaNGMMF-gZ3RZFehma8XyPuZ50tc7HjqHtjAKOay0yPf82DKIOMWAK0qXc7k_TWzZd4dwthbj4ohERs)

![](https://lh3.googleusercontent.com/IeYomYhtOUy2Yz_WxU6MCDY99_fcUiDry2eDrBK_ZMRO9dyVgIpwilmlOAyKFyaotgRpdgRKOnc-xsRNVTSWkBz7YqEsLHhZs2alElGO3-xbe2HU-sd1YH3nZhdFlQX5txYtIL4k35UtztYlu9zSPEw)

1. Allez à la page Contenu


2. Maintenant cliquez sur votre Nouveau FeatureLayer


3. Et cliquez sur Ouvrir dans MapViewer


## Mapviewer

1. Vous avez maintenant la possibilité de jouer avec les différentes propriétés de la couche
2. Cliquez sur Agrégation

![](https://lh3.googleusercontent.com/vCpinqtMR3zLJvQBf4d45t8kosiWX62rXZIv-v2qJ3odBaZTpp_mB2Qd_yVC8fudW0CbvuJE4ySIvRB_u3d8eTSRGJMAetsKK94o0fFW96yYKMeq15iwTSz_uK5BBVqA4zd8WVy46C9gTcJRz0Tzk7g)

1. Maintenant cliquez sur Styles
2. Choisissez Comparer A à B

![](https://lh3.googleusercontent.com/9GsWnhGoyTvB6MgfjMqO023D3PFEV75S_uuFmnWahp3Ae62YbwYL7F9H6tprBKVJWYFmut3I_Jmw-trAG8LfvwD2Fi5Fa_qiEzegH9jb3BsB4FrcFHu0LM3lGAF4PmfifW9uh5LeUIqbY01kRMTs0Ek)

  
  


1. Choisissez Étiquette A pourcentage de A et B

![](https://lh4.googleusercontent.com/GLkK091TFvqTVNSzQ6pC9B9Q5A5rJXSZxho7-ThHNhdBzx0spqqzGO9qPO_expTVOzbJMxeQljDMBNezxT6OS3W-hj5Un94rmSdhbWr1in5nGxTjT2bvJvF5oqWHOcoP_QqcsGbR-C0QnKbSF4xzY94)

  
  
  
  


1. Ensuite enregistrer en tant que “CARTE”

![](https://lh5.googleusercontent.com/B4n1xRJv8jlfpKP6jjkhYHq5vDa-00Ll5mzSYkW43y1zqewvMuGG5J7wOi4ahEnyjNTLIP7xbIgnZherh6mXXJEqfxASFv0Wo0FUvdMV0Nr89v-Z_mI71esfg8DbIBi50lQkDAsMXUBnz2sH-0UO46c)

Une fois enregistré cliquez sur le menu d’applications : 

![](https://lh4.googleusercontent.com/51MYgQqo60HME2SrK8j4aS3LQcQdpp7OLpN4fxdW5yIwtzeY30TPS9RSVzj7JJmvd81PCjYcuyO-wfFaqPM0jloebkBK04AlnMmtZfclk0k03mQ_QbNhGIFWz_Xi2gkidX_tpOpGO0Wz3sE_I4QQfow)




# ESRI Dashboard

1. Créer un nouveau tableau de bord et choisissez le bon dossier

![](https://lh5.googleusercontent.com/5mNkcT1COm0H3p5mIsBbfEqlx08QgWsR0OAy8ajtJJBMI3gzTtomb-zW_3eO1YeJIe9b3nq8BZ9tHDKSsTTAMnbxnio-J_hzCKHbFdWU_j8IvHWJ2LBnsd3ybxOEDMmdSNzHpFi6xfUj74zHuAK2fgk)

1. Ajoutez un élément CARTE

![](https://lh3.googleusercontent.com/bYda0qLiZLIpA4uoDG6_BP6KyK9TUq50FBEfKB4h9baS3dgjfpdOp1SJXSRCzv1XhKr2dxjuxxroAUnTnm17lBSPucssfort_aWSUXnt2ACZgiLjquJu6p1fWgvqRDeRm0i0TpnIM6qJbAMnDvLlWIA)

1. Et choisissez la carte précédemment créer avec les clusters

![](https://lh3.googleusercontent.com/h2jsLGPn7Dbj74D_nUmrBjhQPlxS4lacV5SLce4pDoYVA1v0tky22aOxERWmRwScRRMcCibvejSIQCu8hwVA7PzHRXhA8n-hozZLvpYr9f1IwsqRWUWN9eRYfcCM28WjvDx0y7uRP9SqbB21DEAj50s)

1. Dans réglages choisissez les options que vous désirez
2. Puis cliquez sur terminé

![](https://lh6.googleusercontent.com/QljA2Zi0wG1LPjFYc80Vp2AvkB4-1d9X47yuWtO7pQGgCrT3FaAgAG1dc3F-BEF_KbnCYXMqZ5NYE4pTTMLcafW_bg72JhIEkdMlqqGCcKxY-ISmuCFp_QuqlnJLnrk6EMdoKWsHCjd9B0RgLJIeIDI)

1. Maintenant dans Mise en page 
2. Ajouter une entête

![](https://lh3.googleusercontent.com/FQIUfc1cxUIeTTGKPYOyHde6dJEu_dnE4UUsif3QoLnhQGJFdPKFN_UGl-Myz_uQ6YB4ZwmOhtbwVnRDxocmPHjeVq9-GIc_kLRHG5QtVcCMF__H0yK2-K1zEfcJQLzx7wY38y8RhNa-oqkqvTmTgTU)

  


Exemple d’entête

![](https://lh4.googleusercontent.com/NOPDKfJXTGJ746sshAc9Up9UvXb0DCXky-e9MZwRP5YaS8gb9KKXfhWNlC4sBtXRvLkiKuKjcT3RQ4fC40dK1aJmEqKiDwspjR4TGyyQONjKRtjUrBW3NBLrdiNSlP-6NYF-UYhnEF9wNPoq30OMGZU)

1. Dans CORPS 
2. Ajouter un élément en de type JAUGE

![](https://lh6.googleusercontent.com/uM_wqnrY733UQQ3unkhWP-fchwpgplXvP7eQvl_C4f7iH_rEo6otryvzb9GtYhykI1iBtKe8JAtw10sNoYK2M_EIg0BD5dq8diEPTtJK32g4WGwusd75NyHM6qNkuLO4EZbwK9ZlXOuwLuoTcpV-pW8)

1. Avec la somme statistique sur le start

![](https://lh5.googleusercontent.com/vAjvzKh9s5BC2eKoSbO_aPfjCOudvm8sv2-KFz6tE1-FPcxzzwVOH836YkJzg8SvE_Lu2TEG8kUir8ILXEXjwu0gd3zhCyr8QPgDn8axWcwYtVv0XV3B2Mm7pfh4Y0YAA48o5er91eKKSAMjsoerAKE)

1. Dans généralité changez le Titre et enregistrer


2. Maintenant faites glisser la jauge en bas de la carte

![](https://lh6.googleusercontent.com/nA-gP4G4-VqO3n-4Vvp4mX3rNEJnKEo2k4_hVnsa_wCwzqdS9diqkwY3bMdKjRl-ZjO26veUf2Zfqt4HaB_nLC4hqXCkWHEidZx-JMchKLjjE9wS0_6joVDeXhiP1q1HhPvGYQOPc4UIAa8pl3EdT9s)

1. Ajoutez une deuxième jauge mais sur la sommes de la fin des déplacements

![](https://lh6.googleusercontent.com/OgcizEJX08tFMD6ic25z9GEkNO0wZNap10cy7UgqvI99oeQi3YYobmIPfxK8aPNVSA4i13qB8h3f83t0CNHMm9MpJjo-2_SXosSBo8uaSS3nkcKbEDTHKQ9K43QjZpwdSSCuzdrsedswtOR9ApS2Hek)

1. Ajouter maintenant un indicateur

![](https://lh5.googleusercontent.com/QFOFWF-HXIPUNblA1g4XdCE9sjTO111g_wNyQdckfEpunrcW8ULHr1xsgLyZ45eBCbKgcCAuA96gr5azyn4bHvdodxlJhOOlmY95Q_eEkDisqwcPyexav3e-_jEJoQFGhoZydC8Nhy2sUwBmgq0vAK4)

1. Dans INDICATEUR cliquez sur ACTIVER (mise en forme avancée)

![](https://lh5.googleusercontent.com/p6K716w2EBD11Gz7B9JiCaEPTQtmcylA1jSkypSgTT8v-WTeJ5ht3hPLSy0H98lhRh3ocY4riJzUS7yJlGHgj1NCtPb1Xv5vYE11r4SGfHRHkup1KUBkTTAlXL-fwHDMwtRfchGaTLT67uhZ3Mbgdws)

![](https://lh6.googleusercontent.com/b6806xDtw3hhV-Mcna8ROlhCEc0Z2X0BBIvL4K5R1eVldmmARCCfIAnd-8AXLAh3-KX7FeunJsWs3SPQF7PMjK754N2HYN7Ricwnr0ruJcChA0QU1DG_-UNjft9JjQwCEZogJcEKs3_aRkk_WlF76Ws)

  
  
  


1. Ajouter TOPTEXT : 
2.   topText: 'Ratio départ / arrivée',
3. et
4.   topTextMaxSize: 'medium',
5. et 
6.   middleText: Round($datapoint.sum_start_total_count/$reference.sum_end_total_count,3)

  
  
  


1. Maintenant dans DONNÉES
2. Activer Référence

![](https://lh4.googleusercontent.com/_EwWpvxpV3r9vhy4sdO2QwiuLaWFfEqvGI9OAo308bMmC3sjWOB8dVQBoeSckLJvz2Ty5e7ApgKB7zTRPIY7Gkuo4tW2iGxjkg4tDn681kQBs_tuZfKCYsh7vdYn8PYaAG1_olnbh2lvv9wPAIclidk)

![](https://lh3.googleusercontent.com/GUikShTnhiJVHHrZafNbFdNVoVBw7lR8x6Ib_NZeX4HcYMd3bdB8Afvvoyek9C-H8mQ7iJRu8uuaaZT162L8mBrlfIyF97Ge3QwEvV4Ahg87-RnMTYEWjigUkerfnBNIZW4nwkV8x-Rd6_tpG60Vpvs)

1. Maintenant ajouter un nouvel indicateur sur le total de station à l’écran

![](https://lh6.googleusercontent.com/SkagcTlPL3e8N3cV4pKc48hV0TESkX7jCDAFvzKfiqUdn3LnjG_uCzEs36uT5OLOfKzeWQWQ6sziR0oBbjPRTEosDPfKwizUnK33C_1Vop1z_CFf6Lw88d-WOpw9HE2jzTN0d4qf1j-lhA1nxCvFbps)

1. Et une légende

![](https://lh4.googleusercontent.com/m4Dfs1j0wYRRe-XjYuz6cr2dQNrU4c0NgnmM5Oqs5nTNSsuTrA-strhwZ7iX1sR1tqmY5xAO5-1yC1ZPXQcCePYr_FCxZleBgnL2hbBFKFmMl-u2c0avwh4om0AZ48v7jDWVRF7HI5qacqewwcp2Urw)

Voici à quoi votre Dashboard doit ressembler

![](https://lh6.googleusercontent.com/8uoI_7Et0CW110PSi-KgPCBwRAPy43hPfQtHpv6CXJZHBbD6j4FzxyE_idJX-s2RU1Bfn-cHtguaszltFI3m_digYexZ_QkrN2l9XxVIsMGhER7JaADKMnniN3S6FrQmXnFnEGhICoK4Ofb-jE4DzYk)

1. Maintenant on va activer le calcul dynamique sur chacun des widgets
2. Cliquez sur Configurer la carte

![](https://lh4.googleusercontent.com/azQT_ZXnWuvvoSBk6mSklJyXfrX1lxGO4vHNVUcxsMoHkbHM17BP69V8jwV4tMreZ0XbhANPt1ivvaw0uV4tRsXlMLpk9EZYq58gPisD-0KExx14v0oVFYVmCA0dAKjDEbDbMTZnZC3YKngslAbfXrc)

1. Allez dans ACTIONS SUR LA CARTE et activer toutes valeurs de filtre

![](https://lh3.googleusercontent.com/SRyNB-1v5MflvomXCe49cm495uEeCUdrMtR2fzIkN69gkgY4lkidBkXIl00GTQ46m_lh6gCKczVhDlRA3_y1zcGvHC38Ts3w3zuLXYLWqb5p8RhVKTHwHIygnSqX0M_rOfP4QdzqZCzTrQYuV7zyL20)

1. Maintenant vous pouvez personnaliser votre thème de DB

![](https://lh5.googleusercontent.com/2WfS4waki4va_dWTvw1LNdsxbElmYBN5S-MHl2T8xpKuvBoGEhp6tOjuwLmULbtwYGt4HkNzXBXwL7dIfn7gKsWA_HegxNyxD3anw0qd62dSvA3FbAMomHRp3AcKqp11TOP3kicW8WiPa7czCp2xYs4)

1. Bonus : Fer à cheval avec canal dynamique (si temps en classe le permet)

![](https://lh3.googleusercontent.com/mCkIB0tOE-4FUXqvTeSs5eRMllLhzlTGg2rFSSEXyNELtslz1tUo2ElrdHpByguEXT6FHuzDZBLZdo7MTZFt2aZFdQBSMh3YRo2rpy3aBKlF0iHHn8cVXIwDkr94ALzmTv4cPI3ZI68DRKD8epiDcxE)

![](https://lh4.googleusercontent.com/6RX2GLj-57fH7A1JKV7DNgYAmcBHmHg-1Q0r5qEJC48ToDx3utLTegy_mjy7lgMMeTD59W1bHICAxPVQgVaO1aZSmXV-qqRZ2Rjtm82yjDmy-INSWMIDuf9moBqREjl5VSDpl20rulhOfIU-j11oLgA)


# ESRI Experience Builder

Ouvrir EB

![](https://lh5.googleusercontent.com/Wv80SMr9P8i-J0XQ3or8MVCbk1ve-OPShFySTy6ObcdvQ0yu_UfDQYO0g6aVXXKOGNboh-bjyiwB4MxJbgak8maKVBJu4EdwCGBTYGR_etKQvfhVKr4TPwZMzyuc6M7SrKwDVqu9r9fhCV5_5HpvOD8)

Créer un nouveau EB![](https://lh5.googleusercontent.com/4TT9XZGQw0nyzse6BRyMiC8-5ISxyUrqH9N-0GRidDCV9BHI2L1ncUdmjyA3F2J2-yOKKjLy2D1mEj22CJ-KvylxOFYOVN_MndxmJne7WK7Mn-Wd26vAKtyM-EnrXjwvc-UZ_AaJCgMHv1JpQje8AEg)

Choisir un template Grille vierge

![](https://lh4.googleusercontent.com/4WU68uGGLbZWHH9x7ZcUwVHM8d1g9GVY1uJ6ef6AzPntwAcBX4mOhJxRV1icOlOl0qipSRxr4fZIId-8IYqiw7nJH8yExgEdnHVzkSsHt6IE1vtJN04eBuV-TuhDj7t_TkzI9cONnQCf27lOyaDGwG0)

  


Ajouter une carte

![](https://lh6.googleusercontent.com/E0daj6AHNshLgxt-N2ZQdgARu0rw_zpPJZH2O7HJOOsUnhfRRHOBmxWEByPnQwWAFJ3Mub6T82rJAC6BWRyyfKKlW3taAv-XZox-XExzNLo6_X3CnbohT5sSVWdPD0XKE8Z2mOgYBlAMrydhF1f6qB0)

Modifier la carte avec le bouton “Sélectionner une carte sur la droite”

![](https://lh5.googleusercontent.com/R9l1VwocFD-o4oseleKCJzjcoKWPgfTr16IJuR5rBm7w_SYm4WP2alXZ9hZSnAQpOIMfCUCAT6yhYbOZo3eFF_Gz3VbBtWx7kJBN12ZQ3YGbVLNUrOSrkDDBEMe_i7pwwJkArBcEB0oYgtdZxNe7Fw4)

Cliquez sur l'icône PAGE à gauche

![](https://lh4.googleusercontent.com/E4VlxekLDHy4N14IbnhsGdj3JAtUSmGdQDMdwiuLOshADlDyUh87IYa8RX_2mHB6E7tAAwFe9gFMUHg3u94fhrvNSJjb4vv7xN5pxtt6hbabsj8gJ_rSjU35nbBHrvatH4QERPWdyor-_bfT8Rbed2A)

![](https://lh4.googleusercontent.com/JHUfk10wttM7AHsx5i_181skp4c6Aag9BrC_XlUCMwEZZiKjcVTbl6mGJJe6vxcEhnBUuO_WKsT0IEU6h5RTf7JFaQelXqQXFU-dACj6FAW7IbABZ1oaqULi-wMw_BRwBSgg9gZbjVflpWiyWi2_yMU)

Cliquez sur ajouter des données en bas à gauche

![](https://lh3.googleusercontent.com/AKsVrdlY0ruMQyD1LUi_8DJLujniy5MIGMmdsH368oYPxQRTR1Rk9dF82LQNdUfbBaziDXDTbgw_qH3OFucYTG5std97IRM3MmAUqtqWth63X73YD53j6Y7eqQtUz3P_SLWm9G4xAVqGEMoFyVK6LHk)

Choisissez la bonne carte

![](https://lh3.googleusercontent.com/vbuE2oZXbnIDLVCvcHXMkaTJx4g-f6QhHstT-pPgdbW5eaG1y1iRdEqoIS2iVehzLMAByx0hz29LV89nuehyCtwQFzukB9m-6hSh53lSD2dMd9QU4sE3Yz5JUHr72ZiJItAhxx-azSl4Un9n8tI6A40)

Exemple de rendu

![](https://lh6.googleusercontent.com/QEOGKRWs1D0wmp9NN5T1tkDC8QL3lAFOHOvNdM-SofEc7S-VTty2gJEL1EUP496FWDS8js6NI0SMffNiOr1-TXFFxQ-uKVdAg_decCg1lLPvIo7WoZXaTQd1hxTP-W_bYB9i4BZ688OGDQiG3iqKAcI)

Insérer la légende en drag and drop

![](https://lh4.googleusercontent.com/Kkg9Ihe03pLbRAzNmIXWlXtRhfcdgqmoOnPdAWAlgVGx_8dBvKEKwuvrr1pMZl0f2n1DgHB2xaUM4qQUZlVPNNNKdx9p7eZq8qTVDZ6r6Ft52TFF_9Wb2Au2-AzH_7JXpUY5BYoOID0SQExyuQnuXVA)

Puis des Geosignets

![](https://lh5.googleusercontent.com/awG9QR9wJpupBJzvw_iQNEGaLTr_67Jl0AYcEGj5JXlZghWP34-MuUrLt9qHlY4HudJHOdVTCMCnjF8V3p3CgYhKoC-ew-NloHRdoTgMdVDVcpCCZ2uLClEsC0nFKaFAVzy6Sw9etSQgD71UmIitRj8)

Exemple pour ajouter et modifier un geosignet

![](https://lh6.googleusercontent.com/lS_H_AXx5FYnkJ1Vy1lEIRjz03pmSTs2oEmjkUOIqBYUZ1oi7_T9LeqzAchB3JwEAgLJRg0nkzTcA0SvbZNpmfadONabts6ctz_1DfxejQf5H98HrJm_ee_66MW1o9eOyNuyg67_qlcm4UUgqUEnhL8)![](https://lh6.googleusercontent.com/SVZLvJEzVddmFPd2Kt_2_Md9umEqIcY2f6Of7L49QrVbK2mlJHWJfcnFWV0oQs1UhoSNSBb94OaUkt4Q5CNFkcQlHpkFJD1voPp_54Lr9JraLnhojf9AJpLgwNrAFUVm22T79_mM2uRA3i201s8pLUY)

Dans le même genre d’idée ajouter une TABLE et 2 éléments de texte comme ci-dessous

![](https://lh4.googleusercontent.com/mK9fQuG-RDUo3myJ7cEZrJ52HqaziqCz9AXpzxAv5N9cgcbbUXN3Zh_paXgMw7cMTPnuRRRR-G0oexPo-PYqjVFb90mLH7x9IbtbVMkWB2e2zQbysUiRUW4Ir_UeSqJhJV067Kpyc8w3YNTx1GJ4VTc)

Table

![](https://lh6.googleusercontent.com/pIbKJRWF02CTbt7S-QqpbNvx9COAgUu-7MNnwwJhZcknPJZg4ldwVQbtzpc9LwdF1_gx7mXIUgTN7-ZR2PwQLacnioO_OmYn4_rHc5X8BXZ99yEqZbBSYDRKRQcrLa2xrFADwrQfJVgLaOI8_KMI-ug)

Exemple de configuration de la table

![](https://lh5.googleusercontent.com/g0JJMjqIOYRh4ZQqEAwCNrXiM2vMdCXxM0PnJrE8JcuG_eo2PGjkx4Qj5jdueIsceBBOKe4wRQRmPfxfRVPZYPpCD-_1yBT80uOYVC3GKPpYstJQ3EHJsWzF10eyI4xbc0YtGqxFe6ZDPaL7TkSgYRs)![](https://lh5.googleusercontent.com/hOMRNJ-oN4EI4UO95U7bM9idbldn72zGFVCYWtYiSCSR-JpIWHtKn7XZ6g4SDoEl_BNiAjHmYzDMVrfbKt10bij9_nOnY2bYRe3QOR3LRmOtKiPnxfuMOoEWQQk94bkPulINiWWAxhjTBNZpRKmftlY)

Rendu après configuration de la table

![](https://lh4.googleusercontent.com/TlmfoXo7q2HmqbtFJoKl0RYdxDMUlD1_esqOUleSdhr0JvhetsW7EzZxB6q7MAXFH7aiG8Dq4bngxeP1pzLCXYRdxCWf64OGOiCN5KjW_72AtUXcfCqByx_uHEuLvQ2I6BxMek6bilsLZ0eUjZ9HyMc)

Ajouter des données au texte

![](https://lh4.googleusercontent.com/1RZu8zXfyj2H5iFQXuxk14QdSp1r6pPa_9w9Mz83vcdJzwsDIA8VK2F_nfXVwf7QwOnszSGOdra2pNfobxec2lb3FhrpKWzdh-_fq6TM1MGNpEL3XsmpkzZzxPnUpSWe_MgjRsM45Bw5ZhXZi-6SYg8)

Injecter des données statistiques dynamique au texte

Cliquez sur le texte et sur l’icône Base de données au dessus de la boîte de texte

![](https://lh6.googleusercontent.com/9rFkEJt3iURJmsT3A4vQkuXUYgn6X-67TTjkeZ__mIidCWjugUZenKZXUX4keSgbxdqJuWQWpFP2o7je_vOiDFiIfMYBxv9U6UPhD8osVz8KC9R5hcRkKD6eIr8dih_rCeiX6qRfqj3M9fqGKu5J2hs)

Ajoutez la somme par départ et arrivée dans les boites respectives

![](https://lh4.googleusercontent.com/r4uMymCzd9AOgkCtOje84HFqi5D1DcoZV9WYtsQiYP6x7Obam3nA-AQ32QmeWlOt6VQSw-gCbLCjlfYxn0g4EKzRtXxgxPgSiM38lC_dO0uYVUe_bqPUAPUctQX4b7WScfUkUVqROEHm998V6K2K0E8)

Enregistrer et publier

![](https://lh6.googleusercontent.com/v_t8NE4eveJBPRuexsalzDJTF6_AwJL0YAC572RBG0mzp1k-Of3_-umzErwOYG_BfPmual34wq7_gvt5KMoF0HpBlLby6pWHRp4LLGbZdK_ePitlCXk_wfxcS1ML5sDkOnznytxcYLYNNGThwFijQk4)


# 


# Mise à jour des données avec FME

Dans le même FME que précédemment :


## CSV Reader

<https://sitewebbixi.s3.amazonaws.com/uploads/docs/20220108-donnees-ouvertes-816bd4.zip>

On remplace la source de juillet par la source d'août

![](https://lh3.googleusercontent.com/keXMnQ5tJY99R9vqUza7TVK_2Wwk4ZtteOks-f4i-7bsvn9LGEXI1WQ17W7HUD2UZ2ctadQn5BkRuk1_sH8wNebgW7Fx1o_eUfzJPNrD0Ltg1f8-42xP5ch7hmyl1rf8e7HMKXbEOkC80ezOGMzRjlU)


## AGOL Reader

![](https://lh6.googleusercontent.com/hwscRoixA_udhzSEiTfHN7k0PQ65qsVqs5SwRL_i0R6kd-6-1l4sTmk2gMgZHPJ_ls7BLZUR8ZqGsBmCt9g1E7RB2Iuk6GILSOYocuUa4JdjwAzmwlBoLxPp8pYgHP06eXt_jw1_HE4NdDT-AIwfJtc)

![](https://lh4.googleusercontent.com/z0DcwldD5Xwb_53NxtJCJCEf8e5BFxAO9mAvGjrtDoxKD_iRHEBmOSATVLHMCHgBVMez4szGFpCG1zwL2QLK8NLRUSMXaB926mVrHg8YiHTqjAbBe7XDjWQSiRuNsul0aAVkPDFd6JYeDgOYeqazLP4)


## ChangeDetector

![](https://lh4.googleusercontent.com/X5kpKgEvGtN4CIsmH-w5f6rQe2Ix3zhviwDkSl7Qr6cwkFWSpEcUEdXkSk_Xy9CDfVdMxZikpFj75e5-rVaxJgHLUWazhPEZuKPFAx9ZAAGdVWmcrOYqMnTAUf2uw2EcU7f5067BOCjBWOWjEVTfX0c)


## AttributeManager

![](https://lh6.googleusercontent.com/pFKmA9_Gxf3QAL1Iz3LC4ZgVEcyXLyDM1mFTOV-HzyJseFZONDvBcM73oHVAjBhG1YlgcNU8ny6IhExsKztGXDK9tuU4Bzf-_Nze9luSeNof9bWkDIiSnzZfkiBH_OBhV5wjfmCJlInwiSs4Xqb8g-Y)




## AGOL Writer

![](https://lh4.googleusercontent.com/oCsizwdo6JHMjcxr45cVE8LO8kEEwp2iCa9JrYow17iowt86xlrc3IQZXotbUC2qjrftkEuOxQWjM5qDg6vUVsRYabxBWrvMEywPqbVYJqUndvlbpL2Yaon03wrEwmKiLwSgYc1DTlvGscpWFJAY-cM)![](https://lh6.googleusercontent.com/Mho82OarVzjbaxBq5Xib5ADllIYbvL_XykmuPMrF0zZ23G2LCLuYriE_0nunVBbIDjXUsZDzqZqGB2UDqaGLBLVtK8VGFY-mS6rlkLBlj5Ag74NOjP372mA4RojFdVL4C4fFm9dZEVOA3X0NhpXk5l0)

  


![](https://lh3.googleusercontent.com/dxipnsW9FKzNbTXW91F7aU0_EuRCqBvrH1sBm1JGHMfl8eUzQfnQFs7wxU1IoSuCwjyX8-g_zgk8lnwgm-jdnRuEhFkY6-fRNhM5dZJTdAVqbCI50EYQVfn5n08zqtkQCOfeOPJpSaF1StwTKAqf0MU)
