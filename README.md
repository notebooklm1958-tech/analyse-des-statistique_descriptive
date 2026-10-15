# analyse-des-statistique_descriptive
https://youtu.be/MBDtWcDk9Ic

**Résumé du fichier `statistique_descriptive.ipynb`**

**Nature du document** : notebook Python de 106 cellules (code + commentaires en français) qui réalise une analyse statistique descriptive du jeu de données **Fortune 500 (2019)**. Le code est retranscrit d'une vidéo YouTube. Les cellules ne sont **pas exécutées** : aucun résultat chiffré n'y figure.

**Prérequis** : le fichier `fortune500-2019.csv` doit être placé dans le même dossier. Il n'est pas fourni, donc le notebook ne peut pas tourner en l'état.

**Structure (26 sections)**

1. **Préparation (sections 1 à 3)** : import de pandas, NumPy, Matplotlib et Seaborn, désactivation des avertissements, chargement du CSV dans un DataFrame.
2. **Exploration générale (4 à 10)** : dimensions (`shape`), aperçu (`head`), structure (`info`), valeurs manquantes (`isnull().sum()`), et `describe()` pour les colonnes numériques, textuelles, puis toutes.
3. **Mesures de tendance centrale (11 à 13)** : moyenne, médiane et mode de la colonne `revenue ($ millions)`.
4. **Mesures de dispersion (14 à 22)** : minimum, maximum, étendue, variance, écart-type, quartiles Q1/Q2/Q3 et écart interquartile (IQR).
5. **Visualisation et forme de la distribution (23 à 26)** : boxplot, asymétrie (skewness), histogramme avec courbe de densité (KDE), aplatissement (kurtosis).

**Conclusions annoncées (commentaires, non vérifiées par des résultats)** : la distribution du chiffre d'affaires serait fortement asymétrique à droite, avec de nombreuses valeurs aberrantes et des queues épaisses (quelques géants dominent un grand nombre d'entreprises plus petites).

**Points d'attention**
- Une erreur dans le commentaire de la section 17 : la variance est décrite comme mesurant la dispersion autour de la « moyenne géométrique », alors qu'il s'agit de la moyenne arithmétique.
- `sns.distplot` est obsolète dans les versions récentes de Seaborn. Le notebook propose `sns.histplot(..., stat='density', kde=True)` en remplacement.
- Les interprétations sont rédigées d'avance (par exemple « généralement détenu par Walmart ») : elles restent à confirmer une fois le CSV chargé et les cellules exécutées.

Si vous me fournissez le CSV, je peux exécuter l'analyse et vous donner les vrais résultats.
