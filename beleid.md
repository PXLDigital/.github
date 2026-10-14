# GitHub-beleid PXLDigital

Korte versie. Meer: [workflows](workflows.md) · [Classroom 50](classroom50.md) · [naamgeving](profile/README.md)

## Basis

- **2FA is verplicht** voor alle leden.
- **Repo-namen** volgen `^[a-zA-Z0-9]+(-[a-zA-Z0-9]+)+$` (organisatie-policy). Afspraken over prefixen staan in [profile/README.md](profile/README.md).

## Rulesets

| Ruleset | Geldt voor | Regels |
|---|---|---|
| `classroom50-protect-submission-history` | alle repo's, default branch | lineaire historiek (geen merge commits) · geen force push · niet verwijderbaar |
| `Master branch protection (PEN & POZ)` | repo's `*-PEN-*` en `*-POZ-*`, default branch | PR verplicht: 1 goedkeuring · goedkeuring vervalt bij nieuwe commit · laatste push door een ander goedgekeurd · gesprekken opgelost · de 3 [validatie-workflows](workflows.md) moeten slagen |
| `classroom50-feedback-base-lock` | alle repo's, branch `feedback` | niet wijzigbaar, niet verwijderbaar |

- **Waarom enkel PEN & POZ?** Een PR door meerdere personen laten goedkeuren kan enkel in projectvakken waar studenten in groep werken. De org-brede ruleset bevat alleen wat voor alle lectoren geldt: de historiek beschermen.
- **Mergen:** lineaire historiek verbiedt merge commits, gebruik dus *squash* of *rebase*.
- **Copilot:** in PEN & POZ vragen wijzigingen zonder auteur (Copilot) extra goedkeuring.
- **Bypass:** alleen org-admins. Op `feedback` ook de Classroom 50-staffteams.

## Template

`template-vanrykel` is vrij te gebruiken (initiatief van één lector, mogelijk opleidingsbreed). Studenten:

- linken **relatief**, geen externe of absolute links;
- vermelden elk pdf/stl/beeld in een `.md`;
- gebruiken enkel **reviewbare** bestanden: geen Word, Excel, PowerPoint, zip of CAD (PDF en STL mogen).

Waarom: een PR moet altijd in GitHub te reviewen zijn, en info mag niet verdwijnen met een externe link.

## Classroom 50

Zie [classroom50.md](classroom50.md). Studenten voegen hun PXL-studentenmailadres toe aan hun GitHub-account.

## Wijzigen

Via pull request op deze repo of mail naar [dieter.vanrykel@pxl.be](mailto:dieter.vanrykel@pxl.be). Rulesets: *Organization → Settings → Repository → Rulesets*.
