# Backend — Laravel 10

API REST du projet MedCabinet.

- **Stack** : Laravel 10 + PHP 8.2 + JWT (tymon/jwt-auth)
- **Base de données** : MySQL 8, Redis (cache)
- **IA** : appels à DeepSeek/Gemini/Groq depuis `AiService.php`
- **Intégrations** : Twilio (SMS), SendGrid (email)

Sous-dossiers inclus :
- `app/` — code source (Controllers, Middleware, Models, Services)
- `bootstrap/` — amorçage Laravel
- `config/` — configuration applicative
- `database/` — migrations, seeders, fact