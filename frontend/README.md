# Frontend — Angular 16+

Application monopage (SPA) destinée aux médecins, secrétaires et patients.

- **UI** : Bootstrap 5, Chart.js, FullCalendar, ngx-toastr, ngx-translate
- **State** : RxJS, localStorage (chatbot)
- **Services** : appels HTTP via `HttpClient`, JWT injecté par un intercepteur
- **Chatbot** : composant dédié + service Angular `chatbot.service.ts`, persistance localStorage

Sous-dossiers inclus :
- `src/app/` — composants, pages, services, modèles par rôle
- `src/assets/` — images, i18n, méd icaments JSON
- `environments/` — variables d’environnement
- `public/` — fichiers statiques
- `coverage/` — rapports de tests