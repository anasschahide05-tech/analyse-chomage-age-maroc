# Catalogue pédagogique — 40 projets de Data Science appliquée au commerce international

**Public :** licence avancée / master en commerce international, gestion ou management. **Groupes :** binômes. **Durée :** 14 jours, 20–30 heures. **Outils :** Python, pandas, scikit-learn, matplotlib, Google Colab. **Édition :** 29 octobre 2026.

> **Transparence des sources.** Les pages documentaires officielles UN Comtrade, Banque mondiale et OMC ont été contrôlées le 29/10/2026. Les 40 combinaisons pays–produit–année ne sont **pas** validées individuellement par un téléchargement complet. Les liens du portail LPI et UNCTAD désignent des catalogues, pas des fichiers directs. Les **dimensions réelles ne sont pas déterminables avant extraction** et doivent être calculées par les étudiants. Les endpoints sont documentés, mais la disponibilité des séries, les quotas d'API et les millésimes doivent être vérifiés au jour du TP. Les points non vérifiés sont signalés dans les fiches. Ne pas confondre les 500 lignes preview Comtrade avec la population totale.

## Partie A — Tableau des 40 projets

| N° | Sujet | Domaine | Type | Niveau | Source |
|---:|---|---|---|---|---|
| 1 | Prévision des exportations marocaines par produit | Export et marchés | Régression temporelle | Intermédiaire | COM |
| 2 | Importations marocaines de céréales | Export et marchés | Régression temporelle | Intermédiaire | COM |
| 3 | Solde commercial du Maroc | Export et marchés | Régression temporelle | Intermédiaire | COM |
| 4 | Échanges Maroc–France | Export et marchés | Régression temporelle | Intermédiaire | COM |
| 5 | Prix internationaux des matières premières | Export et marchés | Régression temporelle | Intermédiaire | WB |
| 6 | Recettes d’exportation en dirhams | Export et marchés | Régression temporelle | Avancé | COM+WB |
| 7 | Demande espagnole de produits marocains | Export et marchés | Régression temporelle | Intermédiaire | COM |
| 8 | Commerce international de services | Export et marchés | Régression temporelle | Intermédiaire | WB |
| 9 | Connectivité maritime et commerce | Logistique et macroéconomie | Régression sur panel | Avancé | UNCT+WB |
| 10 | Coûts du commerce et infrastructure | Logistique et macroéconomie | Régression sur panel | Avancé | LPI+WB |
| 11 | Taux de change et importations | Logistique et macroéconomie | Régression temporelle | Intermédiaire | WB |
| 12 | Exportations agroalimentaires marocaines | Export et marchés | Régression temporelle | Intermédiaire | COM |
| 13 | Marchés à croissance d’importations élevée | Export et marchés | Classification binaire | Intermédiaire | WB |
| 14 | Produits à potentiel exportateur | Export et marchés | Classification binaire | Intermédiaire | COM |
| 15 | Alerte sur une chute d’exportations | Export et marchés | Classification binaire | Avancé | COM |
| 16 | Profils de croissance des partenaires | Export et marchés | Classification multiclasse | Intermédiaire | COM |
| 17 | Vulnérabilité des marchés étrangers | Export et marchés | Classification binaire | Avancé | WB |
| 18 | Sensibilité des flux aux tarifs | Export et marchés | Classification binaire | Avancé | WTO+COM |
| 19 | Ralentissement du commerce extérieur | Export et marchés | Classification binaire | Intermédiaire | WB |
| 20 | Secteurs exportateurs émergents | Export et marchés | Classification binaire | Avancé | COM |
| 21 | Segmentation des marchés mondiaux | Export et marchés | Clustering | Intermédiaire | COM |
| 22 | Segmentation des partenaires du Maroc | Export et marchés | Clustering | Intermédiaire | COM |
| 23 | Familles de produits exportés | Export et marchés | Clustering séries | Intermédiaire | COM |
| 24 | Cartographie des échanges internationaux | Export et marchés | Réduction dimension | Intermédiaire | COM |
| 25 | Anomalies des flux Maroc–UE | Logistique et macroéconomie | Détection anomalies | Avancé | COM |
| 26 | Mutation de la structure des exportations | Logistique et macroéconomie | ACP + clustering | Intermédiaire | COM |
| 27 | Systèmes logistiques similaires | Logistique et macroéconomie | Clustering | Avancé | UNCT+LPI |
| 28 | Flux internationaux atypiques | Logistique et macroéconomie | Détection anomalies | Avancé | COM |
| 29 | Typologie de compétitivité | Logistique et macroéconomie | ACP + clustering | Intermédiaire | WB |
| 30 | Concentration des fournisseurs étrangers | Logistique et macroéconomie | Clustering | Intermédiaire | COM |
| 31 | Tableau de bord marocain du commerce extérieur | Export et marchés | Visualisation+analyse | Débutant | COM |
| 32 | Avantage comparatif révélé des produits marocains | Export et marchés | Indices+classement | Avancé | COM |
| 33 | Avant/après d’un accord commercial | Export et marchés | Analyse de panel | Avancé | COM |
| 34 | Choix de marchés cibles | Export et marchés | Aide décision multicritère | Intermédiaire | COM+WB |
| 35 | Barrières tarifaires sur un produit marocain | Export et marchés | Analyse descriptive+classement | Intermédiaire | WTO |
| 36 | Performance logistique des pays | Logistique et macroéconomie | Clustering + visualisation | Intermédiaire | LPI |
| 37 | Commerce agricole Maroc–Afrique | Export et marchés | Analyse panel+prévision | Intermédiaire | COM |
| 38 | Veille de changements commerciaux | Export et marchés | Détection alertes | Intermédiaire | COM |
| 39 | Risque de dépendance fournisseurs | Export et marchés | Analyse concentration | Intermédiaire | COM |
| 40 | Recommandation de marchés export | Export et marchés | Recommandation/ranking | Avancé | COM+WB |

## Partie B — Fiches individuelles et consignes

**Consigne commune à chaque projet :** fournir un modèle de référence et au moins deux méthodes (lorsqu’une méthode exploratoire n’est pas prédictive, comparer deux méthodes ou deux paramétrages justifiés) ; réaliser cinq visualisations commentées, valider sans fuite, produire notebook/rapport/soutenance.

### Projet 01 — Prévision des exportations marocaines par produit

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Comment prévoir la valeur annuelle des exportations marocaines d’un groupe de produits ?
- **Tâche précise :** Régression temporelle. **Variable cible / indicateur :** Valeur annuelle exportée à t+1.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc (504), export X, partenaire monde (0), HS2 (cmdCode=07), 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Agréger par année ; harmoniser nomenclature ; créer retards sans futur. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Persistance; Ridge; GradientBoostingRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE, RMSE, WAPE sur années futures ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Fuite temporelle et séries annuelles courtes.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 02 — Importations marocaines de céréales

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Peut-on prévoir la valeur annuelle importée de céréales ?
- **Tâche précise :** Régression temporelle. **Variable cible / indicateur :** Valeur importée t+1.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, import M, partenaire 0, HS 10, 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Vérifier unités, années manquantes, déflation si pertinente. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Persistance; Ridge; RandomForestRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE, RMSE, WAPE ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Confusion valeur et quantité, variation des prix.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 03 — Solde commercial du Maroc

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Comment prévoir le solde des échanges de marchandises ?
- **Tâche précise :** Régression temporelle. **Variable cible / indicateur :** Exports moins imports t+1.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, cmdCode=TOTAL, flux X et M, 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Fusionner X et M, vérifier même unité, lags. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Solde année précédente; Ridge; HistGradientBoostingRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE, RMSE ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Fuite par agrégats construits avec l’année cible.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 04 — Échanges Maroc–France

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Comment anticiper la valeur des échanges bilatéraux ?
- **Tâche précise :** Régression temporelle. **Variable cible / indicateur :** Valeur X ou M à t+1.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, France 251, TOTAL, X/M, années 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Préserver orientation des flux et cohérence temporelle. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Persistance; Ridge; RandomForestRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE, WAPE ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Symétrie imparfaite des déclarations miroirs.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 05 — Prix internationaux des matières premières

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Les cours passés permettent-ils de prévoir une série de prix ?
- **Tâche précise :** Régression temporelle. **Variable cible / indicateur :** Prix mensuel suivant d’une matière première.
- **Jeu de données officiel :** Banque mondiale, World Development Indicators. [Documentation](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://api.worldbank.org/v2/country/mar/indicator/TX.VAL.MRCH.CD.WT?format=json.
- **Extraction exacte à effectuer :** World Bank Pink Sheet : fichier Excel de prix mensuels (page officielle commodity markets). **Format :** JSON/CSV selon la source. **Accès :** JSON API sans clé, peut contenir valeurs manquantes.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Convertir dates, gérer ruptures, isoler chaque matière. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Naïf; Ridge; GradientBoostingRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE, RMSE chronologiques ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Prix nominal versus réel et changements de régime.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 06 — Recettes d’exportation en dirhams

- **Domaine / niveau / compétences :** Export et marchés ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Comment varie la valeur convertie des exportations avec la devise ?
- **Tâche précise :** Régression temporelle. **Variable cible / indicateur :** Recette estimée en MAD de l’année future.
- **Jeu de données officiel :** UN Comtrade + World Bank API. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/ ; https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS ; https://api.worldbank.org/v2/country/mar/indicator/PA.NUS.FCRF?format=json.
- **Extraction exacte à effectuer :** UN Comtrade Maroc export TOTAL + indicateur Banque mondiale PA.NUS.FCRF (MAD/USD, à confirmer par période). **Format :** JSON/CSV selon la source. **Accès :** Deux sources à harmoniser par période.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Aligner années et devises, documenter taux moyen vs transactionnel. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Persistance; Ridge; RandomForestRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE, WAPE ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Conversion comptable confondue avec causalité.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 07 — Demande espagnole de produits marocains

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** La demande extérieure permet-elle de prévoir les exportations d’un produit ?
- **Tâche précise :** Régression temporelle. **Variable cible / indicateur :** Valeur importée par Espagne t+1.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Espagne 724, imports M, partenaire Maroc 504, HS 07, 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Filtrer pays produit, vérifier codes et périodes. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Naïf; Ridge; GradientBoostingRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE, RMSE ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Données miroir non interchangeables.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 08 — Commerce international de services

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Peut-on prévoir une série annuelle d’exportations de services ?
- **Tâche précise :** Régression temporelle. **Variable cible / indicateur :** Exportations de services en dollars t+1.
- **Jeu de données officiel :** Banque mondiale, World Development Indicators. [Documentation](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://api.worldbank.org/v2/country/mar/indicator/TX.VAL.MRCH.CD.WT?format=json.
- **Extraction exacte à effectuer :** Banque mondiale indicateur BX.GSR.NFSV.CD, Maroc, 2000–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API sans clé, peut contenir valeurs manquantes.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Gérer années absentes et transformations log. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Persistance; Ridge; RandomForestRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE, MAPE si cible non nulle ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Échantillon temporel trop court.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 09 — Connectivité maritime et commerce

- **Domaine / niveau / compétences :** Logistique et macroéconomie ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** La connectivité maritime prédit-elle une variation des échanges ?
- **Tâche précise :** Régression sur panel. **Variable cible / indicateur :** Exportations de marchandises t+1.
- **Jeu de données officiel :** UNCTAD + Banque mondiale. [Documentation](https://unctadstat.unctad.org/datacentre/ ; https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://unctadstat.unctad.org/datacentre/ ; https://api.worldbank.org/v2/country/all/indicator/TX.VAL.MRCH.CD.WT?format=json.
- **Extraction exacte à effectuer :** UNCTAD Liner Shipping Connectivity Index (LSCI), pays/année + World Bank TX.VAL.MRCH.CD.WT. **Format :** JSON/CSV selon la source. **Accès :** Données à joindre pays et année.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Jointure pays/année, valeurs manquantes, décalages temporels. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Moyenne pays; Ridge; RandomForestRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE et R² par années test ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Corrélation confondue avec causalité.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 10 — Coûts du commerce et infrastructure

- **Domaine / niveau / compétences :** Logistique et macroéconomie ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Les indicateurs logistiques expliquent-ils les coûts d’importation ?
- **Tâche précise :** Régression sur panel. **Variable cible / indicateur :** Durée d’importation si disponible ; sinon indicateur LPI cible alternatif.
- **Jeu de données officiel :** LPI + Banque mondiale. [Documentation](https://lpi.worldbank.org/ ; https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://lpi.worldbank.org/ ; https://api.worldbank.org/v2/country/all/indicator/IC.IMP.DURS?format=json.
- **Extraction exacte à effectuer :** LPI par pays et millésime + indicateur BM IC.IMP.DURS (vérifier disponibilité pays/années). **Format :** JSON/CSV selon la source. **Accès :** Indicateur import IC.IMP.DURS à vérifier avant affectation.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Fusionner millésimes, standardiser, filtrer observations. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** DummyRegressor; Ridge; RandomForestRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE, RMSE sur années/pays tenus à part ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Discontinuité des millésimes LPI.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 11 — Taux de change et importations

- **Domaine / niveau / compétences :** Logistique et macroéconomie ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Peut-on prévoir le montant des importations compte tenu des variations monétaires ?
- **Tâche précise :** Régression temporelle. **Variable cible / indicateur :** Valeur importée de l’année suivante.
- **Jeu de données officiel :** Banque mondiale, World Development Indicators. [Documentation](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://api.worldbank.org/v2/country/mar/indicator/TX.VAL.MRCH.CD.WT?format=json.
- **Extraction exacte à effectuer :** Maroc : PA.NUS.FCRF et TM.VAL.MRCH.CD.WT, données annuelles. **Format :** JSON/CSV selon la source. **Accès :** JSON API sans clé, peut contenir valeurs manquantes.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Jointure par année et caractéristiques retardées. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Persistance; Ridge; GradientBoostingRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE et WAPE ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Ne pas attribuer causalité au taux de change.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 12 — Exportations agroalimentaires marocaines

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Comment prévoir les exportations d’agrumes par marchés ?
- **Tâche précise :** Régression temporelle. **Variable cible / indicateur :** Valeur exportée du couple pays-produit t+1.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, X, partenaires France 251/Espagne 724, HS 08, années 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Regrouper HS4, gérer couverture et fluctuations. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Persistance; Ridge; RandomForestRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE, WAPE ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Saisonnalité absente de données annuelles.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 13 — Marchés à croissance d’importations élevée

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels pays connaîtront une croissance des importations supérieure à un seuil ?
- **Tâche précise :** Classification binaire. **Variable cible / indicateur :** Croissance annuelle future > 10% (seuil pédagogique).
- **Jeu de données officiel :** Banque mondiale, World Development Indicators. [Documentation](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://api.worldbank.org/v2/country/mar/indicator/TX.VAL.MRCH.CD.WT?format=json.
- **Extraction exacte à effectuer :** Indicateur TM.VAL.MRCH.CD.WT pour pays sélectionnés, années 2005–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API sans clé, peut contenir valeurs manquantes.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Créer cible future, imputations sur entraînement, lags. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** DummyClassifier; LogisticRegression; RandomForestClassifier. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** F1 macro, PR-AUC ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Classe construite avec l’information future.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 14 — Produits à potentiel exportateur

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quelles lignes HS connaîtront une croissance forte à l’export ?
- **Tâche précise :** Classification binaire. **Variable cible / indicateur :** Croissance t+1 > 15% (seuil explicite).
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, X, HS2 01–24, partenaire 0, 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Mise en panel produit-année, codes stables. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** DummyClassifier; LogisticRegression; RandomForestClassifier. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** F1, rappel, PR-AUC ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Très petits dénominateurs et volatilité.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 15 — Alerte sur une chute d’exportations

- **Domaine / niveau / compétences :** Export et marchés ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Un produit risque-t-il une baisse annuelle de plus de 20% ?
- **Tâche précise :** Classification binaire. **Variable cible / indicateur :** Baisse t+1 <= -20%.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, X, HS2 01–24, année 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Créer variations et indicateurs de retards. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** DummyClassifier; LogisticRegression; GradientBoostingClassifier. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Rappel, PR-AUC ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Rares événements, dénominateur zéro.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 16 — Profils de croissance des partenaires

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Peut-on classer les partenaires selon l’évolution future du commerce ?
- **Tâche précise :** Classification multiclasse. **Variable cible / indicateur :** Croissance future : négative/stable/forte selon seuils.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, X, partenaires 251/724/276/380/826, TOTAL, 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Panel pays-année, équilibrer classes. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** DummyClassifier; RandomForestClassifier; LogisticRegression. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Macro-F1, matrice de confusion ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Peu d’exemples par pays.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 17 — Vulnérabilité des marchés étrangers

- **Domaine / niveau / compétences :** Export et marchés ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels marchés connaîtront une forte contraction des importations ?
- **Tâche précise :** Classification binaire. **Variable cible / indicateur :** Contraction future des imports > 10%.
- **Jeu de données officiel :** Banque mondiale, World Development Indicators. [Documentation](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://api.worldbank.org/v2/country/mar/indicator/TX.VAL.MRCH.CD.WT?format=json.
- **Extraction exacte à effectuer :** TM.VAL.MRCH.CD.WT, NY.GDP.MKTP.KD.ZG par pays et année. **Format :** JSON/CSV selon la source. **Accès :** JSON API sans clé, peut contenir valeurs manquantes.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Fusion indicateurs pays année, retards, imputations. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** DummyClassifier; LogisticRegression; HistGradientBoostingClassifier. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Rappel, PR-AUC ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Absence de véritable étiquette de choc causal.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 18 — Sensibilité des flux aux tarifs

- **Domaine / niveau / compétences :** Export et marchés ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Les flux d’un produit chutent-ils l’année suivante lorsque les tarifs sont élevés ?
- **Tâche précise :** Classification binaire. **Variable cible / indicateur :** Baisse d’import > 15% l’année suivante.
- **Jeu de données officiel :** OMC + UN Comtrade. [Documentation](https://data.wto.org/en/dataset/wto_ttd ; https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://ttd.wto.org/en/download ; https://comtradeapi.un.org/public/v1/preview/C/A/HS.
- **Extraction exacte à effectuer :** WTO Tariff & Trade Data : ADB droits appliqués HS6/pays/année ; Comtrade flux import HS6. **Format :** JSON/CSV selon la source. **Accès :** Alignement nomenclature HS obligatoire.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Harmoniser HS6, pays et année, taux tarifaire. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** DummyClassifier; LogisticRegression; RandomForestClassifier. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** F1, PR-AUC ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Conflit de classification HS et endogénéité tarifaire.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 19 — Ralentissement du commerce extérieur

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Peut-on détecter un ralentissement des échanges de marchandises ?
- **Tâche précise :** Classification binaire. **Variable cible / indicateur :** Croissance commerce total t+1 < 0.
- **Jeu de données officiel :** Banque mondiale, World Development Indicators. [Documentation](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://api.worldbank.org/v2/country/mar/indicator/TX.VAL.MRCH.CD.WT?format=json.
- **Extraction exacte à effectuer :** TX.VAL.MRCH.CD.WT et TM.VAL.MRCH.CD.WT, pays années. **Format :** JSON/CSV selon la source. **Accès :** JSON API sans clé, peut contenir valeurs manquantes.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Calculer cible postérieure, variables retardées. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** DummyClassifier; LogisticRegression; RandomForestClassifier. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Macro-F1, ROC-AUC ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Fuite temporelle.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 20 — Secteurs exportateurs émergents

- **Domaine / niveau / compétences :** Export et marchés ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quel secteur gagnera en part de marché d’exportation ?
- **Tâche précise :** Classification binaire. **Variable cible / indicateur :** Hausse de part export HS2 > 2 points de pourcentage t+1.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, X, HS2, partenaire 0, 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Normaliser par exportations totales, lags. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** DummyClassifier; LogisticRegression; GradientBoostingClassifier. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** F1, PR-AUC ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Seuil arbitraire et faibles volumes.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 21 — Segmentation des marchés mondiaux

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels groupes de pays ont des paniers d’importation comparables ?
- **Tâche précise :** Clustering. **Variable cible / indicateur :** Aucune : vecteurs de parts par chapitre HS.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Importations pays 504,251,724,276,380,826,840,156 pour HS2 01–24, une année disponible. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Pivoter pays × HS2, parts normalisées, valeurs absentes. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** KMeans; AgglomerativeClustering. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Silhouette, stabilité ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Les zéros peuvent être absence de rapport.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 22 — Segmentation des partenaires du Maroc

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels partenaires ont une structure d’achats proche ?
- **Tâche précise :** Clustering. **Variable cible / indicateur :** Aucune : profils des partenaires.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, X, partenaires européens et africains, HS2 01–24, année disponible. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Normaliser par partenaire, regrouper HS2. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** KMeans; GaussianMixture. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Silhouette, Davies-Bouldin ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Biais dû aux tailles de marchés.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 23 — Familles de produits exportés

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels chapitres HS présentent des profils d’évolution semblables ?
- **Tâche précise :** Clustering séries. **Variable cible / indicateur :** Aucune : vecteurs de croissance par chapitre.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504 X, HS2 01–24, 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Corriger zéros, normaliser séries. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** KMeans; AgglomerativeClustering. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Silhouette, stabilité ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Nomenclatures et séries incomplètes.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 24 — Cartographie des échanges internationaux

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quelle représentation 2D préserve les similarités entre pays exportateurs ?
- **Tâche précise :** Réduction dimension. **Variable cible / indicateur :** Aucune.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Exports vers monde par pays 504,251,724,276,380,826,840,156 et HS2, 2022–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Matrice pays × parts HS2, standardisation. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** PCA; TSNE. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Variance expliquée, trustworthiness ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Distances t-SNE non interprétables globalement.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 25 — Anomalies des flux Maroc–UE

- **Domaine / niveau / compétences :** Logistique et macroéconomie ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quelles observations produit-année sont inhabituelles ?
- **Tâche précise :** Détection anomalies. **Variable cible / indicateur :** Aucune, score d’anomalie.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504 X, partenaires 251/724/276/380, HS2 01–24, 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Taux de variation, log1p, niveaux et lags. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** IsolationForest; LocalOutlierFactor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Stabilité des alertes, inspection top 20 ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Anomalie ne signifie pas fraude.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 26 — Mutation de la structure des exportations

- **Domaine / niveau / compétences :** Logistique et macroéconomie ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Peut-on identifier une rupture du panier d’exportations au fil des ans ?
- **Tâche précise :** ACP + clustering. **Variable cible / indicateur :** Aucune.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504 X, HS2 01–24, monde, 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Parts export par année, normalisation. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** PCA; KMeans; AgglomerativeClustering. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Variance expliquée, stabilité ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Petite taille temporelle.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 27 — Systèmes logistiques similaires

- **Domaine / niveau / compétences :** Logistique et macroéconomie ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels pays ont une connectivité maritime comparable ?
- **Tâche précise :** Clustering. **Variable cible / indicateur :** Aucune.
- **Jeu de données officiel :** UNCTADstat + LPI. [Documentation](https://unctadstat.unctad.org/datacentre/ ; https://lpi.worldbank.org/). **Point d’accès / API :** https://unctadstat.unctad.org/datacentre/ ; https://lpi.worldbank.org/.
- **Extraction exacte à effectuer :** UNCTAD LSCI par pays/année et LPI millésime commun. **Format :** JSON/CSV selon la source. **Accès :** Sélection de séries et millésimes manuelle.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Fusion pays/année, standardiser et imputer. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** KMeans; AgglomerativeClustering. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Silhouette, interprétation ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** LPI disponible à années limitées.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 28 — Flux internationaux atypiques

- **Domaine / niveau / compétences :** Logistique et macroéconomie ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels flux produit-partenaire sont inhabituels ?
- **Tâche précise :** Détection anomalies. **Variable cible / indicateur :** Aucune : score atypicité.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, X, HS2 01–24, principaux partenaires, 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Transformer valeurs, variation annuelle, densité. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** IsolationForest; DBSCAN. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Top alertes et robustesse aux seuils ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Faux positifs liés aux petits volumes.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 29 — Typologie de compétitivité

- **Domaine / niveau / compétences :** Logistique et macroéconomie ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Peut-on classer les pays selon exportations et indicateurs de développement ?
- **Tâche précise :** ACP + clustering. **Variable cible / indicateur :** Aucune.
- **Jeu de données officiel :** Banque mondiale, World Development Indicators. [Documentation](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://api.worldbank.org/v2/country/mar/indicator/TX.VAL.MRCH.CD.WT?format=json.
- **Extraction exacte à effectuer :** TX.VAL.MRCH.CD.WT, NY.GDP.MKTP.CD, SP.POP.TOTL, pays année 2022. **Format :** JSON/CSV selon la source. **Accès :** JSON API sans clé, peut contenir valeurs manquantes.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Ratios par PIB/habitant, standardisation. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** PCA; KMeans; GaussianMixture. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Silhouette, interprétabilité ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Variables fortement corrélées.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 30 — Concentration des fournisseurs étrangers

- **Domaine / niveau / compétences :** Logistique et macroéconomie ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels marchés importateurs dépendent d’un petit nombre de fournisseurs ?
- **Tâche précise :** Clustering. **Variable cible / indicateur :** Aucune : indices concentration HHI.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Imports M de pays 504/251/724/276/380 pour HS10, par partenaire, 2022–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Parts fournisseurs, HHI, top fournisseur. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** KMeans; AgglomerativeClustering. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Silhouette, stabilité ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Données partenaires incomplètes.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 31 — Tableau de bord marocain du commerce extérieur

- **Domaine / niveau / compétences :** Export et marchés ; Débutant ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels sont les principaux déséquilibres par produit et partenaire ?
- **Tâche précise :** Visualisation+analyse. **Variable cible / indicateur :** Aucune : KPIs.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, X et M, HS2 01–24, partenaires sélectionnés, 2019–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Agréger valeurs, vérifier unités et dates. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** KPIs de référence; décomposition tendance; clustering exploratoire. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Cohérence des totaux et stabilité de clusters ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Agréger doubles comptes.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 32 — Avantage comparatif révélé des produits marocains

- **Domaine / niveau / compétences :** Export et marchés ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quelles catégories présentent un RCA de Balassa > 1 ?
- **Tâche précise :** Indices+classement. **Variable cible / indicateur :** RCA ou label RCA>1 défini avec dénominateur mondial.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504 et monde (sélection représentative), exports par HS2, 2022–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Construire parts pays et mondiales, vérifier couverture. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Classement RCA; scores normalisés; KMeans sur profils. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Stabilité années, concordance rangs ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Monde non exhaustif dans un extrait preview.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 33 — Avant/après d’un accord commercial

- **Domaine / niveau / compétences :** Export et marchés ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quelles évolutions observe-t-on autour d’un accord documenté ?
- **Tâche précise :** Analyse de panel. **Variable cible / indicateur :** Croissance / écart de flux annuel.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, partenaire choisi, TOTAL X/M, années autour de l’accord. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Identifier date accord via source juridique indépendante. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Comparaison descriptive; tendance linéaire; différences-en-différences si groupe contrôle défendable. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Placebos et diagnostics pré-tendance ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** DID sans tendances parallèles.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 34 — Choix de marchés cibles

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels pays prioriser pour un produit marocain ?
- **Tâche précise :** Aide décision multicritère. **Variable cible / indicateur :** Score de marché défini et documenté.
- **Jeu de données officiel :** UN Comtrade + World Bank API. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/ ; https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS ; https://api.worldbank.org/v2/country/mar/indicator/PA.NUS.FCRF?format=json.
- **Extraction exacte à effectuer :** Importations monde par pays pour HS07 + NY.GDP.MKTP.CD par pays. **Format :** JSON/CSV selon la source. **Accès :** Deux sources à harmoniser par période.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Normaliser taille demande, croissance, risque. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Scoring pondéré; TOPSIS; RandomForest exploratoire. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Robustesse classement selon les poids ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Poids subjectifs et données hétérogènes.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 35 — Barrières tarifaires sur un produit marocain

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels marchés pratiquent les droits les plus élevés pour un produit ?
- **Tâche précise :** Analyse descriptive+classement. **Variable cible / indicateur :** Taux appliqué / classement.
- **Jeu de données officiel :** OMC, Tariff and Trade Data. [Documentation](https://data.wto.org/en/dataset/wto_ttd). **Point d’accès / API :** https://ttd.wto.org/en/download.
- **Extraction exacte à effectuer :** WTO TTD/ADB : droit appliqué HS6 par économie et millésime, sélectionner un code. **Format :** JSON/CSV selon la source. **Accès :** Téléchargement via portail; inscription ou étapes interactives possibles.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Contrôler accords préférentiels et nomenclature. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Statistique descriptive; clustering; scoring. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Comparaison MFN versus préférentiel ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Tarif MFN confondu avec tarif réellement payé.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 36 — Performance logistique des pays

- **Domaine / niveau / compétences :** Logistique et macroéconomie ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Comment se regroupent les pays selon les composantes de la logistique ?
- **Tâche précise :** Clustering + visualisation. **Variable cible / indicateur :** Aucune.
- **Jeu de données officiel :** Banque mondiale, Logistics Performance Index. [Documentation](https://lpi.worldbank.org/). **Point d’accès / API :** https://lpi.worldbank.org/.
- **Extraction exacte à effectuer :** LPI 2023 : dimensions de performance des économies. **Format :** JSON/CSV selon la source. **Accès :** Millésimes distincts, sélection du fichier depuis portail.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Mise à l’échelle et manquants. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** KMeans; AgglomerativeClustering; PCA. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Silhouette, stabilité ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Biais perception et échantillon transversal.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 37 — Commerce agricole Maroc–Afrique

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels marchés africains importent davantage de fruits et légumes ?
- **Tâche précise :** Analyse panel+prévision. **Variable cible / indicateur :** Croissance des importations futures.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Import M des partenaires africains sélectionnés, HS07/08, 2010–2024, origine Maroc 504. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Pays/produits, devises, harmonisation. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Persistance; Ridge; RandomForestRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** MAE, WAPE ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Couverture douanière et saisonnalité.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 38 — Veille de changements commerciaux

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Comment détecter des variations anormales dans les échanges marocains ?
- **Tâche précise :** Détection alertes. **Variable cible / indicateur :** Aucune : alertes.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, X/M, HS2 01–24, données annuelles ou mensuelles si couvertes. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Comparer séries par produit et période. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Règle z robuste; IsolationForest; LocalOutlierFactor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Stabilité et pertinence alertes ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Données publiées avec retard.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 39 — Risque de dépendance fournisseurs

- **Domaine / niveau / compétences :** Export et marchés ; Intermédiaire ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels produits dépendent de quelques pays fournisseurs ?
- **Tâche précise :** Analyse concentration. **Variable cible / indicateur :** HHI des importations par produit.
- **Jeu de données officiel :** UN Comtrade, API publique preview. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS?reporterCode=504&period=2023&partnerCode=0&cmdCode=TOTAL&flowCode=X.
- **Extraction exacte à effectuer :** Maroc 504, M, HS2 01–24, partenaires, 2022–2024. **Format :** JSON/CSV selon la source. **Accès :** JSON API; 500 lignes maximum en aperçu sans clé; téléchargement complet soumis aux conditions d’accès.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Parts fournisseur, couverture pays et codes. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** HHI; concentration CR3; KMeans. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** Stabilité année, sensibilité au champ ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Oublier partenaires manquants.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

### Projet 40 — Recommandation de marchés export

- **Domaine / niveau / compétences :** Export et marchés ; Avancé ; pandas, visualisation, nettoyage, validation de modèles.
- **Question de recherche :** Quels pays pourraient devenir des débouchés pour un chapitre HS marocain ?
- **Tâche précise :** Recommandation/ranking. **Variable cible / indicateur :** Classement futur de croissance des marchés.
- **Jeu de données officiel :** UN Comtrade + World Bank API. [Documentation](https://uncomtrade.org/docs/un-comtrade-api/ ; https://datahelpdesk.worldbank.org/knowledgebase/articles/889392). **Point d’accès / API :** https://comtradeapi.un.org/public/v1/preview/C/A/HS ; https://api.worldbank.org/v2/country/mar/indicator/PA.NUS.FCRF?format=json.
- **Extraction exacte à effectuer :** Maroc X HS07 + importations monde HS07 et PIB, partenaires sélectionnés, 2010–2024. **Format :** JSON/CSV selon la source. **Accès :** Deux sources à harmoniser par période.
- **Dimensions et période :** la période demandée est indiquée dans l’extraction ; nombre de lignes/colonnes **à déterminer à partir du résultat**, non vérifié avant téléchargement. La couverture effective peut être plus courte.
- **Variables à relever :** année/mois, reporter, partenaire, produit HS, flux X/M, valeur commerciale (selon source) ; pour les sources macroéconomiques : code pays, année, valeur d’indicateur. Contrôler le schéma effectif.
- **Prétraitement :** Créer panel pays/année, lags, normaliser par taille. Documenter les valeurs manquantes, doublons, types, unités et exclusions.
- **Modèles :** Classement popularité; Ridge; RandomForestRegressor. Pour la validation, choisir une séparation temporelle pour toute tâche dépendant des années, et un jeu indépendant pour la comparaison finale.
- **Métriques et justification :** NDCG@5, Spearman, backtest temporel ; privilégier les métriques interprétables dans l’unité des échanges ou adaptées à la rareté des classes.
- **Risque majeur :** Recommandations non causales, choix des négatifs.
- **Livrables :** notebook reproductible, au moins cinq figures commentées, tableau comparatif, rapport LaTeX de 10–15 pages et soutenance de 8–10 minutes.
- **Directives de binôme :** J1 définir granularité et cible ; J2–J3 tester l’extraction ; J4–J5 nettoyage/EDA ; J6 référence ; J7–J8 alternatives ; J9 validation ; J10 interprétation ; J11–J13 rapport et contrôle ; J14 soutenance. **Plan B :** si un endpoint est limité, réduire à un seul pays, un chapitre HS et 3 à 5 millésimes accessibles ; si le volume devient trop petit, transformer le projet en analyse descriptive et signaler ce changement.

## Partie C — Guide des binômes (14 jours)

| Jour | Tâche | Preuve attendue |
|---|---|---|
| J1 | Problématique, unité d’analyse, protocole et partage des tâches | Fiche de cadrage |
| J2 | Accès aux données, droits et paramètres d’API | URL + test de chargement |
| J3 | Inventaire des variables, dictionnaire de données | Tableau dimensions/types |
| J4 | Nettoyage, manquants, unités et cohérence | Journal de nettoyage |
| J5 | EDA et 5 figures interprétées | **Jalon 1 : validation de source/EDA** |
| J6 | Modèle naïf ou règle de référence | Première métrique |
| J7 | Méthode alternative n°1 | Modèle exécutable |
| J8 | Méthode alternative n°2 et réglages | Table d’hyperparamètres |
| J9 | Validation sans fuite et mesure des erreurs | Tableau comparatif |
| J10 | Interprétation commerciale, limites et cas d’usage | **Jalon 2 : démonstration des modèles** |
| J11 | Vérification méthodologique et sensibilité | Analyse critique |
| J12 | Rédaction LaTeX et bibliographie | Brouillon PDF |
| J13 | Exécution « Run all », compilation PDF et archive | Dossier reproductible |
| J14 | Soutenance de 8–10 minutes | Projet final |

**Répartition :** les deux membres doivent chacun coder, analyser les résultats et rédiger au moins une section ; tenir un journal de tâches partagé. **Remise :** `.ipynb`, `.tex`, PDF, `README.md`, `requirements.txt`, figures, références. **Intégrité :** données/résultats non inventés, citations des sources, déclaration de l’assistance IA et défense individuelle du code.

**Barème sur 20 :** problème et données 2 ; acquisition/préparation 3 ; EDA 3 ; modélisation 4 ; évaluation 3 ; interprétation économique 2 ; rapport LaTeX 2 ; reproductibilité et soutenance 1. **Qualité :** insuffisant = étapes manquantes/non exécutables ; satisfaisant = protocole complet avec faiblesses ; bon = deux méthodes bien comparées et limites exposées ; excellent = reproductibilité, validation robuste, interprétation approfondie et sensibilité vérifiée.

## Sources et restrictions

- [UN Comtrade API — documentation](https://uncomtrade.org/docs/un-comtrade-api/) : aperçu public plafonné à 500 lignes, limites de fréquence ; accès étendu selon compte/clé.
- [Banque mondiale — API V2](https://datahelpdesk.worldbank.org/knowledgebase/articles/889392) : API libre sans clé, valeurs absentes possibles.
- [OMC — Tariff and Trade Data](https://data.wto.org/en/dataset/wto_ttd) : tarifs et commerce ; extraction via portail à vérifier selon fichier.
- [UNCTADstat](https://unctadstat.unctad.org/datacentre/) et [LPI](https://lpi.worldbank.org/) : tableaux ou millésimes à sélectionner ; disponibilité à vérifier.
- [FAOSTAT — Trade](https://www.fao.org/faostat/en/#data/TCL) : source agricole alternative pour les exercices.

> Les fichiers du package incluent un **squelette étudiant, sans solution**, ainsi qu’un rapport LaTeX exemple sans valeurs expérimentales inventées.
