---
user-type: administrator
product-area: system-administration;setup
title: Konfigurera anpassad lokalisering
description: Med anpassad lokalisering kan du definiera anpassade termer och fraser på olika språk. Workfront visar sedan dessa termer på det språk som angetts i webbläsarinställningarna.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: bdc6d5ee-2037-4d0b-bf18-3e6cc9cb078e
source-git-commit: aeb471fd63269d30a675e44fe1a47db6141eb9ed
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 1%

---

# Konfigurera anpassad lokalisering

Med anpassad lokalisering kan du definiera anpassade termer och fraser på olika språk. Workfront visar sedan dessa termer på det språk som anges i användarens IMS-inställningar (Adobe Identity Management).

Du kan till exempel ställa in etiketten &quot;Målpublik&quot; till att översätta till det tyska ordet &quot;Zielgruppe&quot;. Alla användare med tyska som har valts som webbläsarens huvudspråk ser ordet&quot;Zielgruppe&quot; som etikett för alla fält med namnet&quot;Target Audience&quot; på engelska.

Du kan konfigurera översättningar till flera språk. Tillgängliga språk är:

* Kinesiska (traditionell)
* Kinesiska (förenklad)
* Franska
* Tyska
* Italienska
* Japanska
* Koreanska
* Portugisiska (Brasilien)
* Spanska

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Arbetsflöde Prime eller senare </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör för att konfigurera översättningar.</p>  </td> 
  </tr>
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när lokalisering ställs in

Tänk på följande när du konfigurerar lokalisering:

* Du kan konfigurera en term som ska översättas till flera språk.
* Lokalisering gäller för anpassade fältetiketter (inklusive när de används som kolumnrubrik) och verktygstips.
* Anpassad lokalisering kan gälla för meddelanden som genereras från affärsregler, men måste aktiveras i affärsregeln.

  Instruktioner finns i [Aktivera lokalisering i en affärsregel](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md#using-custom-localization-with-business-rules) i artikeln Skapa och redigera affärsregler.

## Konfigurera översättningar

Översättningar konfigureras under Konfigurera.

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **[!UICONTROL Setup]** ![ikonen Konfigurera](/help/_includes/assets/gear-icon-setup.png).
1. Klicka på **Lokalisering** i den vänstra navigeringspanelen under Konfigurera.
1. Om du vill lägga till en ny översättning klickar du på **Ny rad**.
1. I kolumnen **Engelska** anger du den engelska termen som ska översättas.
1. I kolumnen för det språk som du vill att termen ska översättas anger du termen på målspråket.
1. Om du vill översätta ordet till ytterligare språk lägger du till översättningen i rätt språkkolumn.
1. Om du vill ändra ordningen på språkkolumner klickar du på rubriken för den kolumn du vill flytta och drar den till önskad plats.
