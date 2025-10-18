# 🚀 SIBMITLAB – Organisation GitHub

Bienvenue dans l'espace de collaboration du **Service IT et Innovation** de la Société Ivoirienne de Béton Manufacturé (SIBM).

Ce dépôt sert de point central pour l'organisation, la gouvernance des standards de développement, les pipelines d'infrastructure (CI/CD) et la documentation interne.

---

## 🎯 Mission et Objectifs

Notre mission est de concevoir et maintenir des solutions logicielles robustes, scalables et innovantes en appliquant les meilleures pratiques du génie logiciel moderne.

- **Standardisation** : Définir et maintenir des standards cohérents de codage, d'outillage et de déploiement (CI/CD)
- **Collaboration** : Faciliter la communication et la revue de code entre les équipes (Backend, Frontend, DevOps)
- **Excellence opérationnelle** : Garantir un déploiement continu (CD) stable, sécurisé et performant

---

## 👥 Structure Organisationnelle

L'organisation est structurée selon des rôles et responsabilités clairement définis pour assurer l'efficacité, la sécurité et la traçabilité.

| Équipe | Rôle Principal | Accès | Profil Ciblé |
|:---|:---|:---|:---|
| **DevOps** | Infrastructure, CI/CD, automatisation, déploiement | `Write` / `Maintain` | Techniciens, développeurs avancés |
| **Backend** | Services métier, APIs, bases de données | `Write` / `Maintain` | Ingénieurs, développeurs, stagiaires |
| **Frontend** | Applications web/mobile, UX/UI | `Write` / `Maintain` | Ingénieurs, développeurs, stagiaires |
| **Supervision** | Suivi projet, reporting, gouvernance | `Read` / `Triage` | Responsables, managers, chefs de service |

> 🔑 **Accès et Permissions** : Toute demande de modification de rôle, d'accès ou d'ajout de membre doit être adressée à l'Owner de l'organisation : **@Stagiaire-IT2025**

---

## 🗂️ Dépôts Clés

| Dépôt | Description | Équipes Responsables |
|:---|:---|:---|
| `infrastructure` | **(Ce dépôt)** Scripts d'automatisation, configurations Docker, workflows GitHub Actions, modèles de projet et documentation DevOps | DevOps, Backend, Frontend |
| `api-service-v1` | Services API et logique métier centralisée | Backend, DevOps |
| `frontend-web-app` | Application web client (React/Vue.js) | Frontend, DevOps |

---

## 🛠️ Standards et Pratiques de Développement

### Workflow de Collaboration (Git Flow)

Nous suivons un workflow simplifié basé sur **GitHub Flow** pour la gestion des branches :

1. **Créer une branche** : Pour chaque fonctionnalité ou correction, créez une branche depuis `main` ou `develop`
   ```bash
   git checkout -b feature/description-courte
   ```

2. **Développer et commiter** : Utilisez le format **Conventional Commits** pour la clarté
   ```bash
   git commit -m "feat: ajout de la fonctionnalité X"
   ```

3. **Pull Request** : Fusionner vers `main` ou `develop` **uniquement via Pull Request**
   - Minimum **1 revue approuvée** par un membre qualifié
   - Tous les tests CI/CD doivent passer
   - Les conflits doivent être résolus avant merge

### Normes de Commit

Utilisez le format **Conventional Commits** pour une meilleure traçabilité :

- `feat:` – Nouvelle fonctionnalité
- `fix:` – Correction de bug
- `docs:` – Mise à jour documentation
- `style:` – Formatage du code (sans logique)
- `refactor:` – Restructuration du code
- `test:` – Ajout ou modification de tests
- `ci:` – Mise à jour CI/CD ou configuration

**Exemple :**
```
feat: authentification OAuth2 pour les APIs
Implémenter le flow OAuth2 avec support des scopes personnalisés.
```

### Stack Technologique

| Domaine | Technologies |
|:---|:---|
| **Backend** | Python (Django/Flask), Node.js, PostgreSQL |
| **Frontend** | React, Vue.js, Tailwind CSS |
| **Infrastructure** | GitHub Actions, Docker, Shell scripts |
| **Sécurité** | GitGuardian (secrets), CodeQL (SAST) |

---

## 📋 Checklist Pull Request

Avant de soumettre une PR, assurez-vous que :

- [ ] La branche est à jour avec `main` ou `develop`
- [ ] Les messages de commit respectent **Conventional Commits**
- [ ] Les tests locaux passent (`npm test`, `pytest`, etc.)
- [ ] La documentation a été mise à jour si nécessaire
- [ ] Pas de secrets, tokens ou données sensibles dans le code
- [ ] Le code est conforme aux standards de style du projet

---

## 🔐 Sécurité et Bonnes Pratiques

- **Secrets** : Ne jamais commiter de clés, tokens ou données sensibles. Utiliser les secrets GitHub Actions
- **Reviews** : Tout code doit être revu avant fusion
- **Tests** : Les pipelines CI doivent valider builds, tests et linting
- **Documentation** : Documenter les décisions architecturales majeures

---

## 🔗 Ressources Utiles

- 📖 [Documentation Interne (Confluence/SharePoint)]
- 📊 [Tableau de Bord Projets (Jira/Trello)]
- 🎨 [Charte Graphique SIBM]
- 📚 [Guide DevOps Interne]

---

## 📞 Support et Contact

Pour toute question, demande d'accès ou escalade :

- **Responsable Technique** : [Nom/Contact]
- **Owner Organisation** : @Stagiaire-IT2025
- **Email** : [it-innovation@sibm.ci]

---

*Dernière mise à jour : [Date]*  
*Version : 1.0*
