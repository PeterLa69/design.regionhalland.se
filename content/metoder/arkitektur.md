---
date: 2017-04-01T12:21:15Z
title: "Arkitektur"
description: Hur vi arbetar med arkitektur inom Region Halland
weight: 1000
---
## Principer
Våra grundläggande arkitekturprinciper

### Hög Sammanhållning (Cohesion) och Låg Koppling (Coupling)
Inom mjukvarudesign pratar man ofta om begreppen Cohesion (sammanhållning) och Coupling (koppling). Där sammanhållning är ett mått på graden av komponentens delar som funktionellt relaterade. Det kan sägas vara i vilken grad alla element som är inriktade på att utföra en enskild uppgift finns i komponenten. Koppling är sin tur måttet på graden av ömsesidigt beroende mellan olika komponenter. Inom programvaruutveckling vill man uppnå en hög sammanhållning och en låg koppling. 

Detta beskriver också mycket väl hur vi ser på hela vårt digitala landskap. För de olika komponenterna vi har i form av system, appar, applikationer, etc. vill vi ha en hög så hör sammanhållning som möjligt och en så låg koppling som möjligt.

För att länka samman olika komponenter vill vi att detta sker genom datakoppling. Detta innebär att komponenterna kommunicerar med varandra genom att endast överföra data mellan varandra. Genom att endast överföra data mellan varandra uppnår vi en låg koppling mellan komponenterna.

Genom att försöka hålla samman all hantering kring en viss informationsmängd i en enskild komponent säkerställer vi att vi uppnår så hög sammanhållning som möjligt. Exempel på detta kan vara att ekonomidata hanteras i ett ekonomisystem, journaldata i ett journalsystem, osv. Motsatsen inträffar när en viss informationsmängd hanteras i ett flertal olika system. 


### API-first
Region Hallands grundfilosofi är API-first, vilket innebär att vi alltid tänker oss att bygga lösningar baserade på API-er snarare än klassiska client-server-lösningar. Vi förespråkar pragmatisk API design, vilket innebär att vi utgår ifrån vad det är vi försöker uppnå med vårt API och se det ur en utvecklares perspektiv och att denne ska bli så framgångsrik som möjligt i användandet av API-et. Enkelhet är den viktigaste principen i skapande av API-er. 
