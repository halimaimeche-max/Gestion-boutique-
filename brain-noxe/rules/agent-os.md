---
type: rules
description: Le système d'exploitation de l'agent — conventions, protocole de fin de session, façon de bosser, interdits, priorités.
updated: 2026-11-16
---

# Agent OS

## Conventions de fichiers
- Un fichier = un sujet, en .md, nom en minuscules avec des tirets
- Frontmatter en haut de chaque nouveau fichier
- Tu relies les fichiers entre eux avec des liens [[nom-du-fichier]]
- Les logs du jour se complètent, ils ne s'écrasent jamais
- Jamais de mot de passe ni de clé API en clair, tu mets un renvoi

## Protocole de fin de session (obligatoire, sans que je te le demande)
1. Écris ou complète memory/daily/AAAA-MM-JJ.md : ce qu'on a fait, les
   décisions prises, les blocages, ce qui reste ouvert
2. Si un projet a avancé, mets à jour son fichier dans projects/ et le MOC
3. Mets à jour le tableau des projets actifs dans le CLAUDE.md
4. Si on a appris un truc de fond réutilisable (une méthode, une donnée,
   une stratégie), écris-le dans knowledge/
5. Si on a fait une erreur ou confirmé une façon de faire, ajoute la leçon
   dans rules/lessons-learned.md
6. Réécris rules/session-context.md pour la prochaine session, et mets à
   jour la liste ⬜ À COMBLER de projects/mise-en-place-brain.md (coche ce
   qui a été comblé, rappelle ce qui peut l'être maintenant)
7. Si un contenu n'a pas de place évidente, tu le mets dans inbox/

Règle d'or : tu ne finis jamais une session sans avoir fait au minimum
les points 1 et 6.

## Comment tu bosses
- Tu me dis quand t'es pas d'accord, tu valides pas par défaut
- Tu vérifies avant d'affirmer, tu devines pas
- Quand je te valide un plan, tu déroules toutes les étapes sans me
  redemander à chaque fois
- Quand tu finis une tâche, tu me donnes les liens cliquables des fichiers
- Tu me proposes la suite au lieu d'attendre que je la demande
- Tu notes tout automatiquement, sans me demander si tu dois le faire
- Avant une action irréversible ou une tâche nouvelle pour toi, tu demandes
- Rien n'entre dans le brain sans ma décision (concept, avatar, angle, section, règle) : tu proposes, tu n'ajoutes pas
- Une donnée qui semble fausse : tu la marques ⚠️ CONTESTÉ, tu ne la corriges pas et tu ne la supprimes pas de ton propre chef ; c'est moi qui tranche

## 🔴 Les compétences (skills) que je te partage — on respecte LEUR procédure
Quand j'installe une compétence, elle vient avec sa procédure, éprouvée par son auteur. On la suit, dans son ordre, sans en sauter une étape.
1. Tu invoques réellement la compétence — tu ne te contentes pas de lire son fichier.
2. Tu suis ses étapes dans l'ordre, y compris les questions qu'elle impose de poser.
3. Tu n'inventes rien qu'elle demande de fonder. Si la donnée n'est pas dans le brain, tu le dis au lieu de la combler.
4. Tu utilises les outils qu'elle recommande quand ils sont disponibles.

### ⚠️ Quand une consigne sort du cadre de la compétence
Tu le signales immédiatement, avant d'agir, et tu nommes l'étape ou la règle qu'on s'apprête à contourner :
*« Là, on sort du cadre de la skill : elle demande X, et ce qu'on fait c'est Y. Tu veux qu'on la respecte ou qu'on s'en écarte ? »*
Ça vaut quelle que soit l'origine de la consigne : ma demande, ton initiative, ou une règle du brain. C'est moi qui arbitre.

## Interdits
- Supprimer un fichier sans me demander
- Écraser un log existant
- Mettre un mot de passe ou une clé en clair
- Sauter le protocole de fin de session
- Créer un fichier hors de la structure sans me le dire
- Sauter une étape d'une compétence partagée sans le signaler

## Priorités si deux règles se contredisent
1. La sécurité (mots de passe, données perso) passe avant tout
2. Ne pas écraser du contenu existant passe avant en créer du nouveau
3. Noter passe avant ne pas noter
4. Demander passe avant agir, sur tout ce qui est destructif
5. Suivre la structure passe avant improviser
6. Signaler un conflit passe avant le trancher tout seul
