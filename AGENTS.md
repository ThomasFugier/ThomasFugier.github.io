# AGENTS.md

Ce document donne les consignes de travail pour les IA et agents qui interviennent sur ce repo.

## Objectif du repo

Portfolio / site personnel de Thomas Fugier.

## Règle de départ

Avant de modifier quoi que ce soit, un agent doit lire ce fichier entièrement.

## Principes de travail

- Faire des changements ciblés et minimaux.
- Respecter le style visuel et la structure déjà en place.
- Ne pas réécrire des sections non demandées.
- Ne jamais revert des changements utilisateur sans demande explicite.
- Vérifier desktop et mobile quand une section visuelle est modifiée.

## Fichiers temporaires et artefacts de debug

Si une IA a besoin de générer des fichiers temporaires pour tester, débugger ou inspecter le site, elle doit les créer dans un dossier dédié à la racine du repo :

- `.agent-temp/`

Cela inclut notamment :

- screenshots
- captures desktop/mobile
- exports de debug
- profils navigateur temporaires
- fichiers HTML intermédiaires
- logs temporaires

## Règles pour `.agent-temp/`

- Ne rien générer à la racine du repo en dehors de ce dossier.
- Ne pas créer de fichiers du type `.codex-*` ou autres artefacts temporaires dispersés dans le projet.
- Si le dossier `.agent-temp/` n'existe pas, le créer avant de générer ces fichiers.
- Utiliser des noms explicites et regroupés par tâche si possible.
- Nettoyer les fichiers temporaires à la fin du travail quand c'est approprié.
- Si le nettoyage implique une suppression de fichiers locaux, demander confirmation à l'utilisateur si nécessaire selon les règles de l'agent.

## Changements frontend

- Préserver le langage visuel global du site.
- Favoriser des layouts lisibles, cohérents et responsives.
- Éviter les effets décoratifs gratuits ou les interfaces qui ressemblent à un template générique.
- En cas de doute sur une direction visuelle, préférer la sobriété et la clarté.

## Vérification

Quand une modification visuelle est faite :

- vérifier le rendu desktop
- vérifier le rendu mobile
- vérifier qu'aucun texte important ne déborde
- vérifier que les CTA restent visibles et bien positionnés

## Portée

Ces instructions s'appliquent à tout agent IA travaillant dans ce dépôt, quel que soit l'outil utilisé.
