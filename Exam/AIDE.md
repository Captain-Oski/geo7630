
Vérifier que tout est bien enregistré et que votre branche actuelle est "commitée et poussée"
Vérifier que vous avez bien le upstream : 
- git remote -v

0. git remote add upstream https://github.com/Captain-Oski/geo7630.git
Ensuite :

1. git checkout main
2. git pull upstream main
3. git checkout -b exam 1
4. On vérifie qu'on a bien le README.md avec les informations nécessaires et le dossier FME
5. on ouvre FME pour créer un nouveau projet intitulé : code_ms.fmw
6. on enregistre le fmw dans le repertoire du git
7. losrque terminé et prêt à soumettre: 
8. 1. git commit -m 'mon message personnalisé'
8. 2. git push -u origin main