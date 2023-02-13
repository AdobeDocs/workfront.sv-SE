---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Uppdatera användare för enkel inloggning
description: Du kan uppdatera användare för enkel inloggning i Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 2cbdd0cb065dee01ad128d782334a55233c13156
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 0%

---

# Uppdatera användare för enkel inloggning

{{important-admin-console-onboard}}

När enkel inloggning (SSO) är aktiverat i din Adobe Workfront-instans kan du logga in på Workfront med dina SSO-inloggningsuppgifter.

Om du har ett befintligt system som redan är ifyllt med användare som är kopplade till SSO-inloggningsuppgifter, kan du importera användarens ID:n till Workfront genom att importera en kommaseparerad värdefil (CSV) till Workfront.

Mer information om hur du integrerar Workfront med ett SSO-system finns i [Översikt över enkel inloggning i Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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

## SSO-användarnamn

Beroende på vilken SSO-lösning du använder kan användarnamnet i SSO-miljön kallas något av följande:

* SSO-användarnamn
* Federations-ID
* Federationsanvändarnamn

I Workfront lagras alla dessa namn i SSO-användarnamnsfältet på användarobjektet.

För att dina användare ska kunna använda sina inloggningsuppgifter för enkel inloggning för att logga in på Workfront måste du uppdatera deras profil så att även användarnamnet för enkel inloggning ingår, förutom Workfront användarnamn.

Som Workfront-administratör kan du uppdatera SSO-användarnamnsfältet gruppvis för dina Workfront-användare genom att använda en lista med användarnamn och importera det till Workfront. Listan måste innehålla Workfront användar-ID (GUID) samt motsvarande SSO-användarnamn för varje användare och måste sparas som en CSV- eller TSV-fil. Den här processen uppdaterar antingen befintliga SSO-användarnamn i Workfront eller lägger till ett nytt SSO-användarnamn, om ett sådant saknas för användarna.

## Förbered importfilen {#prepare-the-import-file}

Du kan börja förbereda din importfil genom att skapa en rapport över alla användare i Workfront som måste ha sina fält för SSO-användarnamn uppdaterade.

1. Skapa en användarrapport i Workfront.

   Instruktioner om hur du skapar användarrapporter i Workfront finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Välj följande fält i rapporten:

   | Namn | Workfront-användarens fullständiga namn. |
   |---|---|
   | ID | ID:t är Workfront alfanumeriska GUID. |
   | SSO-användarnamn | Markera SSO-användarnamnsfältet för att kontrollera att det inte finns några användarnamn som du skriver över vid importen. Det här fältet ska vara tomt för alla användare, om dina användare ännu inte har uppdaterats för enkel inloggning. |

   ![](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Spara rapporten.
1. Klicka **Exportera** överst i rapporten och exportera rapporten till Excel.
1. Öppna den exporterade Excel-filen och börja lägga till dina SSO-användarnamn för varje användare i rapporten i kolumnen SSO-användarnamn.

   >[!IMPORTANT]
   >
   >SSO-användarnamn är skiftlägeskänsliga.

1. Ta bort alla kolumner i Excel-filen, förutom **ID** och **SSO-användarnamn** kolumner.

1. Eliminera kolumnrubrikerna och se till att det inte finns några tomma rader överst i rapporten.

   Filen som du använder för att uppdatera dina Workfront-användare med SSO-användarnamn måste innehålla endast två kolumner, i följande ordning:

   * I den första kolumnen ska användar-ID:t (användar-GUID:t som i Workfront) visas.
   * Den andra kolumnen ska innehålla SSO-användarnamnet, som det visas i SSO-systemet.
   * Kolumnerna får inte ha några rubriker och det får inte finnas några tomma rader överst i namnlistan.

      ![](assets/update-users-for-sso-csv-file-for-import.png)

1. Spara rapporten som en CSV- eller TSV-fil på datorn.

## Uppdatera dina användare för enkel inloggning {#update-your-users-for-sso}

Processen att uppdatera användare för enkel inloggning lägger antingen till SSO-användarnamnsfältet till dina Workfront-användare om det inte finns någon, eller uppdaterar värdet i det fältet om det redan finns ett värde kopplat till användarna.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **System** sedan **Uppdatera användare för enkel inloggning**.

1. Klicka **Välj fil** för att bläddra efter filen som du har förberett.

   Mer information om hur du förbereder den här filen finns i [Förbered importfilen](#prepare-the-import-file).

1. Markera filen där den har sparats på datorn och klicka sedan på **Öppna**.

   Detta gör att alla användare kan logga in på Workfront med sina SSO-inloggningsuppgifter.

   The **Tillåt endast `<SSO Configuration>` Autentisering** inställningen är aktiverad för alla användare som ingår i CSV-filen.

## Verifiera enkel inloggning för dina användares Workfront-användarnamn

Instruktioner om hur du skapar en användarrapport som innehåller information om SSO-användarnamn finns i [Förbered importfilen](#prepare-the-import-file).

1. Kör en användarrapport som innehåller information om SSO-användarnamn.

   Observera att SSO-användarnamnskolumnen fylls i för varje användare.

1. Kontrollera att värdena för kolumnen SSO-användarnamn matchar SSO-användarnamnet på SSO-servern.
1. Om kolumnen SSO-användarnamn är tom uppdaterar du användarnas SSO-användarnamn.

   ![](assets/users-with-sso-field-updated.png)

   Instruktioner om hur du uppdaterar användare för enkel inloggning finns i [Uppdatera dina användare för enkel inloggning](#update-your-users-for-sso).
