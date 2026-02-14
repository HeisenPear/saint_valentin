# Projet Saint Valentin

Site statique simple prêt pour déploiement sur Vercel.

Déploiement:

- Connectez le dépôt GitHub à Vercel via https://vercel.com/ en autorisant le dépôt.
- Ou utilisez la CLI Vercel (`vercel`) après l'installation et l'authentification.

Fichiers ajoutés pour Vercel:

- `vercel.json` : configuration de déploiement statique

GitHub Actions (déploiement automatique)

- Un workflow GitHub Actions a été ajouté: `.github/workflows/vercel-deploy.yml`.
- Ce workflow utilise la CLI Vercel pour déployer à chaque `push` sur la branche `main`.
- Configurez les secrets du dépôt GitHub avant d'utiliser le workflow:
  - `VERCEL_TOKEN` (obligatoire) — créez un token sur https://vercel.com/account/tokens
  - `VERCEL_ORG_ID` (optionnel) — identifiant de votre organisation Vercel
  - `VERCEL_PROJECT_ID` (optionnel) — identifiant du projet Vercel

Pour ajouter les secrets : GitHub → Settings → Secrets and variables → Actions → New repository secret.
