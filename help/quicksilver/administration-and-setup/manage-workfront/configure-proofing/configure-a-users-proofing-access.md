---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Konfigurera en användares språkåtkomst
description: Som Adobe Workfront-administratör eller Workfront Proof-administratör kan du konfigurera en användares åtkomst till att skapa och visa korrektur i Workfront och Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 0%

---

# Konfigurera en användares språkkontroll

Som Adobe Workfront-administratör eller Workfront Proof-administratör kan du konfigurera en användares åtkomst till att skapa och visa korrektur i Workfront och Workfront Proof.

Mer information om korrekturfunktioner för grundläggande och integrerad korrektur finns i [Åtkomst till korrekturfunktioner i Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara Workfront-administratör eller Workfront Proof-administratör. Mer information om Workfront-administratörer finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Aktivera och inaktivera korrektur för en användare (endast äldre planer) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Om din organisation använder en äldre Select- eller Premium Workfront-plan, som Workfront-administratör, kan du aktivera och inaktivera språkfunktioner för användaren.

När du aktiverar korrektur för en användare aktiveras alternativet att användarens korrektur genereras automatiskt i Workfront.

Även om du kan aktivera en användare som korrekturanvändare måste han eller hon ha administratörsbehörighet för att kunna navigera direkt till Workfront Proof-gränssnittet från Workfront huvudmeny. Information om hur du kan aktivera det här alternativet för alla språkanvändare i ditt Workfront-system finns i [Konfigurera Workfront Proof-åtkomst via Workfront huvudmeny för alla användare](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. Välj **Användare** på **huvudmenyn**.

1. Markera en användare och klicka sedan på ikonen **Redigera** .
1. I avsnittet **Åtkomst** markerar eller avmarkerar du **Användaren kan generera korrektur**.

## Konfigurera en användares behörighetsprofil för korrektur

Den behörighetsprofil du väljer tilldelas användarna för varje bevis som finns i organisationen.

{{step-1-to-users}}

1. Markera en eller flera användare och klicka sedan på **Redigera**.

1. I avsnittet **Åtkomst** klickar du på något av följande Workfront Proof-behörighetsalternativ i listrutan **Korrekturprofil**:

   >[!NOTE]
   >
   >Om du har en äldre Workfront-plan kontrollerar du att alternativet **Användare kan generera korrektur** är aktiverat, vilket förklaras ovan i avsnittet [Aktivera och inaktivera korrektur för en användare (endast äldre planer)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Ansvarig</strong> </td> 
      <td>Användare kan hantera och visa alla korrektur som skapats på organisationens konto. De kan även redigera granskare som lagts till i dessa korrektur. Användare med den här behörighetsprofilen kan inte hantera användare eller redigera Workfront Proof-inställningar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Hanteraren</strong> </td> 
      <td> <p> Användare kan hantera och visa korrektur som skapats eller ägs av organisationens konto. De kan bara visa andra användares korrektur när de läggs till som granskare. Det här är en standardinställning. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administratör</strong> </td> 
      <td> Användare får administratörsbehörighet i Workfront Proof och kan redigera kontoinställningar. Användare kan hantera och visa alla korrektur som skapats på organisationens konto. Detta inkluderar att lägga till och ta bort granskare, korrektur och kommentarer.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Egen</strong> </td> 
      <td> <p>Endast tillgängligt om du har konfigurerat en anpassad behörighetsprofil i Workfront Proof.</p> <p><b>OBS</b>:  <p>Se till att den behörighetsprofil du anger här inte ger högre åtkomst än användarens åtkomstnivåinställning i Workfront (se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>). Om det ger bättre åtkomst kan användaren få åtkomst till korrektur i Workfront Proof som han eller hon inte har åtkomst till inom Workfront.</p> <p>Detta är särskilt viktigt om du tänker tillåta alla Workfront-användare att få tillgång till Workfront Proof direkt från Workfront enligt beskrivningen i <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Få åtkomst till Workfront Proof från Adobe Workfront</a>.</p> <p>Som standard har bara Workfront-administratörer tillgång till en direktlänk till Workfront Proof-webbplatsen från Workfront Global Navigation Bar.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Den behörighetsprofil du väljer tilldelas användarna för varje bevis som finns i organisationen.

1. Klicka på **Spara ändringar** för att slutföra uppdateringen av användarinställningarna.

   >[!NOTE]
   >
   >När du skapar eller uppdaterar en användare i Workfront och användarens Workfront-e-postadress matchar en licensierad Workfront Proof-användare aktiveras språkkontroll för användaren i Workfront. Mer information finns i [Användarsynkronisering mellan Adobe Workfront och Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Överväganden

Tänk på följande information när du anger behörigheter:

* Om du ändrar en användares behörighetsprofil till en profil med mindre behörigheter kan användaren förlora synligheten för befintliga korrektur i Workfront. Detta kan inträffa när någon delar en uppgift med en användare i Workfront, men inte delar det korrektur som är kopplat till uppgiften (se [Dela ett korrektur i Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) i [Dela ett korrektur i Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* Du kan bara ange Workfront Proof-behörigheter från Workfront om din Workfront-miljö är integrerad med ett Workfront Proof Premium-konto. Kontakta Workfront-administratören om du inte kan använda korrektur enligt beskrivningen i det här avsnittet.
* Minst en användare i din Workfront-miljö måste ha administratörsbehörighet för korrektur. Ett felmeddelande visas om du försöker ta bort administratörsbehörighet för korrektur från alla användare.
* När du ändrar en användares Workfront Access-nivå till någon annan nivå än systemadministratören, används användarens Workfront Proof-behörighetsprofil som standardvärde för Hanterare.

* När du ändrar Workfront Access-nivån till Systemadministratör ändras behörigheten för Korrekturinställningar till Administratör.

## Konfigurera Workfront Proof-åtkomst via Workfront huvudmeny för alla användare {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Som standard kan bara användare med administratörsbehörighet i Workfront få åtkomst till Workfront Proof enligt beskrivningen i [Få åtkomst till Workfront Proof från Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Du kan ge alla användare åtkomst till Workfront Proof-knappen på Workfront huvudmeny genom att kontakta Workfront Support och lämna en begäran.

>[!IMPORTANT]
>
> Om du tänker tillåta alla Workfront-användare att komma åt Workfront Proof direkt från Workfront Global Navigation Bar kontrollerar du att behörighetsprofilen för varje användare inte ger mer åtkomst än användarens åtkomstnivå inom Workfront. Detta förhindrar att användare får åtkomst till korrektur i Workfront Proof som de inte har åtkomst till inom Workfront. Mer information finns i [Aktivera och inaktivera korrektur för en användare (endast äldre planer)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Konfigurera användaråtkomst till Desktop Proofing Viewer

Om användarna i din organisation föredrar att använda Desktop Proofing Viewer istället för Web Proofing Viewer för att granska interaktivt innehåll, kan du konfigurera Desktop Proofing Viewer så att den startas automatiskt när användare öppnar interaktiva innehållskorrektur. Information om detta i Desktop Proofing Viewer och om hur det skiljer sig från Web Proofing Viewer finns i [Förstå Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) och [Skillnader mellan Web Proofing Viewer och Desktop Proofing Viewer ](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. I Workfront klickar du på Workfront Proof-ikonen i det globala navigeringsfältet för att komma åt Workfront Proof.

   ![Korrekturikon](assets/proof-access-proofhq-350x39.png)

1. Klicka på **Kontoinställningar** i det övre högra hörnet av Workfront Proof och klicka sedan på fliken **Inställningar** .

1. Under **Korrekturinställningar** klickar du på **Konfigurera** i slutet av raden **Språkkontroll för interaktivt korrektur**.

1. Ändra inställningarna för Desktop Proofing Viewer, enligt beskrivningen i [Desktop Proofing Viewer](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) i artikeln [Konfigurera korrekturinställningar för din organisation](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Klicka på **Spara**.

## Konfigurera anpassade enheter för interaktiva korrektur

Du kan lägga till anpassade enheter i systemet, så att användarna kan granska interaktivt innehåll och simulera hur innehållet visas på en viss enhet när de använder Desktop Proofing Viewer. (Den här funktionen är inte tillgänglig i Web Proofing Viewer, där användare kan granska interaktivt innehåll, men bara som det visas i olika upplösningar, inte på olika enheter.)

Mer information finns i [Ändra interaktiv korrekturupplösning i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Från Workfront får du tillgång till Workfront Proof-gränssnittet enligt beskrivningen i [Få åtkomst till Workfront Proof från Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Ändra inställningarna för Desktop Proofing Viewer, enligt beskrivningen i [Konfigurera anpassade enheter för korrektur](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) i artikeln [Konfigurera korrekturinställningar för din organisation](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
