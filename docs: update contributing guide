# Contribuer au projet

Merci de vouloir contribuer à cet addon Blender I3D.

Ce projet contient un addon Blender permettant d’exporter des projets vers le format I3D utilisé par GIANTS Engine / Farming Simulator.

Avant de proposer une modification, merci de lire ce fichier et de garder les changements simples, propres et faciles à relire.

## Avant de commencer

Avant d’ouvrir une issue ou une pull request :

- vérifie si le problème existe déjà dans les issues ;
- utilise le formulaire de rapport de bug si tu signales un bug ;
- explique clairement le problème ou la modification proposée ;
- évite les gros changements mélangés dans une seule pull request.

Un bon changement est petit, compréhensible et testable.

## Signaler un bug

Pour signaler un bug, ouvre une issue avec le modèle **Rapport de bug**.

Merci d’indiquer autant d’informations que possible :

- version de Blender ;
- version de l’addon ;
- système d’exploitation ;
- version Farming Simulator / GIANTS Editor si concernée ;
- étapes pour reproduire le problème ;
- résultat attendu ;
- résultat obtenu ;
- logs ou message d’erreur ;
- capture d’écran ou petit fichier de test si possible.

Un rapport du type “ça ne marche pas” est difficile à corriger.

Un rapport avec des étapes précises permet de trouver le problème beaucoup plus vite.

## Proposer une modification

Pour proposer une correction ou une nouvelle fonctionnalité :

1. Crée une branche dédiée.
2. Fais un changement limité.
3. Vérifie que le code Python compile.
4. Mets à jour la documentation si le comportement utilisateur change.
5. Ouvre une pull request avec une description claire.

Le dépôt contient un modèle de pull request. Merci de le remplir correctement.

## Installation en développement

Méthode simple pour travailler sur l’addon :

1. Clone le dépôt.
2. Ouvre Blender.
3. Installe ou lie le dossier de l’addon depuis :

```text
addon/i3dio
```

4. Active l’addon dans Blender.
5. Redémarre Blender si nécessaire.

Selon ta configuration, tu peux aussi créer un lien symbolique depuis le dossier des addons Blender vers le dossier `addon/i3dio`.

## Vérifications à lancer

Après une modification Python, lance au minimum :

```bash
python -m compileall addon/i3dio
```

Cette commande vérifie que les fichiers Python compilent sans erreur de syntaxe.

Pour tester la création du zip de release :

```bash
./prepare_release.sh 0.0.0-test
```

Attention : cette commande modifie temporairement la version dans l’addon et crée une archive zip. Elle est surtout utile pour vérifier le processus de build.

## Tester dans Blender

Quand le changement touche le comportement de l’addon, il faut aussi tester dans Blender :

- l’addon se charge correctement ;
- les panneaux ou menus modifiés s’affichent ;
- l’export I3D fonctionne si le changement touche l’export ;
- aucune erreur n’apparaît dans la console Blender.

Indique dans la pull request la version de Blender utilisée pour tester.

## Style de code

Merci de respecter ces règles :

- garder le code lisible ;
- éviter les changements inutiles de formatage ;
- ne pas mélanger refactorisation et correction de bug sans raison ;
- nommer les variables clairement ;
- ne pas supprimer du code sans expliquer pourquoi ;
- ne pas modifier la structure de `addon/i3dio` sans nécessité.

## Messages de commit

Le projet utilise semantic-release. Les messages de commit doivent suivre une convention claire.

Exemples :

```text
fix: correct material export crash
feat: add new export option
docs: update installation instructions
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

## Documentation

Si une modification change quelque chose pour l’utilisateur, mets à jour la documentation ou le README.

Exemples :

- nouvelle option dans l’interface ;
- changement dans le comportement d’export ;
- nouvelle compatibilité Blender ;
- nouvelle étape d’installation ;
- changement dans les chemins ou préférences.

## Pull requests

Une pull request doit contenir :

- un résumé clair ;
- le type de changement ;
- les fichiers principaux modifiés ;
- les tests effectués ;
- la version Blender utilisée ;
- l’impact utilisateur éventuel.

Avant de demander une revue :

- vérifie que le code Python compile ;
- supprime les fichiers inutiles ;
- vérifie que la PR ne contient pas de changements sans rapport ;
- complète la checklist de la pull request.

## Releases

Le dépôt utilise semantic-release pour préparer les releases.

Ne modifie pas les fichiers de release sans raison claire :

- `.releaserc.yaml`
- `.github/workflows/release.yml`
- `prepare_release.sh`

Si tu dois modifier le système de release, explique précisément pourquoi dans la pull request.

## Consignes pour les agents IA

Le fichier `AGENTS.md` contient les consignes de travail pour Codex / ChatGPT.

Avant de faire une modification automatisée, il faut respecter les instructions de ce fichier.

## Licence

Ne modifie pas la licence du projet sans discussion préalable.

Les contributions doivent rester compatibles avec la licence existante du dépôt.
