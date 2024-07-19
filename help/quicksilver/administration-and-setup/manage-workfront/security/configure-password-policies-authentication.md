---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Konfigurera lösenordsprinciper för autentisering
description: Som Adobe Workfront-administratör kan du konfigurera lösenordsprinciper för att anpassa autentiseringsupplevelsen till ditt Workfront-system.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 970cc86b00dc1afe0473ac3a387e7ce47e4a2433
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 0%

---

# Konfigurera lösenordsprinciper för autentisering

{{important-admin-console-onboard}}

Som Adobe Workfront-administratör kan du konfigurera lösenordsprinciper för att anpassa autentiseringsupplevelsen till ditt Workfront-system.

Vi rekommenderar att du konfigurerar autentiseringsinställningarna under Workfront-implementeringen och endast tillfälligt kan gå tillbaka till dem efteråt.

Förbättrade funktioner för lösenordshantering kommer snart eller finns redan tillgängliga för din organisation. Använd något av följande avsnitt, beroende på om din organisation har tillgång till den nya autentiseringsupplevelsen.

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
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera autentisering (tillgänglig för alla kunder) {#configure-authentication-available-for-all-customers}

Autentiseringsalternativ visas för alla kunder. Förbättrade funktioner för lösenordshantering kommer snart eller är kanske redan tillgängliga för din organisation, vilket beskrivs i avsnittet [Konfigurera förbättrad autentisering)](#configure-enhanced-authentication-coming-soon) i den här artikeln.

Så här konfigurerar du autentiseringsinställningar:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **System** > **Autentisering**.

1. Välj något av följande fält för att ange autentiseringsinställningar för din organisation:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tvinga användare att återställa sitt lösenord var <em>&lt;värde&gt;</em> dag</td> 
      <td>Detta anger tidsramen för när användare ska återställa sitt Workfront-lösenord. Som standard är det här alternativet inaktiverat. När du aktiverar den kan du välja mellan 30, 60, 90, 120 och 180 dagar. Standardvärdet är 30 dagar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt inte användare att ange samma lösenord som något av deras tidigare <em>&lt;värde&gt;</em>-lösenord</td> 
      <td> <p>Det här fältet förhindrar att användare återanvänder lösenord för ett visst antal återställningar. Som standard är det här fältet inaktiverat. När du aktiverar det kan du ange värdet 5, 10 eller 15 för att återställa ett lösenord innan det kan återanvändas.</p> <p>När det här alternativet är markerat kan användare inte återställa sina lösenord mer än en gång på en given dag</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Om ett felaktigt lösenord anges fem gånger i följd låser du kontot i <em>&lt;värde&gt;</em> minuter: </td> 
      <td> <p>Ange hur länge en användare ska låsas ut från Workfront efter att ett felaktigt lösenord har angetts fem gånger i rad. Som standard är det här alternativet aktiverat och väntetiden är 10 minuter. Du kan låsa konton i 10 minuter, 30 minuter, 1 timme, 8 timmar eller 24 timmar. </p> <p>Om du återställer lösenordet för användaren manuellt åsidosätts det här standardväntevärdet. <br>Användare kan återställa sina egna lösenord när de är utlåsta via inloggningsskärmen. Mer information om hur de kan återställa sitt lösenord, om de har glömt det, finns i <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Återställ ditt lösenord</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lösenord måste innehålla minst <em>&lt;värde&gt;</em> olika typer av tecken:</td> 
      <td> <p>Anger hur starka användarlösenord som krävs genom att du kan välja antalet olika typer av tecken som krävs i dina lösenord.</p> <p>Ett identifierbart ordlisteord kan inte användas som lösenord.<br>Som standard kräver Workfront att minst två av följande finns i lösenord (du kan även kräva att 3 av dessa tecken finns för ett giltigt lösenord): </p> 
       <ul> 
        <li>Versaler</li> 
        <li>Gemener</li> 
        <li>Nummer</li> 
        <li>Symboler</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara**.

## Konfigurera förbättrad autentisering{#configure-enhanced-authentication-coming-soon}

I det här avsnittet beskrivs den förbättrade autentiseringsupplevelsen, som kanske inte är tillgänglig för din organisation ännu. Om din organisation inte har migrerats till den nya autentiseringsupplevelsen måste du konfigurera autentiseringsinställningarna enligt beskrivningen i [Konfigurera autentisering (tillgänglig för alla kunder)](#configure-authentication-available-for-all-customers).

Så här konfigurerar du utökade autentiseringsinställningar:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Konfigurera** ![](assets/gear-icon-settings.png) .

1. Klicka på **System** > **Förbättrad autentisering**.
1. Ange det minsta antalet tecken som krävs för ett giltigt lösenord i rutan **Lösenordslängd**.

   Workfront kräver minst 6 tecken.

1. (Valfritt) I avsnittet **Lösenordskrav** väljer du de typer av tecken som krävs i användarlösenord.

   Du kan öka styrkan på användarlösenord genom att kräva någon eller alla typer av tecken i avsnittet Lösenordskrav. Följande alternativ är tillgängliga:

   | Gemener | Kräv minst en gemen bokstav |
   |---|---|
   | Versaler | Kräv minst en versal |
   | Nummer | Kräv minst en siffra |
   | Specialtecken | Kräv minst ett specialtecken |

   {style="table-layout:auto"}

1. Klicka på **Spara**.
