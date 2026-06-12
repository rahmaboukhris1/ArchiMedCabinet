# Structure du projet MedCabinet

## Arborescence

```text
MedCabinet F/
│
├── .dockerignore
├── .gitignore
├── docker-compose.local.yml
├── README.md
│
├── .github/
│   └── workflows/
│       ├── backend-ci.yml
│       ├── build-docker.yml
│       ├── copilot-code-review.yml
│       ├── deploy.yml
│       ├── docker-build.yml
│       ├── docker-push.yml
│       ├── frontend-ci.yml
│       ├── quality-gates.yml
│       ├── security-audit.yml
│       └── security-scanning.yml
│
├── backend/
│   ├── app/
│   │   ├── Console/
│   │   ├── Exceptions/
│   │   ├── Http/
│   │   │   ├── Controllers/
│   │   │   ├── Middleware/
│   │   │   ├── Requests/
│   │   │   └── Resources/
│   │   ├── Models/
│   │   ├── Services/
│   │   └── Providers/
│   ├── bootstrap/
│   ├── config/
│   ├── database/
│   │   ├── migrations/
│   │   ├── seeders/
│   │   └── factories/
│   ├── public/
│   ├── resources/
│   ├── routes/
│   ├── storage/
│   └── tests/
│
├── frontend/
│   ├── src/
│   │   ├── app/
│   │   │   ├── appointments/
│   │   │   ├── components/
│   │   │   │   ├── admin/
│   │   │   │   ├── appointments/
│   │   │   │   ├── auth/
│   │   │   │   ├── charts/
│   │   │   │   ├── chatbot/
│   │   │   │   ├── consultations/
│   │   │   │   ├── doctor/
│   │   │   │   ├── messages/
│   │   │   │   ├── patients/
│   │   │   │   ├── prescriptions/
│   │   │   │   └── shared/
│   │   │   │       └── confirmation-modal/
│   │   │   ├── directives/
│   │   │   ├── guards/
│   │   │   ├── interceptors/
│   │   │   ├── layout/
│   │   │   ├── models/
│   │   │   ├── modules/
│   │   │   │   ├── admin/
│   │   │   │   │   ├── components/
│   │   │   │   │   │   └── user-form/
│   │   │   │   │   ├── pages/
│   │   │   │   │   │   ├── admin-dashboard/
│   │   │   │   │   │   ├── admin-doctors/
│   │   │   │   │   │   ├── admin-medecins/
│   │   │   │   │   │   ├── admin-parametrage/
│   │   │   │   │   │   ├── admin-patients/
│   │   │   │   │   │   ├── admin-rdc/
│   │   │   │   │   │   ├── admin-secretaires/
│   │   │   │   │   │   ├── admin-secretaries/
│   │   │   │   │   │   ├── admin-settings/
│   │   │   │   │   │   ├── admin-users/
│   │   │   │   │   │   └── admin-utilisateurs/
│   │   │   │   │   └── styles/
│   │   │   │   ├── doctor/
│   │   │   │   │   └── pages/
│   │   │   │   │       ├── doctor-appointments/
│   │   │   │   │       ├── doctor-dashboard/
│   │   │   │   │       ├── doctor-help/
│   │   │   │   │       ├── doctor-messages/
│   │   │   │   │       ├── doctor-patients/
│   │   │   │   │       ├── doctor-payment/
│   │   │   │   │       ├── doctor-prescriptions/
│   │   │   │   │       ├── doctor-report/
│   │   │   │   │       ├── doctor-settings/
│   │   │   │   │       └── doctor-waiting-room/
│   │   │   │   ├── patient/
│   │   │   │   │   ├── components/
│   │   │   │   │   │   └── patient-chatbot/
│   │   │   │   │   ├── guards/
│   │   │   │   │   ├── layout/
│   │   │   │   │   │   └── patient-layout/
│   │   │   │   │   ├── pages/
│   │   │   │   │   │   ├── appointment-request/
│   │   │   │   │   │   ├── patient-account/
│   │   │   │   │   │   ├── patient-appointments/
│   │   │   │   │   │   ├── patient-dashboard/
│   │   │   │   │   │   ├── patient-documents/
│   │   │   │   │   │   ├── patient-home/
│   │   │   │   │   │   ├── patient-login/
│   │   │   │   │   │   ├── patient-messages/
│   │   │   │   │   │   ├── patient-notifications/
│   │   │   │   │   │   ├── patient-profile/
│   │   │   │   │   │   ├── patient-register/
│   │   │   │   │   │   └── patient-specialties/
│   │   │   │   │   ├── services/
│   │   │   │   │   └── styles/
│   │   │   │   └── secretary/
│   │   │   │       └── pages/
│   │   │   │           ├── secretary-appointments/
│   │   │   │           ├── secretary-dashboard/
│   │   │   │           ├── secretary-help/
│   │   │   │           ├── secretary-messages/
│   │   │   │           ├── secretary-notifications/
│   │   │   │           ├── secretary-patients/
│   │   │   │           ├── secretary-payments/
│   │   │   │           ├── secretary-profile/
│   │   │   │           └── secretary-salle-attente/
│   │   │   └── shared/
│   │   ├── pages/
│   │   │   └── landing/
│   │   ├── pipes/
│   │   ├── services/
│   │   ├── styles/
│   │   └── templates/
│   │       └── ordonnance/
│   │   └── assets/
│   │       ├── data/
│   │       │   └── medications.json
│   │       ├── i18n/
│   │       │   ├── de.json
│   │       │   ├── en.json
│   │       │   └── fr.json
│   │       └── icons/
│   │           ├── caduceus-top.svg
│   │           └── caduceus-watermark.svg
│   │   └── environments/
│   │       ├── environment.prod.spec.ts
│   │       ├── environment.prod.ts
│   │       ├── environment.spec.ts
│   │       └── environment.ts
│   ├── public/
│   ├── coverage/
│   ├── angular.json
│   ├── karma.conf.js
│   ├── package.json
│   └── tsconfig.json
│
├── docker/
│   ├── backend/
│   ├── frontend/
│   └── mysql/
│
├── kubernetes/
│
├── github-actions/
│
├── documentation/
│   ├── api/
│   ├── architecture/
│   ├── devops/
│   └── security/
│
└── md/
    ├── tests/
    ├── rapports/
    └── specifications/
```

## Description rapide

- **backend/** : API Laravel 10, logique métier, contrôleurs, modèles Eloquent, services (IA, PDF, SMS, email), routes API, migrations et tests.
- **frontend/** : Application Angular 16+ monopage (SPA) avec modules métier par rôle (admin, médecin, secrétaire, patient). Inclut composants UI, services, intercepteurs, pipes, templates et assets.
- **docker/** : Configurations et fichiers Docker pour backend, frontend et base de données MySQL.
- **kubernetes/** : Manifests Kubernetes pour déploiement et orchestration.
- **github-actions/** : Workflows GitHub Actions pour CI/CD (tests, build, déploiement).
- **documentation/** : Documents d’architecture, spécifications API, guides DevOps et audits sécurité.
- **`ARCHITECTURE_GLOBAL_DIAGRAMS.md`** : Diagrammes Mermaid (architecture globale, couches, base de données, module IA, sécurité, DevOps, flux de données).
- **`AI_CHATBOT_DOCUMENTATION.md`** : Pipeline chatbot, flux de requête, sécurisation, limites du LLM et paramètres.
- **`SPECIFICATION_COMPLETE_16WEEKS.md`** : Spécifications fonctionnelles et techniques du projet.

> Repository cible : https://github.com/rahmaboukhris1/ArchiMedCabinet.git
