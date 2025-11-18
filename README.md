🌍 Power BI – Carte géopolitique & météo en temps réel

Ce projet présente une carte interactive mondiale, intégrant des données géopolitiques, démographiques et météorologiques en temps réel, entièrement développée dans Power BI.
Il démontre l’utilisation combinée d’APIs, de transformations avancées Power Query, d’un modèle de données étoilé et de mesures DAX dynamiques.

🚀 Fonctionnalités principales
🗺️ Carte interactive mondiale

Carte choroplèthe colorée dynamiquement selon la métrique choisie
(population, superficie, température, vitesse du vent…)

Zoom & navigation fluide

Infobulle personnalisée au survol de chaque pays

🔎 Filtres interactifs

Continent

Langues

Météo actuelle

Filtre de température (réglette)

🌦️ Météo en temps réel

Appel automatisé à l’API Open-Meteo pour chaque pays

Température, vitesse du vent, direction, code météo

Icône météo affichée automatiquement via une URL dynamique

🏳️ Drapeaux des pays

URL générée automatiquement via flagpedia / flagcdn

Affichage du drapeau dans les infobulles (visuel Simple Image)

🧪 Data processing avancé (Power Query)

Intégration API RestCountries

Nettoyage et extraction des champs complexes

Dé-pivotage des listes (langues, continents…) dans des tables dédiées

Construction d’un modèle en étoile

📐 DAX avancé

Mesure dynamique SelectedMetricValue pilotée par un segment utilisateur

Concaténation de valeurs multiples via CONCATENATEX

Mesures propres pour les infobulles (météo, géopolitique)

🛠️ Technologies utilisées

Power BI Desktop / Service

Power Query (M)

DAX

APIs externes :

RestCountries : données géopolitiques

Open-Meteo : météo en temps réel

Flagpedia : drapeaux des pays

📁 Sources API

🌍 RestCountries
https://restcountries.com/v3.1/all?fields=name,cca2,currencies,capital,languages,translations,latlng,area,population,continents

🌦️ Open-Meteo (exemple)
https://api.open-meteo.com/v1/forecast?latitude=LAT&longitude=LONG&current_weather=true

🏳️ Flagpedia
https://flagcdn.com/160x120/{CCA2}.png

📊 Modèle de données

Modèle en étoile incluant :

Table principale (Pays)

Tables de dimension :

Langues

Continents

Monnaies

Codes météo

Relations en 1→N filtrant la table principale

🎨 Pages du rapport
1. Carte principale

Carte choroplèthe

Segments de filtrage

Sélecteur de métriques

Mise en forme sombre (#121526 / #161C32 / #262D45)

2. Infobulle personnalisée

Informations socio-démographiques

Données météo

Drapeau et icône météo dynamiques

Visuels KPI épurés

📌 Améliorations futures

Publication sur Power BI Service

Actualisation automatique via Power BI Pro

Inclusion d’autres APIs (indicateurs économiques, indices de développement…)

Ajout d’une timeline météo

📜 Licence

Projet librement réutilisable à des fins éducatives.
