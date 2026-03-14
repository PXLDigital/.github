# Welkom

Maak gerust repo's en teams aan maar geef een **duidelijke naamgeving** mee en een **contributing page**. Zie eventueel bij bestaande Templates.

## Policy naamgeving

De meest voorkomende **repositories waarin studenten zullen werken** zijn gebonden aan een trajectschijf of een projectvak.

- Daarom krijgen alle repo's die zich beperken tot een trajectschijf de **prefix [studiejaar]** mee, gevolgd door de cursusnaam.
- Alle projecten die zich niet (gaan) beperken tot één bepaalde trajectschijf krijgen de **prefix Project_** mee. Denk hierbij aan projecten die het jaar erop verder gezet worden.

**Repositories met een ondersteunende functie** en studenten dus niet actief in werken bijvoorbeeld workshops, proeflapen of als example code krijgen een prefix mee die betrekking heeft tot de technologie.

### Technische naamgevingsregel (afdwingbaar)

Alle repository-namen moeten voldoen aan het patroon **`^[a-z0-9]+(-[a-z0-9]+)+$`**.

**Concreet betekent dit:**

- Enkel **kleine letters** `a–z`, **cijfers** `0–9` en **koppeltekens** `-` zijn toegestaan
- De naam bestaat uit **minstens twee blokken**, gescheiden door `-` (bijvoorbeeld: `2eai-ems-2324-course`)
- **Geen** spaties, **geen** underscores `_`, **geen** hoofdletters

### Voorbeelden geldige repository-namen

| Betekenis | Geldige repo-naam |
|:---|:---|
| studiejaar \| cursusnaam (met academiejaar) | 2eai-ems-2324-course \| 2eai-ems-2223-task1 \| 3eai-ia-2122-carproduction \| 3eai-ia-2122-task1-alexpeters |
| Project \| technologie of domein | project-plc-agv \| project-rpi-smarthome \| project-research-groendraken |
| technologie \| doel | tc-demo-dmx \| rpi-workshop-iot \| mtb-psoc6-pdl-adventures \| mtb-psoc4-hal-adventures \| mtb-example-psoc6-dfu-basic |
