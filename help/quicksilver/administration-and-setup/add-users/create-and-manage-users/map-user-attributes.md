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
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 0%

---

# Mappa användarattribut

<!--Audited 2/2024-->

Med enkel inloggning (SSO) kan du skicka attribut från identitetsleverantörens Active Directory till dina Adobe Workfront-användare.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p><p>eller</p><p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tips för mappningsattribut

Tänk på följande när du mappar attribut:

* Testa alltid i en förhandsvisningssandlåda eller i en CR-sandlåda (Customer Refresh).
* Testa med både administratörskonton och icke-administratörskonton för att bekräfta att du mappar attribut korrekt.
* Attribut som mappas tillämpas varje gång en användare loggar in via enkel inloggning.

  Exempel: Om du mappar&quot;efternamn&quot; och uppdaterar deras namn i Workfront utan att uppdatera värdet i deras identitetsleverantör, skrivs efternamnet över så att det matchar värdet i identitetsleverantören nästa gång användaren loggar in.

## Mappa användarattribut för din organisation

Hur du mappar attribut varierar beroende på om din organisation använder den enhetliga upplevelsen i Adobe.

Om du vill ta reda på om din organisation har en enhetlig Adobe-upplevelse kan du kontrollera den URL som du använder för att få tillgång till Workfront.

| URL | Adobe Experience |
|---|---|
| (CompanyName).my.workfront.com | Klassisk erfarenhet |
| experience.adobe.com | Adobe enhetliga upplevelse |

* [Mappa användarattribut i den klassiska upplevelsen](#map-user-attributes-in-the-classic-experience)
* [Mappa användarattribut i Adobe enhetliga upplevelse](#map-user-attributes-in-the-adobe-unified-experience)

### Mappa användarattribut i den klassiska upplevelsen

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på ikonen **Konfigurera** ![Nätövertoningsinställningar](assets/gear-icon-settings.png) .

1. Klicka på **System** > **enkel inloggning (SSO)**.

1. Klicka på **SAML 2.0** i listrutan **Typ**.

1. Klicka på **Mappa användarattribut**.

   ![Mappa användarattribut](assets/map-user-attributes.png)

1. I den rad med alternativ som visas mappar du de attribut du behöver för dina Workfront-användare.

   Du kan mappa attribut som adress, chef, jobbroll, hemgrupp och så vidare.

   Attributmappningar fungerar med ett 1:1-förhållande. Du kan till exempel inte ange alla grupper som en användare tillhör. Du kan bara ange en per användare.

   >[!IMPORTANT]
   >
   >Vi rekommenderar inte att du mappar åtkomstnivåer i attributmappningar. Om du gör det ska du vara försiktig när du anger standardvärdet för att vara säker på att du inte tar bort Admin Access av misstag.

   I följande tabell förklaras de fält som du kan använda för att mappa attribut:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Workfront-användarattribut</td> 
      <td>Välj namnet på attributet som du mappar</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Katalogattribut</td> 
      <td>Skriv den SSO-attributetikett som du vill använda.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardvärde</td> 
      <td> <p>När du har valt ett Workfront-användarattribut fylls det här fältet i med motsvarande standardvärde i systemet om värdet är NULL under anslutningen. Ange bara ett värde här om du tänker tillämpa reglerna för attributmappning (se steg 7). Standardvärdet fungerar som ett undantag till dessa regler.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Klicka på **Regler** om du vill lägga till en regel i attributet.

   1. I listrutan väljer du den attributmodifierare som du vill använda.
   1. I de två fälten till höger anger du värdet för katalogattributet och det värde som du vill ersätta det med.

      ![Regelfält](assets/rule-fields.png)

   Du kan klicka på **Lägg till regel** om du vill lägga till fler regler i attributet.

1. (Valfritt) Om du vill mappa fler användarattribut klickar du på **Lägg till mappning** och upprepar steg 6-7.
1. Klicka på **Spara**.

### Mappa användarattribut i Adobe enhetliga upplevelse

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-left.png) i det övre vänstra hörnet av Adobe Workfront och klicka sedan på ikonen **Konfigurera** ![Nätövertoningsinställningar](assets/gear-icon-settings.png) .

1. Klicka på **System** > **enkel inloggning (SSO)**.

1. Klicka på fliken **Adobe**.

1. (Valfritt och villkorligt) Om din organisations attributmappning har konfigurerats i den klassiska upplevelsen och du vill kopiera den attributmappningen till den enhetliga Adobe-upplevelsen klickar du på **Migrera mappningar**. Du kan sedan ta bort, ta bort eller redigera mappningarna.

   >[!NOTE]
   >
   >Vi rekommenderar att du migrerar mappningar första gången du konfigurerar mappningar i den enhetliga Adobe-upplevelsen. Det skadar inte att migrera dem igen senare, men det är inte nödvändigt att migrera dem mer än en gång.

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


