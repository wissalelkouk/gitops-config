Dépôt GitOps du projet **Gestion Bibliothèque** (projet semestriel Master DevOps & Cloud, ISET Tozeur).
Il contient les manifests Kubernetes surveillés par ArgoCD.

## Architecture
Application web en microservices :
- user-service : authentification et gestion des utilisateurs
- book-service : catalogue et emprunts
- notification-service : notifications de retard

## Dépôts du projet
- https://github.com/wissalelkouk/user-service
- https://github.com/wissalelkouk/book-service
- https://github.com/wissalelkouk/notification-service

## Chaîne DevOps
Jira, GitHub, CI, Docker, Trivy, Kubernetes, ArgoCD, Prometheus et Grafana.

## Stratégie de branches
- `main` : version stable, protégée
- `develop` : intégration
- `feature/LIB-xx-description` : une branche par ticket Jira

## Convention de commit
`type(portée): description (LIB-xx)` avec les types feat, fix, docs, chore, test.

## Structure
- `user-service/`, `book-service/`, `notification-service/` : manifests de chaque service
- `monitoring/` : Prometheus et Grafana
- `docs/` : schémas et documentation# gitops-config
