# NoteMaster Auth

Page d'authentification Google pour l'application NoteMaster utilisant Supabase.

## À propos

Cette page gère l'authentification Google pour l'application NoteMaster, en contournant les limitations des iframes dans Streamlit Cloud.

## Comment ça fonctionne

1. L'utilisateur clique sur "Se connecter avec Google" dans l'application Streamlit
2. Une nouvelle fenêtre s'ouvre avec cette page d'authentification dédiée
3. L'utilisateur s'authentifie avec Google via Supabase
4. Supabase génère un token d'accès valide
5. La page d'authentification redirige vers l'application Streamlit avec ce token
6. Streamlit vérifie et valide le token avec Supabase
7. L'utilisateur est authentifié et peut accéder à ses données personnelles

## Configuration

Avant d'utiliser cette page, vous devez modifier le fichier `index.html` pour configurer:

1. `SUPABASE_URL` - Votre URL Supabase
2. `SUPABASE_KEY` - Votre clé publique Supabase
3. `STREAMLIT_APP_URL` - L'URL de votre application Streamlit

## Déploiement

Cette page est conçue pour être hébergée sur GitHub Pages.
