# Projet : Analyse de la mortalité en France métropolitaine

##  Objectif du projet
Ce projet vise à analyser les **déterminants de la mortalité** en France métropolitaine, à partir d’une approche économétrique appliquée et visualisée via **RStudio**.

La problématique étudiée est la suivante :

> *Quelle est l'influence de la densité des médecins et du nombre d'établissements hospitaliers par département sur le taux de mortalité ?*

##  Données utilisées
Les données proviennent de l’**INSEE** et couvrent :
- Le **nombre de médecins** par département
- Le **nombre d’établissements hospitaliers**
- Le **taux brut de mortalité** par département
- Des variables de contrôle issues du recensement (âge, population…)

##  Méthodologie
- Régression économétrique (modèle log-linéaire)
- Tests statistiques : hétéroscédasticité, autocorrélation (Durbin-Watson, Breusch-Godfrey)
- Correction des biais : méthode **Cochrane-Orcutt** pour l’autocorrélation
- Comparaison de plusieurs modèles (linéaire, log-linéaire, log-log)

##  Résultats clés
- ✅ Une **augmentation de 1% du nombre de médecins** réduit le taux de mortalité de **230 unités**
- ❗ Le nombre d'établissements hospitaliers est **positivement corrélé** avec la mortalité : ce paradoxe soulève des hypothèses structurelles (sous-effectif, hôpitaux en zone à risque…)
- ⚠️ Problèmes d'endogénéité, de petite taille d'échantillon (94 obs.) et d'autocorrélation identifiés

##  Visualisations
Le projet propose plusieurs graphiques interactifs construits avec **ggplot2**, **plotly**, etc. :
- Cartes de densité
- Boxplots comparatifs
- Graphiques temporels


##  Limites & Perspectives
- Multicolinéarité possible entre variables explicatives
- Spécification du modèle à affiner
- Nécessité d’inclure des variables socio-économiques, données sur l’accès aux soins, etc.

## Auteur
**Selim Dridi** – Université de Strasbourg  
Projet réalisé dans le cadre du cours d’économétrie appliquée / visualisation RStudio

---

