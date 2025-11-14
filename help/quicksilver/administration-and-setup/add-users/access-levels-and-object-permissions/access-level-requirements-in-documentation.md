---
title: Åtkomstkrav i Workfront-dokumentationen
content-type: reference
product-area: system-administration
keywords: behörighet,nivå,system,administratör,planerare,arbetare,granskare,begärande,extern,användare
navigation-topic: access-levels
description: I Workfront-dokumentationen finns en tabell med information om vilka behörigheter som krävs för proceduren. I den här artikeln förklaras tabellen över åtkomstkrav mer ingående och den innehåller länkar för mer information.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 39ea0d53-ec31-4644-b772-cfe260b8e013
source-git-commit: c1c30696dc9ef324103467f3bdcb83609cf5d1d8
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# Åtkomstkrav i Workfront-dokumentation

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
   <td role="rowheader">Adobe Workfront package</td> 
   <td> Adobe Workfront-paket avser den uppsättning funktioner som din organisation har köpt. De flesta Workfront-funktionerna finns i alla paket, med några få undantag, som mest gäller strategisk planering och företagskontroller. <p>Paket som fanns före 2022 listas inte.</p>
   <p>Workfront-paketen är uppdelade i tre områden. I vissa områden finns olika paket som Select, Prime och Ultimate.<p>
   <ul>
   <li><b>Workfront-arbetsflöde</b>: Innehåller funktioner som är relaterade till åtgärder, som uppgiftshantering, godkännanden och tidrapporter. Det här paketet är ytterligare uppdelat i Ultimate-paket för arbetsflödesval, arbetsflöden och arbetsflöden.</li>
   <li><b>Workfront Planning</b>: Innehåller funktioner som är relaterade till strategisk planering. Paketet delas upp i Planning Select-, Planning Prime- och Planning Ultimate-paket.</li>
   <li><b>Workfront Automation and Integration</b>: Innehåller funktioner som rör automatisering av processer och integrering med andra program.</li>
   </ul>
  <p>Din organisation kan ha köpt ett Workfront-paket inom ett eller flera av dessa områden.</p>
  <p>Tidigare erbjöd Workfront paket med Workfront Select, Workfront Prime och Workfront Ultimate, utan att göra skillnad mellan arbetsflöde, planering och automatisering och integrering. Din organisation kanske finns i något av dessa äldre paket. 
   <ul><li>Om du vill ta reda på vilket Adobe Workfront-paket din organisation använder, inklusive om din organisation är under den aktuella eller gamla paketeringsmodellen, kontaktar du Workfront-administratören.</li>
   <li>Instruktioner om hur en Workfront-administratör kan hitta din organisations Workfront-paket finns i <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">Visa din organisations kluster och Workfront-paket</a>.</li><li>Mer information om Workfront-paket finns i <a href="https://business.adobe.com/se/products/workfront/pricing.html">Adobe Workfront priser och paketering</a>.</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> Adobe Workfront licenser avser den uppsättning Workfront-funktioner som ingår i licensen som tilldelats dig. En användare kan t.ex. ha en licens som markerar arbetsposter som slutförda och som loggar, medan en annan användare har en licens som endast tillåter dem att godkänna resurser eller skicka begäranden. <p> 
   <ul>
   <li>Kontakta Workfront-administratören om du vill veta vilken licens du har tilldelats.</li>
   <li>Mer information om licenser finns i:
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Översikt över nya licenser</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över licenser</a></li></ul></li>
   <li>Om du har rätt åtkomstnivå och fortfarande inte har åtkomst, frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="/help/quicksilver/administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-package" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.
   </ul>
      </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td><p>Eftersom Workfront samarbetar med andra Adobe-produkter interagerar vissa procedurer i Workfront direkt med dessa produkter. För att kunna följa dessa procedurer måste din organisation ha köpt produkten. Om du till exempel vill använda funktioner som gör att Workfront kan interagera med Adobe Experience Manager Assets måste din organisation ha köpt Adobe Experience Manager Assets.</p>
   <p>Artiklar som beskriver procedurer som utförts med ytterligare produkter listar den önskade produkten på produktraden i denna tabell.</p>
   <p>Kontakta Workfront-administratören om du vill veta om din organisation har köpt någon av dessa produkter.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivå</td> 
   <td> Åtkomstnivåer är behörighetsgrupper för åtgärder som du kan utföra i Workfront, som anges av Workfront-administratören. <p>Workfront har inbyggda åtkomstnivåer som motsvarar Workfront-licenser, men Workfront-administratören kan skapa fler åtkomstnivåer för att bättre återspegla de behörighetsgrupper som behövs i organisationen.</p>
   <ul>
    <li>Mer information om åtkomstnivåer finns i:
   <ul>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md" class="MCXref xref">Översikt över nya åtkomstnivåer</a></li>
   <li><a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md" class="MCXref xref">Översikt över åtkomstnivåer</a></li></ul></li>
    <li>Kontakta Workfront-administratören om du vill veta mer om din åtkomstnivå</li>
    <li>Om du är Workfront-administratör kan du läsa <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Konfigurera åtkomst till Adobe Workfront</a> om du vill veta mer om hur du beviljar åtkomst till specifika objekt på åtkomstnivån.</li>  
   <li>Om du har rätt åtkomstnivå och fortfarande inte har åtkomst, frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</li>
    </td>
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td><p>Objektbehörigheter avser den åtkomst du har till enskilda Workfront-objekt när du skapar dem eller när de delas med dig. Du måste till exempel ha behörigheten Visa för ett visst projekt för att kunna visa projektet, även om åtkomstnivån tillåter dig att visa projekt. I det här avsnittet av tabellen för åtkomstkrav beskrivs eventuella objektbehörigheter som du behöver för att utföra åtgärden i artikeln.</p>
   <p>Mer information om hur du begär ytterligare åtkomst till ett objekt finns i <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt</a>.</p><p>Mer information om hur du delar ett objekt finns i <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md" class="MCXref xref">Dela ett objekt</a>.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Layoutmall</td> 
   <td><p>Layoutmallar styr vad du kan se på huvudmenyn och konfigureras av Workfront-administratören. På den här raden antecknas eventuella områden i Workfront som måste ingå i huvudmenyn för att åtgärden ska kunna utföras.</p><p>Om en artikel uppmanar dig att klicka på ett område på huvudmenyn, och det området inte visas på huvudmenyn, kontaktar du Workfront-administratören för att avgöra om det området kan göras tillgängligt för dig.</p><p>
   Mer information om hur en Workfront-administratör kan konfigurera huvudmenyn finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref">Anpassa huvudmenyn med hjälp av en layoutmall</a>.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion-licens</td> 
   <td>Adobe Workfront Fusion har en separat licensieringsmodell än Workfront. 
   <ul><li>Den aktuella licensmodellen baseras på antalet utförda åtgärder och har inga begränsningar för vilka åtgärder en organisation kan utföra. </li>
   <li>Äldre licenser baseras på om det går att ansluta till program från tredje part eller om scenarierna bara används för Workfront-automatisering. </li>
   </ul>
   Mer information om Fusion-licensiering finns i <a href="https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration" class="MCXref xref">Workfront Fusion-licenser</a>.
   </td> 
  </tr> 
 </tbody> 
</table>
