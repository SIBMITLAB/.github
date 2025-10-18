# SIBMITLAB Organisation GitHub

Bienvenue dans l'espace de collaboration du **DSI [Direction Système Informatique** de la Société Ivoirienne de Béton Manufacturé (SIBM).

Ce dépôt sert de point central pour l'organisation, la gouvernance des standards de développement, les pipelines d'infrastructure (CI/CD) et la documentation interne.

---

## Mission et Objectifs

Notre mission est de Centraliser, Concevoir, Développer, Automatiser nos projets internes, des scripts administratifs, des App/Logiciels, des automatisations des tâches relatif à nos utilisateurs , tout en assurant la stabilité des infrastructures IT et la continuité opérationnelle.

- **Standardisation** : Définir et maintenir des standards cohérents de codage, d'outillage et de déploiement (CI/CD)
- **Collaboration** : Faciliter la communication et la revue de code entre les équipes (Réseaux, Systèmes, Support, Développement, DBA)
- **Excellence opérationnelle** : Garantir un déploiement continu (CD) stable, sécurisé et performant
- **Intégration ERP** : Assurer la continuité et l'optimisation de l'écosystème Sage X3.

---

## Structure Organisationnelle

L'organisation est structurée selon une hiérarchie claire et des rôles définis pour assurer gouvernance, efficacité et traçabilité.

| Rôle | Responsabilité | Accès | Équipes Supervisées |
|:-----|:--------------|:------|:--------------------|
| **DSI** (Directeur SI) | Gouvernance IT, décisions stratégiques, reporting exécutif | `Admin` |Toutes les équipes |
| **RSI** (Responsable SI) | Supervision opérationnelle, coordination inter-équipes, gestion des projets | `Maintain` / `Write` | Réseaux, Systèmes, Support, Dev, DBA|
| **AI** (Assistant Informatique) | Support niveau 2, documentation, automatisation, aide à la supervision | `Maintain` / `Write` | Ingénieurs, développeurs, stagiaires |
| **Dev** (Développeur) | Services métier, APIs, UI/UX, App WEB | `Maintain` / `Write` | N/A |

> 🔑 **Accès et Permissions** : Toute demande de modification de rôle, d'accès ou d'ajout de membre doit être adressée au DSI ou RSI

## Équipes Techniques

| Équipe | Domaine | Accès | Description |
|:-------|:--------|:------|:------------|
| **Réseaux** | Infrastructure réseau, sécurité, VPN, firewalls | `Maintain` / `Write` | Gestion et supervision du réseau SIBM |
| **Systèmes** | Serveurs Windows/Linux, virtualisation, monitoring | `Maintain` / `Write` | Administration serveurs et infrastructure |
| **Développement** | Applications métier, APIs, intégrations ERP, scripts | `Write` / `Maintain` | Dev web, backend, intégrations Sage X3 |
| **Base de Données** | DBA, optimisation SQL Server/MySQL, backups, migrations | `Write` / `Maintain` | Gestion des BD, perf, sécurité données |


---

## Dépôts Clés

| Dépôt | Description | Équipes Responsables | Stack |
|:------|:------------|:---------------------|:------|
| `infrastructure` | Scripts d'automatisation, configs Docker, workflows CI/CD, IaC, monitoring | Réseaux, Systèmes, Dev | Bash, PowerShell, GitHub Actions |
| `sage-x3-integration` | Connecteurs, API, ETL et scripts d'intégration avec Sage X3 | Développement, DBA | Python, C#, Node.js, SQL |
| `api-services` | Services API métier, backend core | Développement, DBA | Python, PHP, Node.js, C#, SQL Server, MySQL | 
| `web-application` | Applications web métier et dashboards | Développement | JavaScript, React, Power BI |
| `monitoring-dashboards` | Grafana, scripts de monitoring, alertes infrastructure | Systèmes, Réseaux | Grafana, Bash, Python |
| `database-scripts` | Migrations DB, procédures stockées, optimisations, backups | DBA | SQL Server, MySQL |
| `windows-admin` | Scripts d'administration Windows Server, GPO, automation | Systèmes | PowerShell, VBScript |
| `linux-admin` | Scripts Debian, configurations système, hardening | Systèmes | Bash, Python, Ansible | 
| `documentation` | Docs techniques, runbooks, procédures, architecture | Toutes les équipes | Markdown |

---

## Stack Technologique et Outils

### Backend et Développement

| Technologie | Usage | Équipes |
|:---|:---|:---|
| **Python** | Scripts d'automatisation, ETL, intégrations, data science | Dev, DBA, Systèmes |
| **PHP** | Applications web légacies, intégrations | Développement |
| **Node.js** | APIs REST, services métier, temps réel | Développement |
| **C#** | Applications .NET, services Windows | Développement |
| **JavaScript** | Frontend, scripting client | Développement |

### Bases de Données

| Technologie | Usage | Équipes |
|:---|:---|:---|
| **SQL Server** | BD production, Sage X3, données critiques | DBA, Développement |
| **MySQL** | BD applicatifs, données secondaires | DBA, Développement |

### Infrastructure et Administration

| Technologie | Usage | Équipes |
|:---|:---|:---|
| **Windows Server** | Serveurs production, services AD/DNS, Exchange | Systèmes |
| **Linux Debian** | Serveurs applicatifs, services légers, CI/CD | Systèmes, Réseaux |
| **GitHub Actions** | CI/CD pipelines, automation workflows | Développement, DevOps |
| **Docker** | Containerisation, déploiement, isolation | Développement, Systèmes |

### Monitoring et Analytics

| Technologie | Usage | Équipes |
|:---|:---|:---|
| **Grafana** | Dashboards temps réel, monitoring infrastructure | Systèmes, Réseaux |
| **Humbutu** | [À préciser : Outil de log management/monitoring ?] | Systèmes |
| **Power BI** | Rapports métier, dashboards analytiques, KPIs | Développement, Management |

### Outils Bureautique et Productivité

| Outil | Usage | Utilisation |
|:---|:---|:---|
| **Office 365** | Email, collaboration, documents | Toute l'entreprise |
| **Excel** | Analyses, calculs, exports de données | Tous |
| **Sage X3** | ERP métier, gestion commerciale/RH/comptabilité | Toute l'entreprise |

### Méthodologie

| Élément | Description |
|:---|:---|
| **SCRUM Agile** | Sprints 2 semaines, dailys, retros, plannings pour toutes les équipes dev |

---

## Processus et Standards de Développement

### Workflow de Collaboration (Git Flow)

Nous suivons un workflow simplifié basé sur **GitHub Flow** pour la gestion des branches :

1. **Créer une branche** : Pour chaque fonctionnalité ou correction, créez une branche depuis `main`.
   ```bash
   git checkout -b feature/description-courte
   # Ou : fix/ticket-123-description
   ```

2. **Développer et commiter** : Utilisez le format **Conventional Commits** pour la clarté
   ```bash
   git commit -m "feat: intégration Sage X3 pour flux d'achat"
   git commit -m "fix(api): correction calcul TVA module facturation"
   ```

3. **Pull Request** : Fusionner vers `main` ou `develop` **uniquement via Pull Request**
   - Minimum **1 revue approuvée** par un développeur expérimenté
   - Tous les tests CI/CD doivent passer
   - Conformité aux standards de code
   - Les conflits doivent être résolus avant merge

### Normes de Commit

Format **Conventional Commits** obligatoire :

- `feat:` – Nouvelle fonctionnalité
- `fix:` – Correction de bug
- `refactor:` – Restructuration du code (sans changement fonctionnel)
- `perf:` – Optimisations de performance
- `test:` – Ajout/modification de tests
- `docs:` – Mise à jour documentation
- `ci:` – Mise à jour CI/CD ou configuration
- `chore:` – Maintenance générale, dépendances
- `infra:` – Modifications infrastructure (Terraform, Ansible)

**Exemples :**
```
feat(sage-x3): synchronisation articles de stock en temps réel
fix(api-services): correction délai timeout API commandes
perf(database): optimisation index table_factures
infra(monitoring): ajout alertes CPU > 80%
```

### Checklist Pull Request

Avant de soumettre une PR, assurez-vous que :

- [ ] La branche est à jour avec `main` ou `develop`
- [ ] Messages de commit respectent **Conventional Commits**
- [ ] Tests locaux passent (`npm test`, `pytest`, `dotnet test`, etc.)
- [ ] Code conforme aux standards de style et linting
- [ ] Documentation mise à jour (README, runbooks, Confluence)
- [ ] Aucun secret, token, credential ou données sensibles
- [ ] Migrations DB testées et documentées (si applicable)
- [ ] Logs et monitoring configurés pour la fonctionnalité

---

## Sécurité et Bonnes Pratiques

- **Secrets Management** : Utiliser GitHub Secrets, ne jamais commiter credentials
- **Code Review** : Tout code production doit être revu avant fusion
- **Tests Automatisés** : CI pipelines valident builds, tests unitaires, linting, SAST
- **Infrastructure as Code** : Documenter infrastructure via code (Terraform, Ansible)
- **Monitoring** : Grafana, alertes configurées pour services critiques
- **Backups BD** : Procédures documentées pour SQL Server et MySQL
- **Audit Logs** : Traçabilité des accès et modifications

---

## Intégration Sage X3

### Principes d'Intégration

- Les connecteurs Sage X3 sont versionnés dans le dépôt `sage-x3-integration`
- Documentations des APIs et flux dans Confluence
- Tests d'intégration obligatoires avant deployment
- Monitoring des synchro en temps réel via Grafana

### Équipes Impliquées

- **Développement** : Dev connecteurs et APIs
- **DBA** : Optimisation requêtes, gestion transactions
- **Systèmes** : Infrastructure serveurs Sage X3

---

## Contacts et Escalades

| Rôle | Nom | Contact | Disponibilité |
|:---|:---|:---|:---|
| **DSI** | <!-- TODO: Prénom Nom --> | <!-- TODO: email@sibmci.com --> | Lun-Ven |
| **RSI** | <!-- TODO: Prénom Nom --> | <!-- TODO: email@sibmci.com --> | Lun-Ven |
| **AI** | <!-- TODO: Prénom Nom --> | <!-- TODO: email@sibmci.com --> | Lun-Ven |
| **Dev** | KEI PRINCE FREJUSTE | stagiaire.info@sibmci.com | Lun-Ven |


---

## Ressources Utiles

- [Documentation Interne (Confluence)](<!-- TODO: URL Confluence -->)
- [Dashboards Grafana (Monitoring)](<!-- TODO: URL Grafana -->)
- [Charte Graphique SIBM](<!-- TODO: URL Charte Graphique -->)
- [Tableau de Bord Projets SCRUM](<!-- TODO: URL Tableau de Bord -->)
- [Wiki Sage X3 Interne](<!-- TODO: URL Wiki -->)
- [Runbooks et Procédures](<!-- TODO: URL Runbooks -->)

---

## Calendrier et Planning

- **Sprints** : Cycles 2 semaines
- **Dailys** : Lun-Ven 10h00
- **Retro/Planning** : Fin et début de sprint
- **Maintenance Serveurs** : Planifiée mardi/jeudi 22h-23h

---

*Dernière mise à jour : 18/10/2025*
*Version : 1.1*
*Approuvé par : [DSI/RSI]*
