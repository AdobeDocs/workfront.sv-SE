---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Förbered er på att anställa Adobe Admin Console
description: Eftersom Adobe Workfront är en Adobe-produkt kan du komma åt den via Adobe Admin Console. På så sätt kan du hantera Workfront tillsammans med andra Adobe-konton och -produkter för dina användare centralt.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Förbered er på att anställa Adobe Admin Console

Eftersom Adobe Workfront är en Adobe-produkt kan du komma åt den via Adobe Admin Console. På så sätt kan du hantera Workfront tillsammans med andra Adobe-konton och -produkter för dina användare centralt.

Alla Workfront-kunder kommer till slut att flyttas till Adobe Admin Console. När ni har flyttat till Adobe Admin Console hanteras Workfront autentisering av Adobe Admin Console. Om ni förbereder och gör det här steget tidigare lägger ni grunden för effektiv arbetshantering och positionerar organisationen för snabbare innovation i framtiden

En översikt över Adobe Admin Console finns på [Översikt över Admin Console](https://helpx.adobe.com/se/enterprise/using/admin-console.html).

## Checklista för migrering

För att din organisation ska kunna migrera till Adobe Admin Console måste du utföra följande åtgärder:

1. Identifiera Adobe Admin Console där du vill lägga till Workfront.

   * Om din organisation inte har någon befintlig Adobe Admin Console, eller om du inte vill använda en befintlig Adobe Admin Console, kan Workfront Support hjälpa dig att skapa en ny.

   * Om du har flera Adobe Admin Console och är osäker på vilken som är bäst att lägga till Adobe Workfront i kontaktar du Workfront support.

1. Bekräfta med Workfront Support att du vill använda en befintlig Adobe Admin Console eller skapa en ny.

1. Konfigurera identitetshantering för Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Var beredd att tala med Workfront Support och ditt IT-team om autentiseringsinställningar som enkel inloggning (SSO) eller icke-enkel inloggning (SSO).

   Instruktioner finns i avsnittet om Identity Management i distributionsguiden för Adobe Admin Console (https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. (Villkorligt) Om du använder enkel inloggning ansluter du den nya Adobe Admin Console till din befintliga SSO-leverantör

   Mer information och instruktioner finns i [Konfigurera identitet](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Om din organisation inte använder enkel inloggning får alla användare som migrerats till Adobe Admin Console ett e-postmeddelande för att skapa sitt konto och lösenord.

1. Kontrollera att användarens e-postadresser är klara för migrering:

   1. Ta bort dubbla e-postmeddelanden från Workfront

      Instruktioner finns i Uppdatera e-postadresser för befintliga användare i din Workfront-instans i Förhindra duplicerade användare.

      Om det finns dubbla e-postadresser i organisationen, representeras användaren av e-postadressen med den senaste `lastLoginDate` kommer att flyttas till Adobe Admin Console. Andra användare med den e-postadressen inaktiveras.

      >[!NOTE]
      >
      >Eftersom endast en användare med en viss e-postadress kan vara aktiv vid en viss tidpunkt måste du först inaktivera den aktiva användaren innan du aktiverar den inaktiverade användaren om du behöver aktivera en annan användare med samma e-postadress som en aktiv användare.

   2. (Villkorligt) Om du använder anpassade API-integreringar ska du kontrollera att användarna har en giltig e-postadress som de har tillgång till.

   3. (Valfritt) Vi rekommenderar att användare som inte längre behöver åtkomst till Workfront inaktiveras så att de inte läggs till i Adobe Admin Console.
   >[!IMPORTANT]
   >
   >Dessa åtgärder för användarens e-post måste vara slutförda innan din organisation kan börja gå över till Adobe Admin Console.

1. (Valfritt) Uppdatera alla anpassade integreringar så att OAuth2 används.

   Instruktioner om hur du konfigurerar OAuth2-integreringar finns i [Skapa OAuth2-program för Workfront-integreringar](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   Det går bara att skapa OAuth2-integreringar i den nya Workfront-upplevelsen.

   >[!NOTE]
   >
   >Det här steget är valfritt, men rekommenderas starkt eftersom andra former av API-autentisering och -auktorisering kommer att bli inaktuella i framtiden.

När din Adobe Admin Console har konfigurerats med Workfront kan du använda den för att hantera dina användare.

Mer information finns i [Hantera användare i Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

En lista över andra åtgärder som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns på [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
