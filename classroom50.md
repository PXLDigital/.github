# Classroom 50

Opdrachten uitdelen, opvolgen en feedback geven via GitHub. Vervangt GitHub Classroom. Webapp: [classroom50.org](https://classroom50.org) (inloggen met GitHub, organisatie `PXLDigital`).

## Lector: opdracht opzetten

1. **Create classroom**: naam, slug en term. Eén classroom per vak per semester.
2. **Staff** toevoegen onder *Settings → Staff and roles* (teacher, hta, ta).
3. **Roster** uploaden (CSV met `username`, `email` of `github_id`) of studenten één voor één toevoegen. Studenten moeten eerst de uitnodiging voor `PXLDigital` accepteren.
4. **+ Assignment**: individueel of team, template-repo, deadline.
5. Deel de **acceptatielink** met de studenten.

Meer: [Teacher Guide](https://github.com/foundation50/classroom50/wiki/Web-Teacher-Guide).

## Onze instellingen (najaar 2026)

| Classroom | Opdracht | Teams | Template |
|---|---|---|---|
| Professional Innovation | `3eai-pi-2627` | max. 2, studenten kiezen zelf | `template-vanrykel` |
| Industrial Automation | `3eai-ai-2627` | max. 4, lector verdeelt | `template-vanrykel` |

Overal: autograder en score uit, Feedback-PR aan, wiki en projects uit.

## Feedback-PR

Elke studentenrepo krijgt één PR (`feedback` ← default branch) waarin je per regel commentaar geeft. Hij wordt bij elke push vanzelf bijgewerkt. **Mergen = beoordeling klaar**, en dat kunnen enkel lectoren en TA's. Studenten sluiten of mergen hem niet.

## Beheer

- **Scores:** in `PXLDigital/classroom50` → Actions → *Collect Scores* → *Run workflow*. Dit schrijft `scores.json`; pas dat nooit met de hand aan.
- **Service token** (`CLASSROOM50_SERVICE_TOKEN`) verlopen, of 401/403 bij een run? Draai *Probe Service Token* en vernieuw met `gh teacher rotate-service-token PXLDigital`.
- Instellingen van een opdracht wijzig je bij voorkeur in de webapp of met `gh teacher`, niet door de JSON te bewerken.
- GitHub Actions kost minuten: [Managing Actions Cost](https://github.com/foundation50/classroom50/wiki/Managing-Actions-Cost).

## Studenten

- Voeg naast je persoonlijke adres je **PXL-studentenmailadres** (met studentnummer) toe aan je GitHub-account. Zo worden commits en opdrachten aan de juiste student gekoppeld.
- Accepteer de uitnodiging voor `PXLDigital` vóór je de opdracht accepteert.

## Rulesets

`classroom50-protect-submission-history` en `classroom50-feedback-base-lock` horen bij Classroom 50. Zie [beleid.md](beleid.md#rulesets).
