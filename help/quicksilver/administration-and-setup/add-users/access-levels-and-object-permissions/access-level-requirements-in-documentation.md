---
title: Krav på åtkomstnivåer
content-type: reference
product-area: system-administration
keywords: behörighet,nivå,system,administratör,planerare,arbetare,granskare,begärande,extern,användare
navigation-topic: access-levels
description: I Workfront-dokumentationen finns en tabell med information om vilka behörigheter som krävs för proceduren. I den här artikeln förklaras tabellen över åtkomstkrav mer ingående och den innehåller länkar för mer information.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
source-git-commit: d786a5bd86bcc1a4fbacf022cc9fbee9cb321da5
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# Krav för åtkomstnivåer i Workfront-dokumentationen

I Workfront-dokumentationen finns en tabell med information om vilka behörigheter som krävs för den proceduren. I den här tabellen för åtkomstkrav kan du förstå om du kan utföra en viss åtgärd i Workfront eller varför du inte kan göra det. I den här artikeln förklaras varje element i tabellen för åtkomstkrav och den innehåller felsökningstips och länkar till mer detaljerad information.

Om det inte finns någon rad i tabellen för åtkomstkrav i en viss artikel finns det inga krav av den typen för den åtgärden.

>[!NOTE]
>
>Kontakta Workfront-administratören om du har frågor om hur något av fälten i den här tabellen gäller dig.

## Åtkomstkravregistret

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> Adobe Workfront planer avser den uppsättning funktioner som din organisation har köpt. De flesta Workfront-funktionerna finns i alla planer, med några få undantag, huvudsakligen för strategisk planering och företagskontroller. 
   <ul><li>Kontakta Workfront-administratören om du vill veta vilken Adobe Workfront-plan din organisation använder, inklusive om din organisation är under den nya eller nuvarande paketeringsmodellen.</li>
   <li>Instruktioner om hur en Workfront-administratör kan hitta din organisations Workfront-plan finns i <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan" class="MCXref xref">Visa din organisations kluster och Workfront-plan</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> Adobe Workfront licenser avser den uppsättning Workfront-funktioner som ingår i licensen som tilldelats dig. En användare kan t.ex. ha en licens som markerar arbetsposter som slutförda och som loggar, medan en annan användare har en licens som endast tillåter dem att godkänna resurser eller skicka begäranden. <p> 
   <ul>
   <li>Kontakta Workfront-administratören om du vill veta vilken licens du har tilldelats.</li>
   <li>Adobe Workfront går över till en ny prissättnings- och paketeringsmodell. Mer information om licenser finns i:
   <ul>
   <li>Nytt: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Översikt över nya licenser</a></li>
   <li>Aktuell: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över licenser</a></li></ul></li>
   <li>Om du har rätt åtkomstnivå och fortfarande inte har åtkomst, frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå</td> 
   <td> Åtkomstnivåer är behörighetsgrupper för åtgärder som du kan utföra i Workfront, som anges av Workfront-administratören. <p>Workfront har inbyggda åtkomstnivåer som motsvarar Workfront-licenser, men din Workfront-administratör kan skapa fler åtkomstnivåer för att bättre återspegla de behörighetsgrupper som behövs i organisationen.</p>
   <ul>
    <li>Adobe Workfront går över till en ny prissättnings- och paketeringsmodell. Mer information om åtkomstnivåer för varje modell finns i:
   <ul>
   <li>Nytt: <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">Översikt över nya åtkomstnivåer</a></li>
   <li>Aktuell: <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Översikt över åtkomstnivåer</a></li></ul></li>
    <li>Kontakta din Workfront-administratör om du vill veta mer om din åtkomstnivå</li>
    <li>Om du är Workfront-administratör kan du läsa <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Konfigurera åtkomst till Adobe Workfront</a> om du vill veta mer om hur du ger åtkomst till specifika objekt på åtkomstnivån.</li>  
   <li>Om du har rätt åtkomstnivå och fortfarande inte har åtkomst, frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td><p>Objektbehörigheter avser den åtkomst du har till enskilda Workfront-objekt när du skapar dem eller när de delas med dig. Du måste till exempel ha behörigheten Visa för ett visst projekt för att kunna visa projektet, även om åtkomstnivån tillåter dig att visa projekt. I det här avsnittet av tabellen för åtkomstkrav beskrivs eventuella objektbehörigheter som du behöver för att utföra åtgärden i artikeln.</p>
   <p>Mer information om hur du begär ytterligare åtkomst till ett objekt finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Workfront erbjuder vissa produkter som kan köpas utöver Workfront.
   <p>Artiklar som beskriver de procedurer som utförs i dessa ytterligare produkter listar den produkt som krävs här.</p>
   <ul>
   <li>Adobe Experience Manager Assets eller Assets Essentials </li>
   <li>Workfront Fusion</li>
   <li>Workfront-mål</li>
   <li>Workfront Scenario Planner</li>
   </ul>
   <p>Kontakta Workfront-administratören om du vill veta om din organisation har köpt någon av dessa produkter.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion-licens</td> 
   <td>Adobe Workfront Fusion har en separat licensieringsmodell än Workfront. 
   <ul><li>Aktuell: Den aktuella licensmodellen baseras på antalet utförda åtgärder och har inga begränsningar för vilka åtgärder en organisation kan utföra. </li>
   <li>Äldre: Äldre licenser baseras på om det går att ansluta till program från tredje part eller om scenarierna bara används för Workfront-automatisering. </li>
   </ul>
   Mer information om Fusion-licensiering finns i <a href="/help/quicksilver/workfront-fusion/get-started/license-automation-vs-integration.md" class="MCXref xref">Workfront Fusion-licenser</a>.
   </td> 
  </tr> 
 </tbody> 
</table>


