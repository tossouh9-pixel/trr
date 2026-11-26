# Gestion Sous-Traitance (Web)

Interface web prête pour Railway qui lit automatiquement toutes vos tables PostgreSQL (`contrats`, `sous_traitants`, etc.) et permet d'afficher, rechercher, ajouter, modifier et supprimer des lignes.

## Mise en ligne sur Railway (sans ligne de commande)

1. Créez un nouveau dépôt sur GitHub (ex. `sous-traitance-web`).
2. Importez les fichiers de ce dossier (`package.json`, `server.js`, `.gitignore` et le dossier `public/`) via **Add file → Upload files**.
3. Dans votre projet Railway :
   - Cliquez sur **+ Add → GitHub Repository** et choisissez `sous-traitance-web`.
   - Dans ce nouveau service → **Variables**, ajoutez :
     - `DATABASE_URL` = `${{Postgres.DATABASE_URL}}`
     - *(Optionnel recommandé)* `APP_PASSWORD` = un mot de passe pour protéger le site.
   - Dans **Settings → Networking**, cliquez sur **Generate Domain**.
