# I3D Blender Addon

Addon Blender communautaire pour exporter des projets vers le format **I3D**, utilisé par **GIANTS Engine** et **Farming Simulator**.

Ce dépôt est une version maintenue / adaptée du projet I3D Blender Addon.  
L’objectif est de garder un exporter utilisable avec les versions récentes de Blender et de faciliter le travail de modding pour Farming Simulator.

## Statut du projet

Ce dépôt est en cours de maintenance.

Les objectifs principaux sont :

- maintenir la compatibilité avec les versions récentes de Blender ;
- corriger les bugs d’export ;
- améliorer la documentation ;
- garder un processus de contribution propre ;
- faciliter le travail avec Codex / ChatGPT pour les corrections et améliorations.

## Fonctionnalités

L’addon permet d’exporter des scènes Blender vers le format I3D utilisé par GIANTS Engine.

Selon les versions et les fichiers utilisés, il peut notamment gérer :

- objets 3D ;
- meshes ;
- matériaux ;
- lumières ;
- attributs utilisateur ;
- options d’export ;
- éléments nécessaires au modding Farming Simulator.

Certaines fonctionnalités peuvent dépendre de la version de Blender, de Farming Simulator ou de GIANTS Editor utilisée.

## Compatibilité

La version minimale de Blender est déclarée dans le fichier :

```text
addon/i3dio/__init__.py
```

Avant de signaler un bug, merci de vérifier :

- la version de Blender utilisée ;
- la version de l’addon ;
- le système d’exploitation ;
- la version Farming Simulator / GIANTS Editor si le problème concerne l’export ou l’import.

## Installation

Méthode générale :

1. Télécharge le fichier zip de l’addon depuis les releases du dépôt.
2. Ouvre Blender.
3. Va dans :

```text
Edit > Preferences > Add-ons
```

4. Clique sur **Install**.
5. Sélectionne le fichier zip de l’addon.
6. Active l’addon dans la liste des addons Blender.
7. Redémarre Blender si nécessaire.

## Installation en développement

Pour travailler sur le code :

1. Clone le dépôt.
2. Ouvre Blender.
3. Installe ou lie le dossier :

```text
addon/i3dio
```

4. Active l’addon dans Blender.
5. Lance les vérifications Python après modification.

Commande minimale de vérification :

```bash
python -m compileall addon/i3dio
```

## Téléchargement

Quand des releases sont disponibles, elles sont accessibles depuis la page **Releases** de ce dépôt.

Le fichier d’addon est généralement fourni sous forme de zip.

## Signaler un bug

Pour signaler un problème :

1. Va dans l’onglet **Issues**.
2. Clique sur **New issue**.
3. Choisis le modèle **Rapport de bug**.
4. Remplis les informations demandées.

Merci d’inclure :

- version de Blender ;
- version de l’addon ;
- système d’exploitation ;
- version Farming Simulator / GIANTS Editor si concernée ;
- étapes pour reproduire ;
- résultat attendu ;
- résultat obtenu ;
- logs ou message d’erreur ;
- capture d’écran ou fichier de test si possible.

Un bug bien décrit se corrige beaucoup plus vite qu’un simple “ça ne marche pas”.

## Contribuer

Les contributions sont les bienvenues.

Avant de proposer une modification, lis le fichier :

```text
CONTRIBUTING.md
```

Le dépôt contient aussi :

```text
AGENTS.md
.github/pull_request_template.md
.github/ISSUE_TEMPLATE/bug_report.yml
.github/workflows/check.yml
```

Ces fichiers servent à garder un projet propre, compréhensible et plus facile à maintenir.

## Vérifications automatiques

Le dépôt utilise GitHub Actions pour vérifier automatiquement le code Python.

Le workflow principal lance :

```bash
python -m compileall addon/i3dio
```

Ce contrôle permet de détecter les erreurs de syntaxe Python avant d’aller plus loin.

## Releases

Le dépôt utilise un système de release automatisé basé sur semantic-release.

Les fichiers liés aux releases sont notamment :

```text
.releaserc.yaml
.github/workflows/release.yml
prepare_release.sh
```

Merci de ne pas modifier ces fichiers sans raison claire.

## Messages de commit

Merci d’utiliser des messages de commit clairs.

Exemples :

```text
fix: correct export crash
feat: add new export option
docs: update README
ci: add workflow check
chore: clean project files
```

Types courants :

- `feat:` nouvelle fonctionnalité ;
- `fix:` correction de bug ;
- `docs:` documentation ;
- `ci:` GitHub Actions / intégration continue ;
- `chore:` entretien du projet ;
- `refactor:` nettoyage ou restructuration sans changement fonctionnel ;
- `test:` ajout ou modification de tests.

## Projet original

Ce dépôt est basé sur le travail communautaire autour de l’exporter I3D Blender.

Crédits historiques :

- StjerneIdioten ;
- GIANTS Software ;
- Jason Oppermann ;
- contributeurs communautaires.

Merci aux développeurs et contributeurs qui ont permis à cet addon d’exister.

## Licence

Ce projet conserve la licence du projet d’origine.

Merci de ne pas modifier la licence sans discussion préalable.
