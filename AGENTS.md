# AGENTS.md

## Projet

Ce dépôt contient un addon Blender pour exporter des projets vers le format I3D utilisé par GIANTS Engine / Farming Simulator.

## Règles générales

- Ne pas modifier la licence du projet.
- Faire des changements petits, propres et faciles à relire.
- Ne pas modifier le workflow de release sans raison claire.
- Ne pas casser la structure de l’addon dans `addon/i3dio`.
- Si une option visible par l’utilisateur change, mettre à jour la documentation ou le README.
- Toujours expliquer les fichiers modifiés dans le résumé final.

## Version Blender

L’addon déclare sa version Blender minimale dans :

`addon/i3dio/__init__.py`

Avant de changer cette valeur, vérifier que le code reste compatible.

## Commandes de vérification

Après une modification Python, lancer au minimum :

```bash
python -m compileall addon/i3dio
```

Pour tester la création du zip de release :

```bash
./prepare_release.sh 0.0.0-test
```

## Release

Le dépôt utilise semantic-release.

Les commits doivent suivre ce style :

- `feat:` pour une nouvelle fonctionnalité
- `fix:` pour une correction
- `docs:` pour la documentation
- `ci:` pour les workflows GitHub Actions
- `chore:` pour l’entretien du projet

## Pull requests

Avant de proposer une PR :

- vérifier que le code Python compile ;
- vérifier que les fichiers modifiés sont nécessaires ;
- résumer clairement ce qui a changé ;
- indiquer les tests lancés.
