---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Mappa användarattribut och autodistribuera nya användare
description: Med enkel inloggning (SSO) kan du skicka attribut från identitetsleverantörens Active Directory till dina Adobe Workfront-användare. Du kan också lägga till nya användare i Workfront med alternativet Automatisk etablering (kallas även Just In Time Provisioning (Tidsetablering) eller JIT).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Mappa användarattribut och autodistribuera nya användare

Med enkel inloggning (SSO) kan du skicka attribut från identitetsleverantörens Active Directory till dina Adobe Workfront-användare. Du kan också lägga till nya användare i Workfront med alternativet Automatisk etablering (kallas även Just In Time Provisioning (Tidsetablering) eller JIT).

>[!NOTE]
>
>Detta är inte tillgängligt om din organisation har anslutit sig till Adobe Admin Console. Kontakta nätverks- eller IT-administratören om du behöver mer information.


## Åtkomstkrav

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tips för mappningsattribut

Tänk på följande när du mappar attribut:

* Testa alltid i en förhandsvisningssandlåda eller i en CR-sandlåda (Customer Refresh).
* Testa med både administratörskonton och icke-administratörskonton för att bekräfta att du mappar attribut korrekt.
* Attribut mappas varje gång en användare loggar in på Workfront via enkel inloggning, inte bara under automatisk etablering.

## Mappa användarattribut och autodistribuera nya användare

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **System** > **enkel inloggning (SSO)**.

1. I **Typ** nedrullningsbar meny, klicka **SAML 2.0**.

1. Klicka **Mappa användarattribut**.

   ![](assets/map-user-attributes.png)

1. (Valfritt) Om du vill att Workfront ska skapa nya användare från din Active Directory automatiskt klickar du på **Automatisk etablering av användare**.

   Den här funktionen kräver attributmappning.

1. I den rad med alternativ som visas mappar du de attribut du behöver för dina Workfront-användare.

   Du kan mappa attribut som adress, chef, jobbroll, hemgrupp och så vidare.

   Attributmappningar fungerar med ett 1:1-förhållande. Du kan till exempel inte ange alla grupper som en användare tillhör; du bara kan ange en per användare.

   >[!IMPORTANT]
   >
   >Följande attribut krävs för varje användare:
   >      
   >* Förnamn
   >* Efternamn
   >* E-postadress

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
      <td>Skriv den SSO-attributetikett som du vill använda./td&gt; 
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

      ![](assets/rule-fields.png)
   Du kan klicka **Lägg till regel** om du vill lägga till fler regler i attributet.

1. (Valfritt) Om du vill mappa fler användarattribut klickar du på **Lägg till mappning** och upprepa steg 6-7.
1. Klicka **Spara**.
