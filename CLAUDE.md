**🔬 Regel: Forschung nur in Kimhub (Klaus 2026-10-31: „einheitlich alles in Kimhub … in den einzelnen Repos soll keine Forschungseinträge sein“):** jeder Forschungseintrag (Sitzungs-Befunde, Messungen, Stunden-Auswertungen, Forschungsnotizen) kommt nach **Kimhub `forschung/messungen/`**; in diesem Repo werden keine Forschungseinträge geführt und keine Forschungsdateien angelegt. Öffentliche Forschungs**aufgaben** stehen in Sage-Protokol.

# Mein-Mixarium · Landingpage — Sitzungs-Anker

Landing-Seite für **Mein Mixarium** (eigenes Repo). Hier liegt **nicht** die App —
wer am Mixarium baut, ist im falschen Repo.

## Prüfen

```bash
node tests/smoke_mikrofon_sprachen.mjs
```

Keine `package.json`; braucht `playwright-core`. Fehlt es, ist die Probe **nicht
lauffähig, nicht rot**.

## Was hier leicht kaputtgeht

- `vendor/` ist mitgeliefert, damit die Seite **ohne CDN** läuft.
- Ladezeit-Regeln (Bilder, Skripte, Layout, Messen): Skill `seiten-bauregeln`.

## Netzweit

Freibrief zum Selbst-Mergen · Gerätename · frisch von `origin/main` vor jeder Arbeit ·
Ton · kein PII · Ehrlichkeit stehen **einmal** in
**[`Sage-Protokol/docs/NETZWEIT.md`](https://github.com/lausiklauskn-png/Sage-Protokol/blob/main/docs/NETZWEIT.md)**.

```bash
git fetch origin --quiet && git checkout -B <branch> origin/main
git push -u origin refs/heads/<branch>:refs/heads/<branch>
git diff --stat origin/main origin/<branch>     # leer = der PR wäre leer
```
