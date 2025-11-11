# Règles de contribution (sécurité)
- Aucun secret (tokens, mots de passe, clés) dans le code, l’historique ou les logs.
- Corriger les alertes **SonarLint** dans l’IDE avant commit.
- Les hooks **pre-commit** (Gitleaks + Semgrep) doivent passer.
- Exécuter `mvn verify` en local avant PR si possible.
- Toute exception (faux positif) doit être documentée dans la PR et traitée via config (`gitleaks.toml`, `.semgrepignore`) approuvée par reviewer.
