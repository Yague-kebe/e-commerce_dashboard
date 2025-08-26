# E-commerce Anomaly Detection Dashboard
Ce projet est un tableau de bord interactif en une seule page (HTML, CSS, JavaScript) conçu pour l'analyse et la détection d'anomalies dans les données de transactions e-commerce. Il permet aux utilisateurs de télécharger un fichier CSV, d'analyser les données, de visualiser les indicateurs clés de performance (KPI), et d'identifier les anomalies dans les commandes.

## Démonstration vidéo
 [Télécharger la vidéo de démonstration](./demo.mp4)

## Fonctionnalités principales
-   Chargement de fichiers **CSV** (via
    [PapaParse](https://www.papaparse.com/))
-   Détection automatique :
    -   Prix incohérents: valeurs négatifs, zéros, anomalies
        statistiques
    -   Quantités (Valeurs nulles, négatives ou excessivement élevées).
    -   Format de données: Données manquantes, emails malformés, dates incorrectes, incohérences de catégories.
    -   Doublons: Identification des entrées dupliquées
-   KPIs en temps réel (CA total, commandes, anomalies détectées...)
-   Graphiques interactifs ([Chart.js](https://www.chartjs.org/)) :
    -   Évolution des ventes
    -   Répartition par pays
    -   Heatmap anomalies **(catégories × statuts)**
-   Tableau dynamique filtrable, triable et paginé
-   Export des données propres en **CSV**

## Guide d'utilisation
### 1. Cloner le dépôt
utilisez votre cmd avec github installer de base

git clone https://github.com/<ton-username>/ecommerce-anomaly-dashboard.git

cd ecommerce_dashboard

### 2. Lancer l'application

Pas de backend ni dépendances :\
 Ouvrez `index.html` dans un navigateur moderne.

### 3. Charger vos données

-   Cliquez sur **"Charger le fichier CSV"**\
-   Analysez anomalies & graphiques\
-   Exportez les données propres

# Format du fichier CSV
Le tableau de bord est conçu pour analyser des données avec les en-têtes de colonnes suivants. Assurez-vous que votre fichier CSV inclut ces colonnes pour un fonctionnement optimal : order_id,order_date,customer_id,customer_email,customer_age,product_name,category,price,quantity,total_amount,country,payment_method,order_status
ORD10582,2024-02-16,CUST0615,user18@gmail.com,57,Vacuum Cleaner,Electronics,610.39,4,2441.56,Netherlands,PayPal,Delivered

## Structure du projet
ecommerce_dashboard/

│── index.html # Interface Web Interactive (React-style avec Vanilla JS)

│── README.md # Documentation

│── demo.mp4 # Vidéo de démonstration 
