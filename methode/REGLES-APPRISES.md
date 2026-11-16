---
type: methode
portee: TOUTES les boutiques
description: Les règles de travail apprises avec l'utilisateur (corrections, décisions, constats de production), démarquées de toute donnée de marque. Se lit en début de session, sur n'importe quelle boutique, en plus du SOCLE.
updated: 2026-10-06
source: règles de travail apprises en production réelle (07/2026 → 10/2026), démarquées de toute donnée de marque.
---

# Règles apprises — communes à toutes les boutiques

> 🔴 Ces règles ont toutes été **posées ou corrigées par l'utilisateur**. Elles valent sur chaque boutique.
> ⛔ **Aucune donnée de marque ici.** Les exemples d'origine (produit, prix, avatars) restent dans le brain de leur boutique.
> Une correction de l'utilisateur **remplace définitivement** l'erreur : je ne refais jamais deux fois la même faute.
> Quand une règle est inversée, je garde **le chemin et la raison** du revirement dans le fichier concerné, sinon la question se rouvre.

---

## 1. Relation de travail

1. **Je lis la source réelle, en entier.** Si un outil échoue, je contourne (attendre, autre navigateur, endpoint `.json`, retry). Je ne me rabats jamais sur une source de substitution sans le dire.
2. **Zéro question dont la réponse est déjà dans les sources** qu'il m'a pointées. Je récupère d'abord, je demande ensuite.
3. **Je ne redemande jamais un fichier que le brain possède.** Un fichier sur le disque s'envoie seul à l'outil.
4. **Je vérifie avant d'affirmer, même quand je suis sûr** (sources citées, consignées dans le brain).
5. **Je ne parle jamais en code.** La première fois que j'emploie une abréviation ou un système de codes, je le déroule en français avec un exemple.
6. **Un document de référence qu'il me donne (fournisseur, MSDS, facture, formation) entre dans le brain le jour même, en entier, et traduit en français s'il est en anglais** (l'original est gardé à côté).
7. **Ressortir un document du brain = le restituer EN ENTIER**, jamais en résumé.
8. **Délégation en langage naturel** : les agents se lancent sur une phrase, sans slash command. Avant de construire un outil, vérifier que la capacité n'existe pas déjà.
9. **Cohérence du brain** : quand une règle nouvelle contredit un ancien fichier, je corrige l'ancien **le jour même**. Exception : une donnée factuelle produit/business ne se retourne jamais en silence — je la marque contestée et l'utilisateur tranche.
10. **Protocole d'entrée** : le `CLAUDE.md` d'un brain n'est pas chargé automatiquement. Avant tout livrable : `CLAUDE.md` du brain → `rules/session-context.md` → `rules/lessons-learned.md` → **ce fichier** → la skill concernée, **suivie bloc par bloc comme une checklist**. Entre ce que je crois savoir et ce qui est écrit, **le fichier gagne**.
11. **Une skill dédiée s'ouvre avant de produire, elle ne se reconstruit pas de mémoire.** J'invoque la skill qui porte le déclencheur et je m'arrête au palier en cours. Un livrable en avance de trois paliers est du travail à jeter.
12. **Le périmètre d'une consigne est exactement ce dont on parle.** Une règle donnée pour un modèle, un format ou une boutique ne sort pas de là. « Règle commune » = partout ; sinon, en cas de doute, je demande. Je n'élargis jamais un mandat.
13. **Rien n'entre dans une banque sans sa décision** (voir SOCLE §4). Une intention large (« plein de modèles ») est une direction, pas un mandat pour remplir. Ce que je propose de mon cru est marqué comme tel dans le fichier. Pas de commentaire décoratif dans une interface.

## 2. Fabrication d'une image (statique et native)

14. **Le format de travail est le CARRÉ 1:1 (2048×2048).** Les autres formats viennent après validation.
15. **🛑 Un seul visuel d'abord, validé par l'utilisateur, puis le reste.** Jamais les 3 formats ni l'adcopy avant son OK.
16. **Une passe par visuel, puis on reste dessus.** Pas de variantes « au cas où ». Un visuel validé est figé : je corrige ce qui est signalé, pas ce qui pourrait l'être.
17. **Limite de 4 passes — aussi pour un concept.** Au-delà, je change de scène ou de procédé, je ne continue pas à régler.
18. **Décliner un format = PROLONGER l'image**, jamais la couper ni la border. Canevas au format cible, carré au centre, bandes à compléter par le générateur (« garde le centre, continue la scène »). Les safe zones sont pour le texte, pas pour l'image.
19. **Typo gros et gras** : titres à partir de ~150 px sur 2048, jamais fine. Gras éditorial, pas « affiche de sport ».
20. **Une statique dont le texte est trop petit est morte.** Avant de produire une référence, je vérifie la lisibilité sur téléphone (et en 9:16) ; trop de texte → je réduis ou je déconseille.
21. **Le texte d'une créa ne se génère pas, il se pose au montage** quand l'orthographe ou les chiffres comptent : scène générée avec le support vierge, texte posé en HTML (Chrome headless). Après toute repasse de la scène, je recale le texte.
22. **Écriture manuscrite :** police Google Fonts **Caveat**, décalage **par mot** uniquement (rotation ±1,6°, hauteur ±4 px, échelle ±5 %, nuance d'encre). Plus j'ajoute d'irrégularité, plus ça se voit. Les polices manuscrites du Mac sont à proscrire. Le trait doit concorder avec l'instrument visible (Bic = fin, marqueur = épais).
23. **Un dessin complexe ne se trace pas en SVG** : générer le croquis seul sur fond blanc, le détourer (alpha = 255 − luminance), puis le poser.
24. **Le vrai produit, toujours, en référence image-to-image.** Jamais un produit inventé. Sur un concept stylisé (clay, 3D, BD), le produit est **rendu dans la matière et la lumière de la scène**, jamais le packshot photo collé.
25. **Jamais de collage/swap de produit dans l'image d'un autre produit** : on génère le produit dans la scène (référence = packshot seul), puis on retouche CETTE image.
26. **Le vrai logo (fichier), jamais la marque écrite en police générique**, et toujours en contraste avec le fond. La marque n'est pas obligatoire partout.
27. **Adapter une référence apportée par l'utilisateur = la COPIER** : police, couleurs, blocs, mise en page. Je ne change que le produit et le décor. La DA de la marque ne s'applique que s'il le demande.
28. **Pour une créa originale, la DA est un ESPRIT, pas une charte** : liberté de typo, couleurs, composition. Seules obligations : le vrai produit et le vrai logo.
29. **Variété obligatoire** : jamais le même template d'une créa à l'autre (Meta regroupe les créas qui se ressemblent et n'en garde qu'une). Oser l'atypique.
30. **Règles de scène :** éléments graphiques (post-it, étiquettes) droits et face caméra ; annotations dessinées SUR leur support et contenues dedans ; scène physiquement cohérente et qui se lit comme le lieu demandé ; produit bien visible, un seul, jamais en double ; **pas de props non demandés** (ultra naturel) ; mot accentué en couleur vive et lisible sur son fond.
31. **Statique : le message attribue le résultat au produit** (le produit est nommé). ⚠️ Règle de la statique uniquement — la native fait l'inverse.
32. **Un bénéfice négatif seul sonne creux** → le tourner en comparaison.
33. **Recadrer une référence sur ce qu'on veut conserver** : une référence ramène tout ce qu'elle contient. Une ancre de personnage se génère **sur fond vide**.
34. **Image partagée par l'utilisateur dans le chat → je la descends sur le disque** et je l'utilise en image-to-image. La décrire avec des mots ne la remplace jamais.
35. **Âge des visages :** « visage lisse » fait rajeunir. Sculpter l'âge explicitement (paupières, sillons, ovale) ; les cheveux longs détachés rajeunissent ; en macro, verrouiller l'âge en toutes lettres. Je contrôle l'âge apparent avant de livrer.
36. **Jamais de visage en noir et blanc. Chaque nouvelle vidéo propose un nouveau casting. Aucun produit concurrent dans l'image.**
37. **Jamais de marque, studio ou film réel dans un prompt** : je décris le style par ses attributs.
38. **Texte généré sur un packaging = risque factuel** : moins il y a de texte à générer, moins il y a d'erreurs. Aucun chiffre généré ne doit atteindre la diffusion sans contrôle.

## 3. Banques et rangement

39. **Quand l'utilisateur demande une banque, je l'OUVRE** (je republie l'artifact, je donne le lien) — **toujours à la MÊME adresse**. Je ne redécris pas son contenu.
40. **Vignettes de banque = carré natif** (le 1:1 de la créa). Artifact, pas widget ; bouton « Copier la sélection ».
41. **Après toute édition programmatique du JS d'un artifact : `node --check`** avant de publier.
42. **Une banque par produit** : chaque banque a un onglet par produit dès qu'une boutique en a plusieurs.
43. **Statique validée → rangée d'office** dans `Créatives <Boutique>/1-STATIQUES/<Produit>/S<n° du concept>/` (3 formats, copie, scène vierge, `_passes/`), puis ajoutée à la **banque Historique** (carré, onglet de son produit), republiée à la même adresse. La banque de concepts fait autorité : une créa hors banque n'a pas sa place dans 1-STATIQUES.
44. **Tout visuel natif validé entre dans la banque des visuels natifs**, sans qu'il le demande : formats livrés + **scène au support VIDE** + script de montage + police + fiche. Un visuel validé laissé dans le scratchpad est perdu.
45. **Native validée = rangée d'office** : un « ok » suffit → dossier créatives + banque des natives + brain, dans le même tour.
46. **Vidéo montée → rangée d'office** dans `4-VIDEOS/<FAMILLE>/<Produit>/<Nom>/` et ajoutée à l'historique des films de la banque vidéo (onglet de son produit). Le dossier garde la version Claude, ses versions, et un sous-dossier « Éléments Claude » pour tout le reste ; le dossier créatives ne garde que les livrables validés, le travail reste dans le scratchpad.
47. **Toute famille vidéo ouverte s'ajoute à la banque vidéo**, à la même adresse.
48. **Nommer les fichiers par ce qui les distingue** quand je livre plusieurs versions.
49. **Banque d'angles systématique** : dès qu'on me demande une idée, un angle, un scénario → j'ouvre la banque d'angles de la boutique, jamais de tête. Une créa complète = **1 angle × 1 concept**.

## 4. Copy et conformité

50. **Statique ≠ native** : statique = image d'abord, copie ensuite ; native = copie d'abord, visuel ensuite. Une règle de l'une ne s'applique jamais à l'autre.
51. **Livrable statique : 1 texte principal + 3 titres + 3 descriptions**, sans sous-titres. Pas de registre imposé : je le propose, l'utilisateur tranche.
52. **La copie se livre seule** : un message qui ne contient QUE la copie, prête à coller dans Meta ; mes remarques dans un message séparé. Les adcopies se livrent dans le chat, jamais en fichier `.txt`. Une adaptation validée et rangée → je livre sa copie d'office, en dernier message.
53. **Native = ultra subtile sur le produit** : nommé tard, de façon incidente ; aucun pitch d'offre ni de mécanisme dans le corps ; la page vend, pas le post.
54. **Jamais d'astérisque ni de petite ligne de renvoi** ; pas de bénéfice flou isolé.
55. **Accroches : jamais deux fois la même**, et pas d'accroche saisonnière hors saison.
56. **La longueur suit le funnel** : BOF = court et condensé ; TOF/MOF = long et développé. Je qualifie chaque format long.
57. **Je tranche et je propose UN titre**, jamais un menu A/B/C. À un palier de décision, je classe les options et je recommande celle que la donnée soutient (VOC, concurrents), preuves à l'appui.
58. **Un prix barré doit correspondre à la valeur réelle de ce qui est montré** (ex. la valeur du lot entier, lot visible à l'image) — sinon prix de référence trompeur (art. L.121-2, directive Omnibus).
59. **Preuve sociale : uniquement réelle et vérifiable.** Pas de logo/mot d'une plateforme d'avis (Trustpilot…) si la note ne vient pas de son vrai profil. Aucun faux avis, aucun faux témoignage nommé.
60. **Jamais le vrai document d'une personne ou entreprise réelle** (devis, facture, avis, ordonnance) dans une créa, même flouté : on fabrique un document 100 % fictif.
61. **Questions santé d'un client** : jamais de conseil médical ni de « aucun risque » ; renvoyer vers son médecin ou pharmacien, rappeler la garantie.
62. **Remboursement = retour de la commande demandé**, sauf si l'utilisateur dit de l'offrir.

## 5. Native — constats de marché (source : 60 natives gagnantes analysées)

63. **Le levier n°1 des natives qui scalent : le narrateur qui trahit son propre camp** (l'expert qui dénonce les pratiques de son industrie). L'autorité seule ne vend pas.
64. **La zone morte 800-1 200 signes** : les winners sont soit très courts (~600 signes), soit très longs.
65. **Les formats gagnants se transposent d'un marché à l'autre** (ex. le classement « top 3 » noté).
66. **Un dossier de swipe s'aspire** : navigateur, scroll, extraction JS des cartes (auteur, spend, jours, copie intégrale), `curl` des visuels, planche contact numérotée.
67. **Le persona d'advertorial (l'experte) est réservé aux natives et aux pages** ; il n'est jamais un avatar de créative vidéo ou statique.

## 6. Vidéo

68. **Les skills du formateur font foi** (claymotion, Disney classic, podcast, interview, papercut…) : je les invoque et je les suis palier par palier.
69. **Construction d'un scénario (skills narrés)** : ① le problème → ② pourquoi les solutions actuelles échouent → ③ comment on corrige, SANS le produit → ④ le produit → ⑤ les bénéfices → ⑥ la fin (rappel du 1er cadre + signature). Séquences présentées regroupées sous ces titres. ⛔ Pas pour le podcast et les formats exclus par l'utilisateur.
70. **Toute nouvelle vidéo démarre par un essai** (personnage + produit + décor), sans demander.
71. **Storyboard complet d'un coup, validation globale, puis animation clip par clip.** Je n'assemble jamais avant validation des clips, livrés séparés et numérotés.
72. **Un concept vidéo n'est jamais une trame figée** : je propose un scénario neuf et on le modèle ensemble ; jamais repartir d'une vidéo déjà faite.
73. **⛔ Jamais de sous-titres** sur une vidéo, même si une méthode les exige.
74. **Clips sans son** ; montage livré **avec la voix off seule** — musique et bruitages, c'est l'utilisateur (sauf demande).
75. **Le moteur validé ne change pas sans son accord**, même s'il bloque. Le modèle/mode imposé par une skill prime sur mes défauts.
76. **Un avatar peut vivre dans plusieurs familles** : la matière et l'ancre changent, jamais l'identité (il se décline, il ne se duplique pas sous un autre nom).
77. **Ne jamais faire porter à un personnage un effet qu'il ne peut physiquement pas porter.**
78. **Kling :** une seule image de départ (start + end = morphing) ; remplir la durée d'actions enchaînées, rythme vif, sinon il ralentit ou fait rebrousser chemin ; les petits visages perdent leurs traits en milieu de clip → couper sur la fin ; une cadence se force au rendu (ffmpeg), pas au générateur.
79. **Claymation :** on n'ouvre jamais un visage en pâte (lueur, transparence ou reflet à la place).
80. **Calage voix off : Palmier (`inspect_media`, wordTimestamps)**, jamais Whisper. Je crée ou j'ouvre moi-même le projet Palmier.

## 7. Outils
81. **Images : KIE** (`gpt-image-2-5-sunburst-image-to-image` par défaut) — ⬜ À COMBLER : l'installation de l'outil arrive avec le module créa. Clé jamais affichée. **Vidéo : KIE Kling 3.0 std** par défaut (`--video`). **Voix, musique, bruitages : ElevenLabs.** **Décomposer une pub vidéo : outil d'analyse vidéo**, jamais de tête.

- **Copie statique ≠ native (l'utilisateur, 06/10/2026) :** la copie d'une statique est écrite dans la voix de la marque, jamais en monologue à la 1re personne. Seule exception : citer entre guillemets une phrase que la cliente a tendance à dire.

- **Statique validée = nouvelle vignette du concept (l'utilisateur, 06/10/2026) :** quand une statique tirée d'un concept de la banque est validée, son carré remplace la vignette de ce concept dans la banque (ancienne vignette archivée), et la banque est republiée à la même adresse.
