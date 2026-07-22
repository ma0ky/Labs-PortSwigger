# PortSwigger Web Security Academy — Writeups

Writeups persos des labs de la [Web Security Academy](https://portswigger.net/web-security) de PortSwigger, réalisés dans le cadre de ma préparation au métier de pentester.

Chaque writeup détaille la méthodologie utilisée, les requêtes/payloads testés, et le raisonnement derrière chaque étape — pas juste "voici la solution".

## 🎯 Objectif

Documenter ma progression en exploitation web (recon, analyse de vulnérabilité, exploitation, contournement de protections) de façon structurée et réutilisable, dans une logique de portfolio pentest.

## 📁 Structure

```
Labs-Portswigger/
├── 01_SQL_Injection/
│   ├── 00_Start/
│   ├── 01_UNION/
│   ├── 02_Examining_the_database/
│   └── 03_BIND/
├── 02_Authentication/
├── 03_XSS/
├── 04_CSRF/
├── ...
```

Chaque catégorie suit la progression officielle de l'academy (du plus simple au plus avancé). Chaque lab a son propre dossier contenant :

- `ATTAQUE.md` — le writeup (contexte, méthodo, exploitation, résultat)
- Screenshots à l'appui (requêtes, réponses, preuve de résolution)


## 📊 Progression

| Catégorie | Labs résolus | Statut |
|---|---|---|
| SQL Injection | 1/13 | 🟡 En cours |
| Authentication | 0/? | ⬜ À venir |
| XSS | 0/? | ⬜ À venir |
| CSRF | 0/? | ⬜ À venir |

*(tableau à mettre à jour au fil de l'eau)*

## 🛠️ Stack / outils utilisés

- Burp Suite (Community/Pro)
- Navigateur + DevTools
- Notes manuscrites de méthodologie SQLi/XSS/etc.

## ⚠️ Disclaimer

Tous les labs sont réalisés sur l'environnement légal et dédié de PortSwigger (web-security-academy.net). Aucune technique ici ne vise des systèmes réels sans autorisation.

## 🔗 Liens utiles

- [PortSwigger Web Security Academy](https://portswigger.net/web-security)
- [SQL Injection cheat sheet](https://portswigger.net/web-security/sql-injection/cheat-sheet)
