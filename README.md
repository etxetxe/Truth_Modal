# 🎮 Titre du jeu : Truth Modal

En posant le constat inquiétant que l'actualité en flux continu influence les politiques, même lorsqu'elle est fausse, cette expérience XR souhaite faire prendre connaissance au spectateur de ses propres biais d'interprétation de l'information au travers d'une expérience narrative en réalité virtuelle.

![image](https://github.com/etxetxe/VR_Bifurcation/blob/main/Firefly_First-person_mixed_reality_experience_filmed_from_the_player's_perspective_using_Meta_Quest_.gif)

## 🎯 Objectif du joueur

Dans un environnement XR immersif, le joueur doit attraper, trier et stocker des objets virtuels représentant des informations. Chaque objet possède des caractéristiques spécifiques (poids, durée de vie, type) et peut être véridique ou faux. Le joueur doit optimiser ses décisions pour éviter la surcharge et maximiser le bon stockage d’objets avant la fin du temps imparti (10 minutes).

### ✅ Objectifs pédagogiques ou émotionnels possibles

- Apprendre à gérer la surcharge d'information
- Hiérarchiser les priorités rapidement
- Explorer le concept de filtrage mental ou émotionnel
- Stimuler la prise de décision sous stress
- Sensibiliser aux biais cognitifs et à la désinformation

## ⏱️ Durée & rythme

- **Durée** : 10 minutes
- **Rythme croissant** : les objets apparaissent plus vite au fil du temps
- **Tension narrative** : le joueur doit trier sous pression, ce qui simule le stress cognitif ou décisionnel

## 📊 Feedback et évaluation

### En temps réel :
- Changements de couleur ou de forme des objets en fonction des décisions du joueur.
- Sons spécifiques associés aux bonnes ou mauvaises décisions.
- Vibrations ou autres retours haptiques pour renforcer l'immersion.

### Fin de l'expérience :
- Tableau de bord présentant :
  - Nombre total d'objets traités.
  - Taux de bonnes décisions.
  - Temps moyen de réaction.
  - Analyse des biais cognitifs détectés.

## ⚙️ Mécaniques de jeu (gameplay loop)

![image](https://github.com/etxetxe/VR_Bifurcation/blob/main/Truth_Modal_Schema.png)

### 1. Phases du jeu

- **Play → Game → End**  
  Le jeu commence avec un lancement manuel (“Play”).  
  Le joueur entre en phase d’activité (“Game”) où il interagit activement avec les objets.  
  La fin (“End”) est conditionnée par le temps, ou par la capacité de stockage atteinte.

### 2. Système d’objets

- **Zone de spawn** : Les objets apparaissent à intervalles réguliers.
- Chaque objet a :
  - Une durée de vie (temps avant disparition)
    - Type 1 : 5 sec
    - Type 2 : 2,5 sec
    - Type 3 : 10 sec
  - Un poids (type 2 > type 1 > type 3)
  - Un type identifiable visuellement (forme, texture, couleur)
  - Un statut : véridique (à stocker) ou faux (à rejeter)

#### Interactions possibles :
- Attraper un objet (grab)
- Le déplacer (drag & drop)
- Le stocker (dans la zone prévue)
- Le laisser disparaître (erreur ou choix tactique)

### 3. Zone de stockage

Les objets doivent être placés dans une zone de stockage avec collision.  
Elle a une capacité limitée dépendant de :
- La taille des objets
- Leur quantité accumulée

Si trop d’erreurs ou dépassement → fin prématurée ou pénalité.
