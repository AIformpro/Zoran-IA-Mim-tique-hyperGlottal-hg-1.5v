# HyperGlottal©® (HG©®) — v1.5 (“1.5V”)
_Méta‑langage programmable au‑delà de QuantaGlottal©® : types dépendants, linéarité, effets, budgets prouvables, ZK natif, sessions typées, interop multi‑cible._

## TL;DR
- **Modèle** : λ‑calcul dépendant + types linéaires + effets à lignes + contrats + sessions typées
- **Sécurité** : capacités, labels MAC, sandbox éphémère **Z🦋NESTLOCK©®**
- **ZK natif** : compilation des fragments purs → circuits ZK + receipts d’exécution
- **Tooling** : `hg` (CLI stdlib‑only) : `new`, `run`, `prove`, `zk`, `pack`, `version`

## Installation (développement)
```bash
python -m venv .venv && source .venv/bin/activate
pip install -e .
hg version
```

## Essai rapide
```bash
hg new examples/hello.hg
hg run examples/hello.hg       # interprétation déterministe (subset M0)
hg prove examples/hello.hg     # obligations de preuve (mock SMT)
hg zk examples/hello.hg        # receipt ZK (mock)
hg pack                        # crée dist/hg-artifact.hgz + SHA256
```

## Structure
```
.
├── README.md
├── pyproject.toml
├── src/hyperglottal/...
├── schemas/module-0.1.json
├── grammar/hg.ebnf
├── examples/hello.hg
├── docs/spec.md
├── tests/test_basic.py
└── .github/workflows/ci.yml
```

## Mentions
Frédéric Tabary — Institut ia — 0645605023 — Canada, Montréal, France — INSTITUT🦋 IA INC., 7100-380, rue Saint-Antoine Ouest, Montréal (Québec) H2Y 3X7.
