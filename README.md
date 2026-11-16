# Gestion boutique — brains

| Dossier | Contenu |
|---|---|
| `brain-solevita/` | Brain de **Solevita** (le coussin) |
| `brain-noxe/` | Brain de **Noxe** (le beurre corporel) |
| `methode/` | Méthode commune à toutes les boutiques (le COMMENT) |
| `agents/` | L'équipe des 9 agents, commune à toutes les boutiques |

## Installation sur ton ordinateur
Les brains cherchent la méthode dans `~/methode/` et les agents dans `~/.claude/agents/`.
Après avoir récupéré ce dépôt, une seule fois (sans écraser ce qui existe déjà) :

```bash
cp -rn methode ~/methode
mkdir -p ~/.claude/agents && cp -n agents/*.md ~/.claude/agents/
```

Ensuite, ouvre toujours Claude Code **dans le dossier du brain** de la marque sur laquelle tu travailles.
