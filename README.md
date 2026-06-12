# Architecture Documentation — MedCabinet

Ce dépôt contient la documentation d'architecture du projet **MedCabinet**.
Aucun code source n'est inclus : seulement l'arborescence, les schémas et les explications de chaque couche.

## Contenu

| Fichier / dossier | Rôle |
|-------------------|------|
| `PROJECT_STRUCTURE.md` | Arborescence ASCII complète et description des dossiers |
| `backend/` | Structure du backend Laravel (API REST + JWT + MySQL) |
| `frontend/` | Structure du frontend Angular 16 (SPA multiprofils) |
| `docker/` | Configurations Docker (Nginx, PHP, MySQL) |
| `kubernetes/` | Manifests de déploiement (Deployments, Services, Ingress) |
| `github-actions/` | Workflows CI/CD (tests, build, scan, déploiement Docker) |
| `documentation/` | Documents d'architecture, API, sécurité et DevOps |

## Stack technique

- Frontend : Angular 16 + TypeScript + Bootstrap 5
- Backend : Laravel 10 + PHP 8.2 + JWT
- Base de données : MySQL 8 + Redis
- IA : DeepSeek / Gemini / Groq (chatbot médical)
- DevOps : Docker Compose + GitHub Actions + Kubernetes

> Voir `PROJECT_STRUCTURE.md` pour l'arborescence détaillée.
