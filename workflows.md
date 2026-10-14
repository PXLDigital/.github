# Validatie-workflows

Drie workflows controleren pull requests in repo's (voorlopig nog enkel in `*-PEN-*` en `*-POZ-*`). 

Ze staan in `.github/workflows/` van deze repo en worden afgedwongen via de ruleset *Master branch protection (PEN & POZ)*.

| Workflow | Controleert |
|---|---|
| `validate-documentation.yml` | Er is minstens één `.md`. Elk toegevoegd pdf/stl/png/jpg/gif/svg/webp wordt in een `.md` vermeld. |
| `validate-links.yml` | Interne links zijn niet kapot. Geen absolute links naar de eigen repo (`blob`, `tree`, `raw`), geen lokale paden (`C:\`, `file://`), geen externe links naar mediabestanden. |
| `validate-file-formats.yml` | Geen bestanden die je niet in GitHub kan reviewen: Word, Excel, PowerPoint, zip, CAD (step, dwg, …). PDF, STL, afbeeldingen en tekst mogen. |

- Ze draaien op pull requests en controleren enkel gewijzigde bestanden (behalve de bestaande documentatie en interne links).
- Paden vanaf de repo-root, zoals `/docs/foto.png`, zijn toegelaten.
- Externe links (`https://…`) worden niet op bereikbaarheid gecontroleerd, enkel op media.

## Wijzigen

Via pull request. Zodra die op `master` staat, geldt de wijziging **meteen** voor alle PEN/POZ-repo's. Test dus eerst in een testrepo.
