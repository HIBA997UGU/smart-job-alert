
# Smart Job Alert 🚀

## 1. Présentation du projet

Smart Job Alert est une application web qui automatise la recherche et le suivi des offres d'emploi grâce à un workflow développé avec n8n.

L'objectif est de faciliter la recherche d'opportunités professionnelles en centralisant la récupération, le filtrage et le suivi des offres.

## 2. Fonctionnalités principales

- Recherche d'offres selon un mot-clé.
- Sélection de la source d'offres disponible.
- Recherche par localisation (facultative).
- Filtrage automatique des offres.
- Calcul d'un score de pertinence pour chaque offre.
- Affichage des résultats dans une interface web.
- Enregistrement des offres dans Google Sheets.
- Envoi de notifications par e-mail.

## 3. Architecture du workflow n8n

Le workflow suit les étapes principales suivantes :

1. **Webhook** : reçoit les données du formulaire.
2. **Edit Fields** : prépare les paramètres de recherche.
3. **Switch** : oriente le traitement selon la source choisie.
4. **HTTP Request** : récupère les offres depuis l'API.
5. **Split Out** : sépare les offres pour leur traitement.
6. **Filter** : filtre les offres selon les critères.
7. **Job Score** : calcule le score de pertinence.
8. **Respond to Webhook** : renvoie les résultats à l'interface.
9. **Google Sheets** : enregistre les offres.
10. **Send an Email** : envoie les alertes par e-mail.

## 4. Technologies utilisées

- HTML
- CSS
- JavaScript
- n8n Cloud
- API REST
- Google Sheets
- SMTP
- GitHub Pages

## 5. Démonstration

Application en ligne :

https://hiba997ugu.github.io/smart-job-alert/

## 6. Exemple de test

Lors d'un test avec le mot-clé `scientist`, l'application a retourné deux offres :

- Senior Data Scientist (NLP & Applied AI)
- Research Scientist

Les résultats peuvent varier selon la disponibilité des offres et les critères de recherche.

## 7. Structure du projet

Le dépôt GitHub contient actuellement le frontend :

- `index.html` : interface utilisateur et formulaire de recherche.

Le workflow d'automatisation est hébergé séparément sur n8n Cloud.

## 8. Sécurité

Les identifiants, mots de passe, clés API, tokens et URL privées du webhook ne doivent jamais être publiés dans le dépôt GitHub.

---

**Projet personnel – Smart Job Alert**
