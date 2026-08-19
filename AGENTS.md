# AGENTS.md

## What this repo is
- Requirements-only repo: the single source of truth is `Anforderung.md` (a German spec for a survey / "Umfragen" app). There is no code, build tooling, or git history yet.
- `Anforderung.md` is the product contract. When implementing in the future, treat it as the authoritative feature list.

## Working in this repo
- Domain context is German; keep any new requirements/spec text in German to match.
- `Anforderung.md` lists ~10 features and 3 roles (Host, Teilnehmer, Abteilungen). Notable hard design constraint: **max 3 colors** in the UI.
- No commands to run (no manifests, lockfiles, tests, or CI). If a build step is requested, it must be introduced from scratch.
