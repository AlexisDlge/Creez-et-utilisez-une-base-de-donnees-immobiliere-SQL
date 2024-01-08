# Creez-et-utilisez-une-base-de-donnees-immobiliere-SQL
Projet 3 de la formation de data analyst de OpenClassrooms

<img width="614" alt="IMG_Scenario" src="https://github.com/AlexisDlge/Detectez-des-faux-billets/assets/152527939/6c949932-3da9-4faa-a408-3d3da4ec7247">

Vous êtes data analyst chez Laplace Immo, un réseau national d’agences immobilières. Le directeur général est sensible depuis quelque temps à l’importance des données, et il pense que l’agence doit se démarquer de la concurrence en créant un modèle pour mieux prévoir le prix de vente des biens immobiliers. 

<img width="614" alt="Logo_LaplaceImmo" src="https://github.com/AlexisDlge/Creez-et-utilisez-une-base-de-donnees-immobiliere-SQL/assets/152527939/65867700-8bde-4af2-85af-4d3bdaa738cc">

Ce projet stratégique est appelé en interne le projet « DATAImmo ». La CTO de l’entreprise, Clara Daucourt, a la responsabilité de conduire le projet.
Dans ce cadre, elle vous a confié la modification de la base de données permettant de collecter les transactions immobilières et foncières en France. Vous utiliserez ensuite cette base pour analyser le marché et aider les différentes agences régionales à mieux accompagner leurs clients.
À votre arrivée ce matin, vous avez reçu un e-mail de la part de Clara, qui donne plus de détails sur ce qui est attendu de votre part.

    Objet : Réunion de validation – Modification de la base de données.
    De : Clara
    À : Moi

    Hello, 
  
    Afin d’avancer sur le projet DATAImmo, je prévois une première réunion pour valider la modification de la base de données.
    Tu trouveras en pièce jointe un fichier zip avec les données suivantes :
      ● des données extraites du site open data des Demandes de valeurs foncières (DVF) ;
      ● des données de l’INSEE avec les résultats des recensements de la population ;
      ● des données de data.gouv sur les régions, avec le référentiel géographique français, 
        communes, unités urbaines, aires urbaines, départements, académies, régions.

    D’ici la réunion, j’aurais besoin de 2 choses de ta part : 

      ● Il faut que tu prépares le dictionnaire des données en respectant le template en PJ pour répertorier et décrire
        les données importantes à stocker car nous avons omis de le faire. Il faut le remplir pour les trois fichiers de données.
      ● Ensuite, peux-tu modifier le schéma relationnel en pièce-jointe pour qu’il prenne en compte les nouvelles données
        région et population ? Ça nous permettra de bien visualiser les différentes entités, associations et cardinalités de la base
        de données. Enfin, il faudra que tu me présentes ce nouveau schéma relationnel normalisé (Il doit suivre la norme 3NF) 
        de la base de données qui donnera lieu à la création des nouvelles tables. 

    On validera tout ça ensemble lors de notre réunion de validation, pour que tu puisses avancer sur la création de la base.

    Je reste à ta disposition en cas de besoin.

    Bien à toi,
    Clara Daucourt
    CTO
 
    Pièces jointes : 
      Template du dictionnaire des données
      Les données
      Le schéma relationnel à recréer et modifier 

**Données :**
* [Template du dictionnaire des données](https://s3.eu-west-1.amazonaws.com/course.oc-static.com/projects/DAN_V2_P3/Template_dico_donne%CC%81es.xlsx)
* [Les données](https://s3.eu-west-1.amazonaws.com/course.oc-static.com/projects/DAN_V2_P3/Donne%CC%81esImmo.zip)
* [Le schéma relationnel à recréer et modifier](https://s3.eu-west-1.amazonaws.com/course.oc-static.com/projects/DAN_V2_P3/Sche%CC%81ma_a%CC%80_comple%CC%80ter.jpg)

<img width="614" alt="IMG_EnonceProjetSQL" src="">  

Une fois cette première partie de votre travail effectuée, vous présentez votre travail à Clara qui valide votre schéma relationnel ainsi que le dictionnaire des données. 
À ce stade du projet, vous pouvez valider avec votre mentor que votre conception est correcte avant d’aller plus loin.
Félicitations ! Elle vous envoie un e-mail à la suite de cette réunion.

    Objet: Validation du schéma relationnel et suite du projet
    De : Clara
    À : Moi

    Hello,

    Félicitations pour cette première étape de conception ! Comme on en a parlé en réunion ce matin, on est bons pour partir sur la modification de la base de données. Il faut maintenant que tu implémentes les tables dans la base de données en respectant ce       qu’on s’est dit ce matin (cf. compte rendu de réunion en pièce jointe).

    On a échangé en interne, et on pense qu’un outil comme SQLite est pertinent pour ce type d’implémentation. Si tu es plus à l’aise, tu peux essayer d’implémenter un outil comme mySQL ou postgreSQL.

    Une fois que tu auras fait ça, tu pourras faire les requêtes pour extraire les données dont nous avons besoin. Pour ça, envoie-moi un document PDF avec tous les résultats des requêtes ainsi que la requête associée. Utilise des alias pour que ça soit plus      lisible. Tu trouveras toutes les demandes auxquelles il faudra répondre dans le CR de réunion.

    Une fois que tu auras terminé, on regardera tout ça ensemble pour voir ce que tu as réussi à tirer comme données.

    Bon courage !

    Clara Daucourt
    CTO
 
    Pièce jointe : 
        Compte-rendu de réunion

**Données :**
[Compte-rendu de réunion](https://s3.eu-west-1.amazonaws.com/course.oc-static.com/projects/DAN_V2_P3/CR_re%CC%81union.pdf)
