---
title: Granska begränsningar för samarbete med personer utanför organisationen
description: Granska begränsningar för samarbete med personer utanför organisationen
author: Courtney
draft: Probably
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Granska begränsningar för samarbete med personer utanför organisationen

Det finns vissa begränsningar som du bör vara medveten om när du kommunicerar med personer utanför organisationen när de läggs till i ett bevis, särskilt om personen utanför organisationen har språkåtkomst i en separat miljö.

## Kontakter med distinkt medlem

Det finns tre typer av kontakter i en korrekturmiljö:

* **Användare**: Användare har en Workfront Proof-inloggning i din organisations miljö.
* **Medlemmar**: Medlemmar har egna Workfront Proof-inloggningar i en annan organisations miljö (inte din egen). Du kan inte konvertera medlemmar till användare i din miljö.
* **Gäster**: Gäster har inte egna Workfront-korrekturinloggningar i din organisations miljö, men du har lagt till deras information i ditt konto (till exempel gästgranskare på korrektur). Du kan konvertera gäster till användare.

Eftersom medlemmar inte kan konverteras till användare är deras möjlighet att tagga personer i korrekturkommentarer begränsad till användare från *sin ursprungliga organisation*.

**Exempel:** Företag A bjuder in en extern användare att granska ett bevis. Den här användaren finns redan i en separat korrekturmiljö, företag B.

 

När företag A bjuder in den utomstående användaren till beviset läggs den utomstående användaren till i företagets kontaktlista som medlem. Granskare i korrekturarbetsflödet från företag A kan tagga den externa användaren i korrekturkommentarer eftersom de nu finns i kontaktkatalogen för företag A.

 

Den utomstående användaren kan inte tagga användare från företag A, även om de befinner sig i samma korrekturarbetsflöde, eftersom användarna från företag A inte har lagts till som kontakter till företag B.

 

Utomstående användare från företag B kan tagga andra användare från företag B om de är i korrekturarbetsflödet eller om de har behörighet att dela korrekturet med nya användare eftersom dessa användare finns som kontakter i företag B.
