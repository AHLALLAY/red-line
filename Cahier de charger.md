# 🏫 System de Gestion Des Ecoles [Ecole Network]

## ❗ Problématique
Dans le domaine de l'éducation, notre étude révèle une réalité préoccupante: **plus de 70%** des établissements restent dépendants des méthodes traditionnelles (papier et gestion manuelle) pour leurs opérations quotidiennes, notamment :
* L'inscription des étudiants
* La gestion du personnel
* Les tâches administratives
* Le suivi académique

### 📊 Impact Négatifs Constatés

Impact|Description
--|--
Temps|Gestion inefficace et chronophage des processus
Ressources humaines|Surcharge de travail et risques d'erreurs
Ressources Financières|Coûts élevés liés à la gestion papier
Qualité de service|Délais de traitement importants
Communication|Difficulté de partage d'information

## 💡 Solutions
**Ecole Network** est une solution innovante dédiée à la gestion scolaire moderne. Cette Application répond aux besoins croissants de digitalisation du secteur éducatif en proposant des outils performants et intuitifs.

### 🔧 Architecture Technique
* Backend : PHP/MySQL.
* Frontend : HTML5, CSS3, JavaScript.
* Sécurité : 
    * Authentification sécurisée.
    * Chiffrement des données sensibles.
    * Protection contre les injections SQL.
* Conformité RGPD :
    * Gestion des consentements.
    * Protection des données personnelles.
    * Droit à l'oubli.

## 👥 Acteurs et leurs rôles
### 👨‍💼 Admin
#### 📋 Users stories
1. Se connecter avec un email fixe (stocké dans la base de données)
2. Gérer les personnels :
    * Ajouter un personnel (nom, prénom, date de naissance, adresse, diplôme, rôle, photo)
    * Suspendre un personnel
    * Suppression douce d'un personnel
3. Générer les emplois du temps
4. Consulter les Statistiques :
    * Absences (personnel et élèves)
    * Effectifs
    * Données financières
5. Filtrer les élèves selon :
    * Niveau scolaire
    * Classe
    * Âge
    * Notes

#### 📱 Pages
1. index.php :
    * Section accueil :
        * Carrousel d'images présentant l'école.
        * Paragraphe de bienvenue.
    * Section d'informations :
        * L'équipe pédagogique.
        * Capacité maximale.
        * Localisation.
    * Section de demande d'inscription :
        * Formulaire d'inscription.
    * Section offres d'emploi/stage.
2. login.php
    * Formulaire de connexion :
        * Email.
        * Mot de passe.
3. admin.php
    * Section 'nouvelle personnel' :
        * pour ajouter un nouveau personnel.
    * Section 'Personnelles' :
        * Liste des personnels.
        * Options de filtrage.
    * Section 'Elèves' :
        * Liste des élèves.
        * Filtres de recherche.
    * Section statistiques :
        * Tableaux de bord.
        * Graphiques.

### 👨‍🏫 Professeur
#### 📋 Users stories
1. Se connecter
2. Gérer les absences
3. Noter les activités :
    * Cours effectués
    * Évaluations
4. Consulter les documents
5. Gérer les parcours scolaires
6. Filtrer les élèves
7. Gérer les congés
#### 📱 Pages
1. login.php :
    * Formulaire de connexion sécurisé.
2. professeur.php :
    * Section tableau de bord
        * Emploi du temps
        * Notifications
    * Section classes
        * Liste des élèves
        * Gestion des absences
    * Section cahier de texte
        * Activités réalisées
        * Devoirs donnés
3. evaluations.php
    * Section notes
        * Saisie des notes
        * Historique des évaluations
    * Section statistiques
        * Moyennes par classe

### 👨‍🎓 Elèves
#### 📋 Users stories
1. Consulter les activités.
2. Consulter les notes.
3. Voir les congés.
#### 📱 Pages
1. login.php :
    * Formulaire de connexion élève.
2. eleve.php :
    * Section 'activité à domicile' :
        * Liste des devoirs..
        * Ressources disponibles.
    * Section 'relever de note' :
        * Notes par matière.
        * Moyenne générale.
    * Section emploi du temps :
        * Planning hebdomadaire.
        * Événements spéciaux.

### 👪 Parents
#### 📋 Users stories
1. Consulter l'accueil
2. Inscrire un enfant
3. Suivre les activités
4. Consulter les notes
#### 📱 Pages
1. index.php :
    * Même contenu que admin.index.php.
2. login.php :
    * Formulaire de connexion parents.
3. parent.php :
    * Section suivi enfants :
        * Notes et évaluations.
        * Absences et retards.
    * Section communications :
        * Messages des enseignants.
        * Notifications école.

### 👩‍💼 Secrétaire
#### 📋 Users stories
1. Gérer les documents :
    * Scanner les pièces
    * Imprimer les attestations
    * Gérer les relevés
    * Gérer les départs
#### 📱 Pages
1. login.php :
    * Formulaire de connexion secrétaire.
2. document.php :
    * Section gestion documents :
        * Scanner de documents.
        * Classement numérique.
    * Section attestations :
        * Génération attestations :
            - Pour stagiaires.
            - Pour personnels.
        * Impression relevés de notes.
    * Section archivage :
        * Gestion des départs.
        * Historique documents.

### 💰 Comptable
#### 📋 Users stories
1. Gérer la comptabilité
#### 📱 Pages
1. comptable.php :
    * Section comptabilité :
        * Saisie des charges.
        * Saisie des produits.
    * Section rapports.

## ⭐ Fonctionnalités Additionnelles
* Notifications par email ou SMS
* Export PDF des documents
* Sauvegarde automatique
* Messagerie interne