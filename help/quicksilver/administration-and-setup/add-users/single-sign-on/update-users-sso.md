---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Uppdatera användare för enkel inloggning
description: Du kan uppdatera användare för enkel inloggning i Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# Uppdatera användare för enkel inloggning

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

När enkel inloggning (SSO) är aktiverad i din Adobe Workfront-instans kan dina användare logga in i Workfront med sina SSO-inloggningsuppgifter.

Om du har ett befintligt system som redan är ifyllt med användare som är kopplade till SSO-inloggningsuppgifter, kan du importera användarens ID:n till Workfront genom att importera en kommaseparerad värdefil (CSV) till Workfront.

Mer information om hur du integrerar Workfront med ett SSO-system finns i [Översikt över enkel inloggning i Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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
   <td> <p>Du måste vara Workfront-administratör.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## SSO-användarnamn

Beroende på vilken SSO-lösning du använder kan användarnamnet i SSO-miljön kallas något av följande:

* SSO-användarnamn
* Federations-ID
* Federationsanvändarnamn

Oavsett vad användarnamnet kallas i SSO-miljön lagras fältets värde i SSO-användarnamnsfältet i User-objektet.

För att dina användare ska kunna använda sina inloggningsuppgifter för enkel inloggning för att logga in på Workfront måste du uppdatera deras profil så att även användarnamnet för enkel inloggning ingår, förutom Workfront användarnamn.

Som Workfront-administratör kan du uppdatera SSO-användarnamnsfältet för dina Workfront-användare genom att importera en lista med användarnamn till Workfront. Denna lista måste

* Innehåller Workfront användar-ID (GUID) och motsvarande SSO-användarnamn för varje användare
* Spara som en CSV- eller TSV-fil.

Den här processen uppdaterar antingen befintliga SSO-användarnamn i Workfront eller lägger till ett nytt SSO-användarnamn, om ett sådant saknas för användarna.

## Förbered importfilen {#prepare-the-import-file}

Du kan börja förbereda din importfil genom att skapa en rapport över alla användare i Workfront som måste ha sina fält för SSO-användarnamn uppdaterade.

1. Skapa en användarrapport i Workfront.

   Instruktioner om hur du skapar användarrapporter i Workfront finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Välj följande fält i rapporten:

   | Fält | Förklaring |
   |---|---|
   | Namn | Workfront-användarens fullständiga namn. |
   | ID | ID:t är Workfront alfanumeriska GUID. |
   | SSO-användarnamn | Genom att lägga till SSO-användarnamnsfältet försäkrar du dig om att inga användarnamn skrivs över med importen. Det här fältet ska vara tomt för alla användare, om dina användare ännu inte har uppdaterats för enkel inloggning. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Spara rapporten.
1. Klicka **Exportera** överst i rapporten och exportera rapporten till Excel.
1. Öppna den exporterade Excel-filen och lägg till SSO-användarnamn för varje användare i rapporten i kolumnen SSO-användarnamn.

   >[!IMPORTANT]
   >
   >SSO-användarnamn är skiftlägeskänsliga.

1. Ta bort alla kolumner i Excel-filen, förutom **ID** och **SSO-användarnamn** kolumner.

1. Ta bort kolumnrubrikerna och kontrollera att det inte finns några tomma rader överst i rapporten.

   Den fil du använder för att uppdatera dina Workfront-användare med SSO-användarnamn **måste** innehåller bara 2 kolumner, i den här ordningen:

   * I den första kolumnen måste användar-ID:t (användar-GUID:t som i Workfront) visas.
   * Den andra kolumnen måste innehålla SSO-användarnamnet, som det visas i SSO-systemet.
   * Kolumnerna får inte ha några rubriker och det får inte finnas några tomma rader överst i namnlistan.

     ![](assets/update-users-for-sso-csv-file-for-import.png)

1. Spara rapporten som en CSV- eller TSV-fil på datorn.

## Uppdatera dina användare för enkel inloggning {#update-your-users-for-sso}

Processen att uppdatera användare för enkel inloggning lägger antingen till SSO-användarnamnsfältet till dina Workfront-användare om det inte finns någon, eller uppdaterar värdet i det fältet om det redan finns ett värde kopplat till användarna.

1. Klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om tillgängligt), klicka på **[!UICONTROL Main Menu]** icon ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka, **System** välj **Uppdatera användare för enkel inloggning**.

1. Klicka **Välj fil** för att bläddra efter filen som du har förberett.

   Mer information om hur du förbereder den här filen finns i [Förbered importfilen](#prepare-the-import-file).

1. Markera den fil som filen sparas från på datorn och klicka sedan på **Öppna**.

   Detta infogar SSO-inloggningsuppgifterna till Workfront, så att alla användare kan logga in på Workfront med sina SSO-inloggningsuppgifter.

   The **Tillåt endast `<SSO Configuration>` Autentisering** inställningen är aktiverad för alla användare som ingår i CSV-filen. Detta garanterar att användarna måste logga in via enkel inloggning.

## Verifiera enkel inloggning mot dina användares Workfront-användarnamn

Instruktioner om hur du skapar en användarrapport som innehåller information om SSO-användarnamn finns i [Förbered importfilen](#prepare-the-import-file).

1. Kör en användarrapport som innehåller information om SSO-användarnamn.

   Observera att SSO-användarnamnskolumnen fylls i för varje användare.

1. Kontrollera att värdena för kolumnen SSO-användarnamn matchar SSO-användarnamnet på SSO-servern.
1. Om kolumnen SSO-användarnamn är tom uppdaterar du användarnas SSO-användarnamn.

   ![](assets/users-with-sso-field-updated.png)

   Instruktioner om hur du uppdaterar användare för enkel inloggning finns i [Uppdatera dina användare för enkel inloggning](#update-your-users-for-sso).
