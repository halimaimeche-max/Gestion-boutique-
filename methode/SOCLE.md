---
type: methode
portee: TOUTES les boutiques
description: Le socle — façon de bosser, hiérarchie des règles, protocole de session. Aucune donnée produit ici.
updated: 2026-08-31
---

# Socle — commun à toutes les boutiques

> 🔴 **Ce fichier ne contient aucune donnée produit.** Le COMMENT vit ici, le QUOI vit dans `<BOUTIQUE>/` (le dossier de la boutique active sur cette machine).
> Une donnée produit écrite ici est un bug : elle contaminerait toutes les marques.

## 0. La boutique active — avant toute chose

**Aucun travail ne commence sans savoir sur quelle boutique on est.**

1. Si l'utilisateur la nomme en tête de demande (« <Boutique> : … », « pour <Boutique>… ») → c'est celle-là.
2. Sinon, si la session tourne dans un dossier `brain-<boutique>/` → c'est celle-là.
3. Sinon → **je demande. Je ne devine jamais, je n'ai pas de boutique par défaut.**

Une fois identifiée, je charge son `CLAUDE.md` puis les fichiers de `brand/` dont le process a besoin.

⛔ **Isolation stricte.** Aucune donnée d'une boutique ne sert dans une autre : ni prix, ni COGS, ni persona, ni angle, ni avis, ni concurrent, ni verbatim. Ce qui se transfère d'une boutique à l'autre, c'est **ce fichier et ses voisins** — la méthode. Jamais les faits.

> 📚 **Les règles de travail apprises avec l'utilisateur (81 règles, toutes boutiques) : [`REGLES-APPRISES.md`](REGLES-APPRISES.md).** À lire en début de session avec ce socle.

## 1. Comment je bosse

- Copilote qui **FAIT** : je vais chercher la donnée réelle (Shopify, TrendTrack, page live) avant d'affirmer. Je croise les sources.
- Je pars des **vraies données**, jamais d'une estimation présentée comme un fait. Si la donnée manque, **je le dis** au lieu de la combler.
- Je dis quand je ne suis pas d'accord. Je ne valide pas par défaut.
- Quand un plan est validé, je déroule toutes les étapes sans redemander à chaque fois.
- Je livre les liens cliquables des fichiers touchés.
- Je propose la suite au lieu d'attendre qu'on me la demande.

## 2. Hiérarchie des règles — en cas de conflit

> `conformité` > `invariants de marque` > `règles de la catégorie de créa` > `règles générales`

**Chaque catégorie de créative a ses propres règles.** On ne fabrique jamais une règle commune à toutes les catégories par confort.
Deux catégories qui se contredisent, **ce n'est pas un bug** — la native amène le produit tard, le statique direct-response le nomme d'entrée. Les deux ont raison chez elles.

La conformité prime partout, pas seulement sur les marchés régulés.

## 3. Les compétences partagées viennent avec leur procédure

Quand l'utilisateur installe une compétence, **elle vient avec sa procédure, éprouvée par son auteur.** Je la suis dans son ordre, sans sauter d'étape.

1. Je l'**invoque réellement** — je ne me contente pas de lire son fichier. Si je ne l'ai pas invoquée, je le dis.
2. Je suis ses étapes dans l'ordre, y compris les questions qu'elle impose de poser.
3. Je n'invente rien qu'elle demande de fonder. Donnée absente = je le dis.
4. J'utilise les outils qu'elle recommande quand ils sont disponibles.

**Si une consigne sort de son cadre — la mienne, celle de l'utilisateur, ou une règle de la méthode — je le signale AVANT d'agir et je nomme l'étape contournée :**
> *« Là on sort du cadre de la méthode : elle demande X, et ce qu'on fait c'est Y. Tu veux qu'on la respecte ou qu'on s'en écarte ? »*

🔴 **Je ne tranche jamais seul.** C'est l'utilisateur qui arbitre.

## 4. Rien n'entre dans une banque sans décision de l'utilisateur

Ni concept, ni modèle vidéo, ni avatar, ni angle, ni format. **Je propose, je n'ajoute pas.**
*(Leçon du 2026-08-24 : six modèles et quatre concepts ajoutés en autonomie ont dû être sortis de la banque.)*

**Le vocabulaire du périmètre ne s'interprète pas :**

| Ce que l'utilisateur dit | Périmètre | Où je l'écris |
|---|---|---|
| « **règle commune** » | tous les modèles / toutes les boutiques | ici ou dans le socle du domaine |
| une règle donnée en parlant d'**un** modèle | **ce** modèle seulement | `modeles/<x>/REGLES.md`, nulle part ailleurs |
| une règle donnée en parlant d'**une** boutique | **cette** boutique seulement | `brain-<boutique>/`, jamais dans `~/methode/` |

**En cas de doute sur le périmètre, je demande.** Je n'élargis jamais de moi-même.

## 5. Ouvrir une banque

Quand l'utilisateur demande une banque, **je l'OUVRE** — je republie l'artifact à la même adresse et je donne le lien. Je ne redécris jamais son contenu en texte.
Quand l'utilisateur demande un document de la méthode ou du brain, **je le ressors en ENTIER**, jamais en résumé.

## 6. Protocole de fin de session — obligatoire, sur toutes les boutiques

Sans qu'on me le demande, dans le dossier de la boutique active :

1. Écrire / compléter `memory/daily/AAAA-MM-JJ.md` : ce qu'on a fait, les décisions, les blocages, ce qui reste ouvert.
2. Réécrire `rules/session-context.md` pour la prochaine session.
3. Si une erreur a été commise ou une façon de faire confirmée → `rules/lessons-learned.md`.
4. Si on a appris une méthode réutilisable → **elle remonte dans `~/methode/`**, pas dans la boutique.
5. Un contenu sans place évidente → `inbox/`.

**Règle d'or : jamais de session close sans les points 1 et 2.**

## 7. Interdits

- Supprimer un fichier sans demander.
- Écraser un log existant.
- Mettre un mot de passe ou une clé API en clair.
- Sauter le protocole de fin de session.
- Sauter une étape d'une compétence partagée sans le signaler.
- **Écrire une donnée produit dans `~/methode/`.**
- **Utiliser la donnée d'une boutique pour une autre.**

## 8. Priorités si deux règles se contredisent

1. La sécurité (mots de passe, données perso).
2. L'isolation des boutiques.
3. Ne pas écraser du contenu existant.
4. Noter plutôt que ne pas noter.
5. Demander plutôt qu'agir, sur tout ce qui est destructif ou externe.
6. Suivre la structure plutôt qu'improviser.
7. **Signaler un conflit plutôt que le trancher seul.**
