---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Aktivera eller inaktivera snabbversioner för din organisation
description: Du kan välja om du vill få nya Workfront-funktioner månadsvis eller kvartalsvis.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 71ef7a50-7a9f-43c4-b67c-8d9fc722569f
source-git-commit: 7ca27795ec115a112acb55113bfade4a5fee15ad
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Aktivera eller inaktivera snabba releaser för din organisation

Adobe Workfront har två modeller för att lansera nya funktioner och uppdateringar. Du kan välja om du vill få tillgång till nya funktioner kvartalsvis eller enligt ett snabbare schema.

Båda modellerna har samma funktioner och uppdateringar. Den enda skillnaden är i timingen.

Exempel:

* Företag X har aktiverat processen för snabb lansering. De får A i augusti, B i september och C i oktober.
* Företag Y har inaktiverat processen för snabb lansering. De får funktionerna A, B och C i kvartalsversionen i oktober.

>[!NOTE]
>
>* Kunder som har köpt Workfront efter version 23.3 (juli 2023) har snabbversionsprocessen aktiverad som standard och kan avanmäla sig.
>* Kunder som har köpt Workfront före version 23.3 har den snabba versionsprocessen inaktiverad som standard och kan välja att delta.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara Workfront-administratör. </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du aktiverar eller inaktiverar processen för snabb släppning

Tänk på följande när du aktiverar eller inaktiverar snabbversionsprocessen:

* **Om du aktiverar** den snabba versionsprocessen mitt i ett kvartal får din organisation tillgång till funktioner som redan har släppts i den snabba versionen.

  Om till exempel funktion A släpps i augusti och funktion B släpps i september får alla företag som aktiverar den snabba releaseversionen i september omedelbart tillgång till funktionerna A och B.

* **Om du inaktiverar** börjar den snabba versionsprocessen inte gälla förrän nästa kvartalsrelease.

  Om till exempel en organisation som har aktiverat en snabb release inaktiverar den i augusti får de fortfarande de snabba releasefunktionerna i september, eftersom de inte kommer att gå över till den kvartalsvisa versionen förrän nästa kvartalsrelease inträffar i oktober.

## Aktivera eller inaktivera snabbversionsprocessen för din organisation

Så här aktiverar eller inaktiverar du snabbversionsprocessen:

{{step-1-to-setup}}

1. Expandera **System** i den vänstra navigeringen och klicka sedan på **Inställningar**.
1. Markera kryssrutan **Tillåt snabbsläppsprocess** om du vill aktivera snabba releaser.

   eller

   Om du vill inaktivera snabba releaser och gå till en kvartalsvis versionscykel avmarkerar du kryssrutan **Tillåt snabbversionsprocess**.

1. Bekräfta ditt val i popup-fönstret.
1. Klicka på **Spara**.
