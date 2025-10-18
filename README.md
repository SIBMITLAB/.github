# 🚀 SIBMITLAB - Organisation GitHub

Bienvenue dans l'espace de collaboration du Service IT et Innovation de la [Société Ivoirienne de Béton Manufracturé].
Ce dépôt sert de point central pour l'organisation, les standards de développement, les scripts d'infrastructure (CI/CD) et la documentation interne.

## 🎯 Mission et Objectifs

Notre mission est de construire des solutions logicielles robustes, maintenables et innovantes, en appliquant les meilleures pratiques du Génie Logiciel.

* **Standardisation :** Définir et maintenir des standards de codage et d'outillage (CI/CD).
* **Collaboration :** Faciliter la communication et la revue de code entre les équipes (Backend, Frontend, DevOps).
* **Performance :** Assurer un déploiement continu (CD) stable et rapide de toutes nos applications.

## 👥 Structure de l'Organisation et Équipes

L'organisation est structurée autour de rôles clairs pour garantir l'efficacité et la sécurité.

| Équipe | Rôle Principal | Accès aux Dépôts Clés | Membres Ciblés |
| :--- | :--- | :--- | :--- |
| **Team DevOps** | CI/CD, Scripts d'automatisation, Déploiement. | `Write` / `Maintain` | Techniciens et développeurs avancés. |
| **Team Backend** | Développement des API, Services, Bases de données. | `Write` / `Maintain` | Stagiaires, Développeurs, Ingénieurs. |
| **Team Frontend** | Interfaces utilisateur (Web/Mobile), UX/UI. | `Write` / `Maintain` | Stagiaires, Développeurs, Ingénieurs. |
| **Team Supervision** | Suivi, Statut des projets, Rapports. | `Read` / `Triage` | Managers, Chefs de Service. |

> 🔑 **Important :** Toute demande de modification de rôle ou d'accès doit être adressée à l'**Owner** de l'organisation (@Stagiaire-IT2025).

## 🗃️ Dépôts Clés

Voici quelques-uns des dépôts essentiels de notre organisation :

| Dépôt | Description | Équipes Responsables |
| :--- | :--- | :--- |
| `infrastructure` | **(Ce dépôt)** Contient les scripts shell, les configurations Docker, les workflows GitHub Actions (CI/CD) et les modèles de projet. | DevOps, Backend, Frontend |
| `api-service-v1` | Le cœur de notre logique métier et l'API principale. | Backend, DevOps |
| `frontend-web-app` | L'interface utilisateur de notre application web. | Frontend, DevOps |

## 🛠️ Standards de Développement et Outils

### 1. Workflow de Collaboration (Git Flow)

Nous utilisons un workflow basé sur `git-flow` simplifié (ou `GitHub Flow`).

1.  **Créer une branche :** Pour toute nouvelle fonctionnalité ou correction de bug, partez de `main` (ou `develop`) : `git checkout -b feature/nom-de-la-feature`
2.  **Pull Request (PR) :** La fusion vers `main` ou `develop` doit *toujours* passer par une Pull Request et nécessiter au moins **une revue par un autre membre de l'équipe** (Technicien / Ingénieur IT).
3.  **Tests :** Toutes les PR doivent passer les tests automatisés du CI/CD.

### 2. Normes de Commit

Veuillez utiliser le format **Conventional Commits** pour des messages clairs :

* `feat: Ajout d'une nouvelle fonctionnalité...`
* `fix: Correction d'un bug critique...`
* `docs: Mise à jour de la documentation...`
* `ci: Mise à jour des workflows CI/CD...`

### 3. Outils et Technologies

| Domaine | Outils/Langages (Exemple à adapter) |
| :--- | :--- |
| **Backend** | Python (Django/Flask), Node.js, PostgreSQL |
| **Frontend** | React, Vue.js, Tailwind CSS |
| **CI/CD & Infra** | GitHub Actions, Docker, Scripts Shell |

## 🔗 Ressources Utiles

* [Lien vers la Documentation Interne (Confluence/SharePoint)]
* [Lien vers le Tableau de Bord Projet (Trello/Jira)]
* [Lien vers la Charte Graphique SIBM]

---
*Dernière mise à jour : [Date]*
