# homeshare-visning

Offentlige, statiske visningssider for HomeShare AS. Ingen bygging, ingen avhengigheter, ingen tester.

## Hva som ligger her
- `index.html`: tom forside («HomeShare AS»).
- `fyresdal/index.html`: visningssiden for Fyresdal, én selvstendig HTML-fil (ca. 2,3 MB) med kart, galleri og boligliste. Commit-historikken viser at den oppdateres ved å erstatte hele filen («Update fyresdal map to latest client version»).
- `.nojekyll`: GitHub Pages serverer filene som de er.

## Publisering
GitHub Pages fra `main`: https://home-share-as.github.io/homeshare-visning/fyresdal (adressen brukes i Home-Share-AS/homeshare-ops, AGENTS.md). En push til `main` er altså en publisering. Alt går via branch og PR, og ingenting merges uten Olafs ja.

## Forhold til andre repoer
- Tilbudssiden i salgstavla (`/tilbud/` i Home-Share-AS/homeshare-ops, `flows/flyt-01/tilbud.py` og `sider/tilbud.*`) er bygd ordrett etter Fyresdal-siden. Nye tilbud lages der, ikke her.
- Nettsiden www.homeshare.no er Home-Share-AS/homeshare-website.
- Bakgrunn om HomeShare og botene: Home-Share-AS/homeshare-context (`business.md`, `grokbot/felles/README.md`). Claude Code-agentens playbooks: `grokbot/claude-code/` der.

## Regler
- Norsk bokmål, ingen tankestreker, datoer DD.MM.YYYY, beløp i NOK.
- Ingen kundedata, kontonummer, koder eller hemmeligheter i filene. Siden er offentlig.
- Bildene i `fyresdal/index.html` lastes fra en ekstern bildetjeneste (a0.muscache.com). Ny side: bruk bilder HomeShare har rett til, og helst lagret i repoet.
