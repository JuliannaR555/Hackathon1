# Hackathon1
Hackathon - Analyse des Dépenses Médicales

Ce projet a été réalisé dans le cadre du Hackathon IA & Data Science - Week 3 du GenAI Bootcamp.
Il vise à analyser les facteurs influençant les charges médicales individuelles aux États-Unis, à partir du dataset insurance.csv.
Structure du projet

    hackaton_reworked.ipynb → Notebook principal contenant toute l'analyse, propre et commentée
    data/insurance.csv → Données d'assurance maladie
    data/healthcare_spending_per_capita_1991_2014.csv → Dépenses médicales par État et par année
    img/ → Dossier optionnel pour y mettre les visuels importants (graphiques, captures, etc.)

Objectifs

    Identifier les facteurs qui influencent le plus les charges médicales
    Étudier l'impact de variables telles que :
        Le tabagisme (smoker)
        L'IMC (bmi)
        Le nombre d’enfants (children)
        La région (region)
    Fusionner avec un second dataset pour explorer le lien avec les dépenses de santé régionales (dépenses par habitant en 2010)

Méthodologie

    Analyse exploratoire des données (EDA)
    Visualisations avancées (Boxplot, Heatmap, Stripplot, etc.)
    Corrélations simples et croisées
    Création de variables combinées (ex: bmi * smoker)
    Tests statistiques (test t entre régions)
    Fusion avec données macro (spending per capita) via regroupement par grande région

Résultats clés

    Le facteur tabagisme est de loin le plus corrélé aux charges médicales.
    L’IMC, l’âge, et leurs interactions avec le tabagisme renforcent fortement l’explication des coûts.
    Les familles avec 4 enfants ont montré un outlier, lié à un individu âgé et en surpoids.
    Les régions du Sud-Est et Sud-Ouest affichent les plus fortes charges moyennes.
    Une légère correspondance est observée entre les régions à fortes dépenses globales et celles aux charges élevées, bien que les deux sources soient différentes.

Comment exécuter
Cloner ce repo :

git clone https://github.com/Jeynova/hackathon_insurance_analysis.git
cd hackathon_insurance_analysis
