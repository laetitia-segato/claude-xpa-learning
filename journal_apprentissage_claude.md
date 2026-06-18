# Journal d apprentissage Claude (version A)

> Document vivant. À mettre à jour à la fin de chaque session (5 minutes suffisent).
> Versionner dans Git dès la Phase 1. Ce journal EST ta trace.

---

## Métadonnées

- **Date de démarrage** : 2026-04-23
- **Phase en cours** : Phase 1
- **Heures cumulées** : 7.75 h
- **Dernière session** : 2026-05-22
- **Prochaine étape prévue** : Phase 1 Bloc B suite — branches, GitHub, push, PR, conflit
- **Repo GitHub du parcours** : _à compléter après Phase 1_

---

## Suivi des phases (vue d'ensemble)

| Phase | Titre | Statut | Heures estimées | Heures réelles | Date début | Date fin |
|-------|-------|--------|-----------------|----------------|------------|----------|
| 0 | Écosystème Claude | ✅ terminé  | 5.5 h | |2026-04-23|2026-05-06|
| 1 | Fondations dev modernes | ⏳ en cours | 15 h | | | |
| 2 | Maîtrise de Claude Code | ⬜ À faire | 15 h | | | |
| 3 | Consommer et créer des APIs | ⬜ À faire | 25 h | | | |
| 4 | Déployer et maintenir | ⬜ À faire | 25 h | | | |
| 5 | MCP — brancher Claude sur tes systèmes | ⬜ À faire | 20 h | | | |
| 6 | Capstone | ⬜ À faire | 30 h | | | |

Légende : ⬜ à faire · ⏳ en cours · ✅ terminé · ⚠️ bloqué

---

## Checklist détaillée par phase

### Phase 0 — Écosystème Claude

- [x] Compte Claude.ai créé, Projets explorés
- [x] Doc prompt engineering lue (une fois suffit)
- [x] 10 prompts de code testés avec explication "comme à un dev XPA"
- [x] Différence claire entre Claude.ai / Claude Code / API
- [x] Checkpoint atteint : je sais quel outil Claude choisir pour chaque tâche

### Phase 1 — Fondations dev modernes

- [x] Terminal installé (WSL2 Ubuntu / iTerm / autre)
- [x] 20 exercices shell faits
- [ ] Git installé + compte GitHub
- [ ] 10 commits sur plusieurs branches, 1 PR, 1 merge conflict résolu
- [ ] Python 3.12+ et uv installés
- [ ] Bases Python : types, fonctions, classes, modules, venv, async
- [ ] Mini-projet CSV fait à la main puis comparé avec Claude
- [ ] Checkpoint atteint : clone + branche + commit sans chercher les commandes

### Phase 2 — Maîtrise de Claude Code

- [ ] Claude Code installé
- [ ] Extension VS Code installée
- [ ] Premier CLAUDE.md écrit
- [ ] Calculatrice + tests faite avec Claude Code
- [ ] Refactor d'un script de 200 lignes
- [ ] README généré à partir d'un code existant
- [ ] Workflow Git complet piloté via Claude Code
- [ ] Projet open-source analysé (architecture expliquée)
- [ ] Bug volontaire corrigé via tests
- [ ] Checkpoint atteint : projet Git propre construit à 80 % par Claude Code, chaque fichier expliqué

### Phase 3 — APIs

- [ ] HTTP/REST : méthodes, codes, headers, body compris
- [ ] Outil API installé (Bruno recommandé)
- [ ] Client Python pour 3 APIs tierces (Open-Meteo, GitHub, une avec OAuth)
- [ ] Tuto FastAPI "First Steps" + "Path" + "Body" fait
- [ ] Mini-CRM : modèles Pydantic, CRUD complet
- [ ] Tests pytest avec couverture > 80 %
- [ ] SQLAlchemy / SQLModel branché (SQLite)
- [ ] Auth JWT ajoutée
- [ ] Audit API par Claude demandé et issues corrigées
- [ ] Checkpoint atteint : API publique sur GitHub, docs OpenAPI, tests, auth

### Phase 4 — Déploiement

- [ ] Concepts Docker compris, API dockerisée
- [ ] docker-compose avec PostgreSQL fonctionnel
- [ ] Déploiement cloud (Railway / Fly.io / autre) avec HTTPS
- [ ] BDD PostgreSQL managée branchée
- [ ] GitHub Actions : lint + test + build + deploy auto
- [ ] Logs structurés + Sentry
- [ ] 1 dépendance majeure mise à jour via Claude Code
- [ ] 1 erreur Sentry diagnostiquée et corrigée via Claude Code
- [ ] Checkpoint atteint : API en ligne, CI/CD < 5 min, monitoring actif

### Phase 5 — MCP

- [ ] Concepts MCP compris (host/client/server, tools/resources/prompts)
- [ ] 1 MCP existant testé dans Claude Desktop / Claude Code
- [ ] Tuto "weather server" officiel fait
- [ ] MCP server perso pour le mini-CRM écrit (tools : list_clients, create_client, …)
- [ ] MCP branché à Claude Desktop, commandes en langage naturel fonctionnelles
- [ ] Bonus : MCP déployé en HTTP/SSE avec auth
- [ ] Bonus : Agent SDK exploré
- [ ] Checkpoint atteint : serveur MCP en prod qui pilote l'API

### Phase 6 — Capstone

- [ ] Projet choisi et cadré (scope, livrables)
- [ ] Code sur GitHub, README complet
- [ ] CI verte
- [ ] Déployé en ligne
- [ ] Documentation rédigée
- [ ] Post de blog / doc interne écrit

---

## Journal de sessions

> À chaque fin de session, ajoute une entrée. Format court, pas de littérature.

### Session n°1 — 2026-04-23 — Durée : ~1 h

- **Phase** : 0 — Écosystème Claude
- **Ce que j'ai fait** :
  - Modèle mental des 5 surfaces Claude (Claude.ai, Claude Code, API, Agent SDK, Chrome/Excel)
  - Quiz de routage des surfaces : 3/3
  - Exploration des paramètres Claude.ai (Projects, Styles, Settings, Connectors)
  - 2 premiers prompts de code "à la XPA" : typage Python + listes/dicts
  - Écriture d'une première structure `list[dict]`
- **Ce que j'ai appris** :
  - Python est dynamiquement typé, mais les type hints sont la norme pro (FastAPI en dépend)
  - `list[dict]` = structure tabulaire standard (mappe SQL, JSON, CSV)
  - Conventions : clés en anglais, snake_case, pas d'accents
- **Ce qui m'a bloqué** : rien de bloquant
- **Artefacts produits** : aucun (session conceptuelle)
- **Prochaine étape** : concepts 3 à 5 des 10 prompts (fonctions, classes, modules) + commencer la doc prompt engineering officielle
  -

---

### Session n°2 — 2026-04-23 — Durée : ~30 min

- **Phase** : 0 — Écosystème Claude
- **Ce que j'ai fait** :
  - Concept n°3 des 10 prompts : fonctions Python
  - Prompt sur Claude.ai avec analogie XPA (sous-tâche / User Function)
  - Exercice pratique : écrit une fonction `calculer_remise` avec valeur par défaut et return multiple
  - 3 modes d'appel testés (position implicite, position explicite, par nom)
- **Ce que j'ai appris** :
  - L'indentation Python est syntaxique : 4 espaces, jamais de tab
  - `return a, b` crée un tuple ; il faut l'unpacker (`m, f = calculer_remise(...)`) pour récupérer les valeurs séparément
  - Équivalent des arguments nommés XPA mais plus souple (position OU nom)
- **Ce qui m'a bloqué** : mélange tab/espaces invisible dans l'éditeur ; oubli que le retour multiple = un tuple unique
- **Artefacts produits** : aucun (snippet dans le chat)
- **Prochaine étape** : concept n°4 — classes (avec analogie Business Components XPA)

---

### Session n°3 — 2026-04-23 — Durée : ~45 min

- **Phase** : 0 — Écosystème Claude
- **Ce que j'ai fait** :
  - Concept n°4 des 10 prompts : classes Python
  - Prompt sur Claude.ai avec analogie XPA (j'ai trouvé moi-même : classe ≈ tâche XPA)
  - Exercice pratique : classe `Produit` avec `__init__`, méthode `prix_ttc`, méthode `afficher`
  - 2 instances créées et appelées
  - Itérations correctives : redondance self/paramètre, écrasement de méthode, oubli des `:`, appel de méthode sans `()`
- **Ce que j'ai appris** :
  - `class` + `__init__(self, ...)` = constructeur, `self` = l'instance courante
  - Une méthode utilise `self.attribut` au lieu de redemander les attributs en paramètre
  - `obj.methode` ≠ `obj.methode()` : sans parenthèses, on référence la fonction sans l'exécuter
  - Les f-strings (`f"..{var}.."`) pour formater
  - Les floats ont des arrondis traîtres (1.5 * 1.20 ≠ 1.80 exact) → utiliser `Decimal` pour la monnaie
- **Ce qui m'a bloqué** : confusion entre attributs/paramètres, oubli du `:` après `def`, oubli des `()` à l'appel
- **Artefacts produits** : snippet classe `Produit` (dans le chat)
- **Prochaine étape** : concept n°5 — modules et imports (analogie composants/programmes XPA)

---

### Session n°4 — 2026-05-06 — Durée : ~2 h

- **Phase** : 0 — Écosystème Claude
- **Ce que j'ai fait** :
  - Concept n°5 : modules et imports (analogie module ≈ programme XPA, package ≈ composant)
  - Concept n°6 : environnements virtuels (.venv, uv, pyproject.toml, uv.lock)
  - Concept n°7 : exceptions (try/except, EAFP, exercice `demander_age`)
  - Concept n°8 : list comprehensions (exercice : labels des produits chers)
  - Concept n°9 : async/await — vue de culture, mots-clés reconnus
  - Concept n°10 : décorateurs — vue de culture, lien avec FastAPI vu
- **Ce que j'ai appris** :
  - 2 styles d'import (`import x` vs `from x import y`), trade-offs
  - Trio Python moderne : `pyproject.toml` (recette) + `uv.lock` (versions exactes) + `.venv/` (jamais commit)
  - EAFP : on tente, on rattrape — plutôt que de vérifier en amont
  - `except` doit être précis ; `except:` tout nu masque les bugs
  - List comprehension = SELECT projeté+filtré sur une liste mémoire
  - Décorateurs = chapeaux sur une fonction (clé pour FastAPI)
- **Ce qui m'a bloqué** : confusion clés de dict / variables dans la list comprehension (premier essai)
- **Artefacts produits** : snippets `demander_age` et list comprehension produits chers
- **Prochaine étape** : lire la doc officielle de prompt engineering + valider le checkpoint Phase 0

---

### Session n°5 — 2026-05-06 — Durée : ~30 min

- **Phase** : 0 — Écosystème Claude (CLÔTURE)
- **Ce que j'ai fait** :
  - Lecture de la doc officielle "Prompting best practices" (section General principles)
  - Identification rétrospective des techniques déjà utilisées dans mes propres prompts
  - Validation des derniers items de la checklist Phase 0
- **Ce que j'ai appris** :
  - 6 techniques fondamentales nommées : be clear and direct, add context, use examples (few-shot), XML tags, give Claude a role, long context
  - J'utilisais déjà "be clear and direct", "give a role" et "add context" sans le savoir
  - Les XML tags vont devenir clés dès que mes prompts dépasseront 10 lignes
  - Multishot (2-3 exemples concrets) > consignes verbales pour des transformations de données
- **Ce qui m'a bloqué** : la doc a été restructurée depuis le programme (1 page unique au lieu de sous-pages)
- **Artefacts produits** : aucun
- **Prochaine étape** : Phase 1 — installer terminal/WSL2, Git, Python+uv

---

### Session n°6 — 2026-05-15 — Durée : ~45 min

- **Phase** : 1 — Fondations dev modernes (Bloc A : Terminal)
- **Ce que j'ai fait** :
  - Installé WSL2 + Ubuntu sur Windows 11 (en 2 étapes : `wsl --install` puis `wsl --install -d Ubuntu`)
  - Compris la structure du prompt Linux (`user@machine:chemin$`)
  - 12 premières commandes shell tapées à la main : `pwd`, `cd`, `ls`, `ls -a`, `mkdir`, `touch`, `echo`, `cat`, `grep`, `wc`, redirections `>` et `>>`, pipe `|`
  - Création de `/home/laetitia/projets/hello.txt` avec contenu
  - Première chaîne de traitement avec un pipe : `cat | grep`, `cat | wc -l`
- **Ce que j'ai appris** :
  - WSL2 = vraie machine Linux dans Windows, partage le système de fichiers via `/mnt/c/`
  - On travaille dans `/home/<user>` pour le dev, pas dans `/mnt/c/`
  - Les fichiers cachés Linux commencent par `.` (`.bashrc`, `.profile`, etc.)
  - `>` écrase, `>>` ajoute — à ne pas confondre
  - Le pipe `|` chaîne des programmes (philosophie Unix : petits outils combinables)
  - Les messages d'erreur Linux sont littéraux, à lire au lieu de paniquer
- **Ce qui m'a bloqué** :
  - Installation Ubuntu n'a pas démarré seule après `wsl --install` → fallu relancer avec `wsl --install -d Ubuntu`
  - Confusion `-1` (chiffre) vs `-l` (lettre L) dans `wc -l`
- **Artefacts produits** : dossier `~/projets/` + fichier `hello.txt` dans WSL2
- **Prochaine étape** : suite Bloc A (rm, mv, cp, which, variables env, curl) puis Bloc B (Git + GitHub)

---

### Session n°7 — 2026-05-15 — Durée : ~45 min

- **Phase** : 1 — Fondations dev modernes (Bloc A : Terminal, fin)
- **Ce que j'ai fait** :
  - Fin du Bloc A : `cp`, `mv`, `rm`, `rm -r` (avec règle d'or "pas de corbeille sous Linux")
  - `which` pour localiser les commandes installées
  - Variables d'environnement : `$HOME`, `$USER`, `$PATH`, `$SHELL`
  - Premier appel HTTP avec `curl` sur api.github.com/zen
  - Lecture des headers HTTP avec `curl -i` (HTTP/2 200, rate limits, sécurité)
  - Découverte des 3 méthodes pour relancer WSL (menu Démarrer, Windows Terminal, `wsl` depuis PowerShell)
- **Ce que j'ai appris** :
  - Python 3 et Git sont préinstallés sur Ubuntu WSL2 (vérifié avec `which`)
  - `$PATH` WSL2 mélange chemins Linux ET Windows → je peux lancer des commandes Windows depuis Ubuntu
  - `rm` n'a PAS de corbeille → vérifier avec `ls` avant de supprimer
  - `cp/mv` même mécanique : renommer = déplacer dans le même dossier
  - Une réponse HTTP brute contient un status code + des headers (vu en vrai, prélude Phase 3)
  - Si je ne suis pas dans le bon dossier, la commande plante (réflexe `pwd` avant toute action sur fichiers)
- **Ce qui m'a bloqué** :
  - Lancé `cp hello.txt` depuis `~` au lieu de `~/projets` → "No such file or directory"
- **Artefacts produits** : aucun nouveau (manipulation de `hello.txt` existant)
- **Prochaine étape** : Bloc B — Git + GitHub (config git, compte GitHub, premier repo, branches, merge, conflit)

---

### Session n°8 — 2026-05-22 — Durée : ~50 min

- **Phase** : 1 — Fondations dev modernes (Bloc B : Git, première moitié)
- **Ce que j'ai fait** :
  - Vérifié Git préinstallé (v2.53)
  - Configuré Git : `user.name`, `user.email`, `init.defaultBranch=main`
  - Créé le dossier `~/projets/claude-xpa-learning/`
  - Copié le journal depuis OneDrive vers WSL via drag-and-drop dans Explorer (`explorer.exe .`)
  - Premier `git init` → création du `.git/` caché
  - Premier `git status` (fichier untracked)
  - Premier `git add` (fichier passé en staging)
  - Premier `git commit` (hash c9e9358 sur branche main)
  - Premier `git log` (historique visible)
- **Ce que j'ai appris** :
  - Le modèle mental des **3 zones Git** : Working Directory → Staging Area → Repository
  - Git affiche systématiquement la prochaine étape suggérée → lire ses messages
  - Une commande Linux qui réussit est souvent silencieuse (`git add` n'affiche rien)
  - `HEAD` = pointeur sur "où je suis dans l'historique" ; il pointe sur la branche courante (`main`)
  - Un hash de commit = empreinte cryptographique infalsifiable du contenu
  - `explorer.exe .` lance l'Explorateur Windows sur le dossier Linux courant (pont WSL)
- **Ce qui m'a bloqué** : rien de bloquant cette session
- **Artefacts produits** : repo Git local `~/projets/claude-xpa-learning/` avec 1 commit
- **Prochaine étape** : Bloc B suite — plusieurs commits, branches, créer compte GitHub, push, PR, conflit

---

<!-- Dupliquer ce bloc pour chaque nouvelle session -->

---

## Questions ouvertes à creuser

> Liste des trucs qui t'ont intrigué mais que tu ne veux pas explorer maintenant.
> Reviens-y quand tu as un trou entre deux phases.

- [ ] _exemple : comment fonctionnent les hooks Claude Code en détail ?_
- [ ]
- [ ]

---

## Aha moments

> Les déclics importants. Un par ligne. Date optionnelle.

- 2026-04-23 — En Python, `return a, b` c'est un tuple déguisé, pas deux valeurs indépendantes. L'unpacking (`x, y = f()`) est la clé.
- 2026-04-23 — En Python, une classe ≈ une tâche XPA : données (attributs) + comportements (méthodes) regroupés.
- 2026-04-23 — `obj.method` retourne la fonction elle-même, `obj.method()` l'exécute. Confusion fréquente.
- 2026-04-23 — Le trio Python moderne : pyproject.toml = recette versionnée, uv.lock = versions exactes versionnées, .venv/ = jamais versionné.
- 2026-04-23 — En Python on attrape une erreur précise (ValueError) qu'on sait gérer, jamais "tout".
- 2026-04-23 — Une list comprehension, c'est un SELECT SQL projeté+filtré en une ligne.
- 2026-05-06 — Mes propres prompts utilisaient déjà 3 techniques officielles sans le savoir : clarté, contexte, rôle. Le travail consiste maintenant à structurer (XML) et à donner des exemples (multishot).
- 2026-05-15 — Le pipe `|` en Linux, c'est de la composition de programmes. Aucun équivalent direct en XPA. Permet d'assembler des Lego d'outils pour fabriquer un traitement.
- 2026-05-15 — WSL2 mélange les deux mondes dans $PATH : depuis Ubuntu je peux lancer notepad.exe ou code.exe. Pont magique Windows ↔ Linux.
-    2026-05-22 — Git, c'est 3 zones : ton dossier (working) → la table de préparation (staging) → l'historique gravé (repository). `git add` puis `git commit` fait le pont entre les 3. Aucun équivalent XPA — ici c'est toi qui choisis ce qui rentre dans chaque "photo".

---

## Ressources sauvegardées

> Liens utiles découverts en route, que tu veux garder.

- Doc officielle Claude : https://docs.claude.com
- Doc Claude Code : https://code.claude.com/docs/en/overview
- MCP : https://modelcontextprotocol.io
- FastAPI : https://fastapi.tiangolo.com
- Anthropic Cookbook : https://github.com/anthropics/anthropic-cookbook
- _ajouter tes propres liens ici_

---

## Rétrospectives mensuelles

> Une fois par mois, prends 15 minutes pour faire le bilan.

### Mois 1 — AAAA-MM

- **Ce qui a bien marché** :
- **Ce qui a moins bien marché** :
- **Ajustements pour le mois prochain** :
- **Heures totales du mois** : X h

---

## Idées de projet Capstone (à creuser)

- Passerelle API entre une base XPA et une app moderne
- Assistant Claude pour la maintenance de programmes XPA
- Outil interne avec front + API + MCP

## Liens utiles XPA → moderne

- Documentation XPA officielle : à compléter
- Forum Magic XPA developers : à compléter
- Articles parallèle XPA / Python : à compléter
