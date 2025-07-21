# Analyse du Speed Dating Tinder

## Contexte
Tinder est une application de rencontres en ligne où on “swipe à droite” pour aimer ou “swipe à gauche” pour passer un profil.

L’équipe marketing constate une baisse des correspondances et veut identifier ce qui suscite l’intérêt mutuel.

Ils ont donc organisé une expérience de speed dating en 21 vagues, chaque participant rencontrant tous les autres membres de sa vague pendant 4 minutes.

## Jeu de données
Chaque ligne du fichier correspond à une interaction de speed dating entre deux partenaires. Les colonnes incluent :
- Informations démographiques (âge, revenu, genre)
- Évaluations sur six attributs
- Consentement pour un second rendez-vous
- Questionnaires pré et post-événement


## Résultats
Le notebook génère :
- Statistiques descriptives par genre et attribut
- Corrélations entre évaluations et seconde invitation
- Comparaison entre perception personnelle et perception des autres
- Analyse temporelle de l’ordre des rendez-vous
- Visualisations interactives via Plotly

## Nettoyage et prétraitement
- Filtrage des IDs partenaires manquants
- Conversion du revenu en format numérique
- Recodage des variables et correction des incohérences
- Ajout de colonnes de différence d’âge et de revenu entre partenaires
- Agrégation par participant pour réduire le biais lié au nombre de rencontres par vague

## Insights clés
- Les deux genres surestiment l’importance de l’attractivité et sous-estiment les intérêts communs et l'humour.
- Attractivité, intérêts partagés et fun sont les meilleurs prédicteurs d’une décision positive.
- Les matchs sont maximisés lorsque la différence d’âge est faible, et plus de décisions positives se produisent quand le partenaire est plus jeune.
- Les habitués des sorties obtiennent plus de secondes invitations et génèrent davantage de matchs.
- Le premier et le dernier speed dates offrent un léger avantage de seconde invitation par rapport aux positions intermédiaires.

## Solutions proposées
- Favoriser les mises en relation avec une faible différence d’âge.
- Mettre en avant l’importance des centres d’intérêts partagés et du sens de l’humour aux côtés de l’attractivité.
- Offrir un programme d’entraînement pour instaurer de bonnes habitudes de rendez-vous.
- Ajuster les algorithmes pour corriger la surestimation des auto-évaluations.
- Limiter simultanément à deux le nombre de propositions de speed dates.
