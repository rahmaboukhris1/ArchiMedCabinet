# GitHub Actions

Workflows CI/CD définis dans `.github/workflows/` du projet.

Workflows couverts :
- `backend-ci.yml` — tests PHPUnit / Pint / PHPStan
- `frontend-ci.yml` — build Angular + lint
- `build-docker.yml` — construction d’images Docker
- `docker-push.yml` — push vers GitHub Container Registry
- `deploy.yml` — déploiement staging / production
- `security-audit.yml` — audit des dépendances
- `security-scanning.yml` — scan d’images
- `quality-gates.yml` — vérification qualité globale
- `copilot-code-review.yml` — re vue automatisée

Ce dossier contient la documentation et le référencement de ces workflows.