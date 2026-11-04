# Exigences de sécurité de l'application des notes

| # | Exigence : « Le système doit… » | Vérification | Étape du SDLC | Test |
|---|---|---|---|---|
| 1 | refuser la modification d'une note à toute personne non identifiée (réponse 401) | Test automatique | Exigences | |
| 2 | refuser la modification d'une note à un étudiant (réponse 403) | Test automatique | Conception | |
| 3 | refuser à un enseignant la modification des notes d'un autre module (réponse 403) | Test automatique | Conception | |
| 4 | refuser toute note qui n'est pas un nombre entre 0 et 20 (réponse 400) | Test automatique | Développement | |
| 5 | résister à l'injection SQL dans la recherche par nom | Test automatique + Bandit | Développement | |
| 6 | ne montrer aucun détail technique en cas d'erreur (réponse 500 générique) | Test automatique | Revue de code | |