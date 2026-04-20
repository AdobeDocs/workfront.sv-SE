---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Mappa användarattribut
description: Med enkel inloggning (SSO) kan du skicka attribut från identitetsleverantörens Active Directory till dina Adobe Workfront-användare.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: d8ccdeac9a658ca7a2862781e98c2c3c6fa0e8a0
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Mappa användarattribut

<!--Audited 2/2024-->

Med enkel inloggning (SSO) kan du skicka attribut från identitetsleverantörens Active Directory till dina Adobe Workfront-användare.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td><p>Du måste vara Workfront-administratör</p></td>
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tips för mappningsattribut

Tänk på följande när du mappar attribut:

* Testa alltid i en förhandsvisningssandlåda eller i en CR-sandlåda (Customer Refresh).
* Testa med både administratörskonton och icke-administratörskonton för att bekräfta att du mappar attribut korrekt.
* Attribut som mappas tillämpas varje gång en användare loggar in via enkel inloggning.

  Exempel: Om du mappar&quot;efternamn&quot; och uppdaterar deras namn i Workfront utan att uppdatera värdet i deras identitetsleverantör, skrivs efternamnet över så att det matchar värdet i identitetsleverantören nästa gång användaren loggar in.

## Mappa användarattribut för din organisation

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-left.png) i det övre vänstra hörnet av Adobe Workfront och klicka sedan på ikonen **Konfigurera** ![Nätövertoningsinställningar](assets/gear-icon-settings.png) .

1. Klicka på **System** > **enkel inloggning (SSO)**.

1. Klicka på fliken **Adobe**.

1. (Valfritt och villkorligt) Om attributmappningen i den klassiska upplevelsen har konfigurerats i organisationen och du vill kopiera den attributmappningen till den enhetliga Adobe-upplevelsen klickar du på **Migrera mappningar**. Du kan sedan ta bort, ta bort eller redigera mappningarna.

   >[!NOTE]
   >
   >Vi rekommenderar att du migrerar mappningar första gången du konfigurerar mappningar i Adobe enhetliga upplevelse. Det skadar inte att migrera dem igen senare, men det är inte nödvändigt att migrera dem mer än en gång.

1. Om du vill skapa en ny attributmappning klickar du på **Lägg till mappning**.

1. Klicka på pilen bredvid fältnamnet för Workfront och markera fältet [!DNL Workfront] som du vill mappa till.

1. (Valfritt) Om du vill skapa mer än en regel för ett givet fält klickar du på pilen bredvid **Alltid** och väljer den operator som du vill att regeln ska använda.

1. (Villkorligt) Om du har valt en operator förutom Alltid, markerar du fältet Workfront och värdet som operatorn gäller för.

   >[!NOTE]
   >
   >Operatorerna `Is Truthy` och `Is Falsy` kräver inga värden.

1. Välj om du vill använda värdet för ett attribut i din identitetshanterare på fältet Workfront eller om du vill använda ett visst konstantvärde.

1. Ange namnet på det identitetshanteringsfält som du vill använda, eller ange texten för det konstanta värde som du vill använda.

1. (Valfritt) Om du vill lägga till fler regler för samma Workfront-fält klickar du på **Lägg till ny regel** och följer steg 4-9.

   >[!IMPORTANT]
   >
   > * Alla linjer under och alltid kommer att ignoreras. Om du har en regel för alltid måste du flytta den längst ned i listan med regler. Du kan flytta regler i listan genom att klicka på menyn med tre punkter till höger om linjen och flytta regeln uppåt eller nedåt.
   > * Om du vill skapa en regel i mitten av listan klickar du på menyn med tre punkter bredvid regeln som du vill placera ovanför eller nedanför den nya regeln och väljer **Lägg till regel ovanför** eller **Lägg till regel nedanför**.

1. Om du vill ta bort en regel klickar du på menyn med tre punkter bredvid regeln som du vill ta bort och väljer **Ta bort**.
1. Om du vill ta bort en mappning klickar du på ikonen **Ta bort** som finns på kortet för den mappningen.

1. Om du vill spara bläddrar du längst upp på sidan och klickar på **Spara**.


