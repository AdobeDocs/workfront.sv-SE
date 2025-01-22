---
title: Bevilja fullständig administratörsåtkomst för användare
description: Du kan ge användare fullständig administrativ åtkomst till Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 46bcb65a-1cb7-443b-88ba-6d0e516e3050
source-git-commit: eb68357ed4fd8f323707aa4a54a0f946253bf4e0
workflow-type: tm+mt
source-wordcount: '1550'
ht-degree: 0%

---

# Bevilja användaren fullständig administrativ åtkomst

<!--Audited: 12/2024-->

>[!IMPORTANT]
>
>Det förfarande som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Admin Console. Om du har anslutit dig till Adobe Admin Console måste du utföra den här åtgärden via Adobe Admin Console.
>
>Instruktioner om hur du ger fullständig administratörsåtkomst i Adobe Admin Console finns i [Hantera användare i Adobe Admin Console](../../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns i [Plattformsbaserade skillnader i administration (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Som Adobe Workfront-administratör kan du skapa en annan Workfront-administratör genom att tilldela dem åtkomstnivån Systemadministratör. En användare med den här åtkomstnivån har fullständig administrativ åtkomst till allt i Workfront, inklusive objekt som de inte skapat själva.

>[!NOTE]
>
>Detta skiljer sig från att använda en åtkomstnivå för att ge användarna administrativ åtkomst till vissa delar av systemet. Mer information finns i följande:
>
>* [Bevilja användare administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)
>* [Åtkomst för en Workfront-administratör jämfört med åtkomst för en avtalsanvändare med administratörsbehörighet](#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights) i den här artikeln
>

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
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Nytt: Standard</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör. </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Ge fullständig systemadministratörsåtkomst till en enskild användare

{{step-1-to-users}}

1. Klicka på namnet på den användare som du vill ge administratörsbehörighet till.
1. Klicka på menyn **Mer** ![](assets/more-icon.png) till höger om användarnamnet och klicka sedan på **Redigera**.

   Rutan **Redigera person** visas.
1. Klicka på **Åtkomst** i den vänstra panelen.
1. Välj åtkomstnivån **Systemadministratör** i listrutan **Åtkomstnivå**.

   Beroende på ändringar som gjorts i systemet kan namnet på den här åtkomstnivån ha ändrats.

1. Klicka på **Spara ändringar.**

   Användaren har nu fullständig behörighet som systemadministratör i systemet.

## Åtkomst för en Workfront-administratör jämfört med åtkomst för en Plan-användare med administratörsbehörighet  {#access-of-a-workfront-administrator-vs-access-of-a-plan-user-with-administrative-rights}

De två tabellerna nedan visar skillnaden mellan en användares åtkomstbehörighet med Workfront-systemadministratörsbehörighet och en användares åtkomstnivå med en avtalslicens med vissa administrativa rättigheter.

Workfront-administratörer kan visa alla objekt i systemet (oavsett vem som skapade dem), skapa nya och ändra eller ta bort befintliga. De har fullständig åtkomst till alla objekt i systemet.

Användare med en planlicens som kan redigera funktionalitet i ett område har full tillgång till funktionaliteten i det området.

>[!NOTE]
>
>Användare med en planlicens som är utsedd till gruppadministratörer kan utföra några av de åtgärder som är tillåtna för Workfront-administratörer. De får endast utföra dessa åtgärder för de grupper de administrerar, deras undergrupper och användarna i dessa grupper och undergrupper. Mer information finns i [Gruppadministratörer](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

* [Åtkomst till inställningsområdet](#access-to-the-setup-area)
* [Åtkomst till objekt](#access-to-objects)

### Åtkomst till inställningsområdet {#access-to-the-setup-area}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Område/objekt</th> 
   <th>Workfront-administratör </th> 
   <th>Användare med en planlicens och vissa administrativa rättigheter</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projektinställningar: Projekt</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>Projektinställningar: Aktiviteter och problem</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>Projektinställningar: Status</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst</p> </td> 
  </tr> 
  <tr> 
   <td>Projektinställningar: Prioriteringar</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>Projektinställningar: Allvarlighetsgrader</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>Projektinställningar: växelkurser</td> 
   <td>Fullständig åtkomst</td> 
   <td>Fullständig åtkomst</td> 
  </tr> 
  <tr> 
   <td>Processer: Godkännanden</td> 
   <td> <p>Fullständig åtkomst</p> </td> 
   <td>Fullständig åtkomst</td> 
  </tr> 
  <tr> 
   <td>Processer: Milstolpebanor</td> 
   <td>Fullständig åtkomst</td> 
   <td>Fullständig åtkomst</td> 
  </tr> 
  <tr> 
   <td>Anpassad Forms</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Hantera egna formulär som de skapat eller anpassade formulär som de delar med sig.</p> <p>Bifoga anpassade formulär som de skapat eller anpassade formulär som de delat med sig till objekt som de har behörighet att hantera eller bidra till.</p> </td> 
  </tr> 
  <tr> 
   <td>Papperskorgen: Nyligen borttaget</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Användare som är gruppadministratörer kan återställa projekt som tilldelats grupper som de hanterar samt uppgifter, ärenden och dokument som är kopplade till dessa projekt.</p> </td> 
  </tr> 
  <tr> 
   <td>Papperskorgen: Nyligen återställt</td> 
   <td>Fullständig åtkomst</td> 
   <td>Användare som är gruppadministratörer kan se de objekt som de nyligen har återställt.</td> 
  </tr> 
  <tr> 
   <td>Jobbroller</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ändra men inte ta bort befintliga jobbroller.</p> <p>Lägg till nya jobbroller.</p> </td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst att skapa team.</p> <p>Lägg till befintliga team till användare när du skapar eller redigerar användare.</p> </td> 
  </tr> 
  <tr> 
   <td>Grupper</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst att skapa grupper.</p> <p>Endast gruppadministratörer kan hantera gruppmedlemskap, undergrupper och gruppnivåstatus för de grupper som de hanterar. </p> </td> 
  </tr> 
  <tr> 
   <td>Företag</td> 
   <td>Fullständig åtkomst</td> 
   <td>Fullständig åtkomst</td> 
  </tr> 
  <tr> 
   <td>Logga in som</td> 
   <td>Fullständig åtkomst </td> 
   <td> <p>Om gruppadministratörsåtkomsten är aktiverad på åtkomstnivån och de har utsetts till gruppadministratör kan de logga in som användare i gruppen de administrerar och deras undergrupper. De kan inte logga in som systemadministratör.<br>Mer information om hur du aktiverar gruppadministrativ åtkomst för användare finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Scheman</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst att redigera scheman.</p> <p>Tillgång att lägga till befintliga scheman för andra användare på användarnivå. </p> </td> 
  </tr> 
  <tr> 
   <td>Tidrapport och timmar: Tidrapportprofiler</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Tillgång till att tilldela befintliga tidrapportprofiler till användare på användarnivå.</p> <p>Användare som är gruppadministratörer kan skapa tidrapportprofiler för de grupper de administrerar och deras undergrupper. </p> </td> 
  </tr> 
  <tr> 
   <td>Tidrapport och timmar: timtyper</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Tillgång till att tilldela timtyper till användare på användarnivå.</p> </td> 
  </tr> 
  <tr> 
   <td>Tidrapport och timmar: Inställningar</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>E-post: Meddelanden: Händelsemeddelanden</td> 
   <td>Aktivera/inaktivera alla</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>E-post: Meddelanden: Påminnelsemeddelanden</td> 
   <td>Fullständig åtkomst</td> 
   <td>Fullständig åtkomst</td> 
  </tr> 
  <tr> 
   <td>E-post: Meddelanden: E-postmallar</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst att redigera e-postmallar.</p> <p>Åtkomst att lägga till befintliga e-postmallar i påminnelsemeddelanden.</p> </td> 
  </tr> 
  <tr> 
   <td>E-post: Automatiska påminnelser</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>E-post: Inbjudningar</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst att redigera e-postinbjudningar.</p> <p>Åtkomst att skicka om e-postinbjudningar till oregistrerade användare endast från fliken Personer.</p> </td> 
  </tr> 
  <tr> 
   <td>E-post: Inställningar</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst</p> </td> 
  </tr> 
  <tr> 
   <td>Styrkort</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Fullständig åtkomst</p> </td> 
  </tr> 
  <tr> 
   <td>Utgiftstyper</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst</p> </td> 
  </tr> 
  <tr> 
   <td>Risktyper</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>Åtkomstnivåer</td> 
   <td> <p>Fullständig åtkomst för att ändra alla åtkomstnivåer.</p> <p>Åtkomstnivåerna för systemadministratörer och externa användare kan inte ändras som standard.</p> </td> 
   <td> <p>Ingen åtkomst att redigera åtkomstnivåer.</p> <p>Tilldela andra användare en åtkomstnivå som är lägre eller lika med deras på användarnivå.</p> </td> 
  </tr> 
  <tr> 
   <td>Gränssnitt: Layoutmallar</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Tillgång till att tilldela befintliga layoutmallar till andra användare på användarnivå. </p> <p>Användare som är utsedda som gruppadministratörer kan skapa layoutmallar för grupper och undergrupper som de hanterar.</p> </td> 
  </tr> 
  <tr> 
   <td>Gränssnitt: Uppdatera feeds</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst att ändra uppdateringsfeeds.</p> <p>Tillgång till att lägga till fält som ska spåras i Uppdatera feeds när du redigerar anpassad Forms.</p> </td> 
  </tr> 
  <tr> 
   <td>Gränssnitt: Filter</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst att skapa filter i området Inställningar.</p> <p>Åtkomst för att skapa nya filter i en lista med objekt.</p> </td> 
  </tr> 
  <tr> 
   <td>Gränssnitt: Vyer</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Det finns ingen åtkomst att skapa vyer under Konfigurera.</p> <p>Åtkomst för att skapa nya vyer i en lista med objekt.</p> </td> 
  </tr> 
  <tr> 
   <td>Gränssnitt: Grupperingar</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst att skapa grupperingar i området Inställningar.</p> <p>Åtkomst för att skapa nya grupperingar i en lista med objekt.</p> </td> 
  </tr> 
  <tr> 
   <td>Gränssnitt: Listkontroller</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst</p> </td> 
  </tr> 
  <tr> 
   <td>Dokument: Molnleverantörer</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst att konfigurera molnleverantörer.</p> <p>Åtkomst till att länka dokument till och från molnleverantörer från fliken Dokument när molnprovidern har integrerats med Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>Dokument: Metadatamappning</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>Dokument: SharePoint Integration</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst för att konfigurera en SharePoint-integrering.</p> <p>Åtkomst till att länka dokument till och från SharePoint från fliken Dokument när SharePoint-integreringen med Workfront har konfigurerats.</p> </td> 
  </tr> 
  <tr> 
   <td>Dokument: Anpassad integrering</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Ingen åtkomst för att konfigurera en anpassad integrering.</p> <p>Åtkomst till att länka dokument till och från tredjepartsleverantörer på fliken Dokument när tredjepartsleverantörerna har integrerats med Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td>System: Varumärkning</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>System: Kundinformation</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>System: enkel inloggning (SSO)</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>System: Uppdatera användare för enkel inloggning</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>System: Quick-Starts</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>System: Diagnostik</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
  <tr> 
   <td>System: Inställningar</td> 
   <td>Fullständig åtkomst</td> 
   <td>Ingen åtkomst</td> 
  </tr> 
 </tbody> 
</table>

### Åtkomst till objekt {#access-to-objects}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Område/objekt</th> 
   <th>Workfront-administratör </th> 
   <th>Användare med en planlicens och vissa administrativa rättigheter</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Kalendrar</td> 
   <td>Fullständig åtkomst</td> 
   <td>Hantera kalendrar som de skapar och kalendrar som delas med dem.</td> 
  </tr> 
  <tr> 
   <td>Kontrollpaneler</td> 
   <td>Fullständig åtkomst</td> 
   <td>Hantera paneler som de skapar och instrumentpaneler som delas med dem.</td> 
  </tr> 
  <tr> 
   <td>Dokument</td> 
   <td>Fullständig åtkomst</td> 
   <td>Hantera dokument som de överför eller dokument som de delar med sig.</td> 
  </tr> 
  <tr> 
   <td>Problem</td> 
   <td>Fullständig åtkomst</td> 
   <td>Hantera problem som de skapar eller problem som delas med dem.</td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>Fullständig åtkomst</td> 
   <td>Hantera portfolior som de skapar eller portfolior som delas med dem. </td> 
  </tr> 
  <tr> 
   <td>Program</td> 
   <td>Fullständig åtkomst</td> 
   <td>Hantera program de skapar eller program som delas med dem.</td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>Fullständig åtkomst</td> 
   <td>Hantera projekt som de skapar eller projekt som delas med dem.</td> 
  </tr> 
  <tr> 
   <td>Rapporter</td> 
   <td>Fullständig åtkomst</td> 
   <td>Hantera rapporter som de skapar eller rapporter som delas med dem. Visa, kopiera och redigera systemrapporter.</td> 
  </tr> 
  <tr> 
   <td>Uppgifter</td> 
   <td>Fullständig åtkomst</td> 
   <td>Hantera uppgifter de skapar eller uppgifter som delas med</td> 
  </tr> 
  <tr> 
   <td>Mallar</td> 
   <td>Fullständig åtkomst</td> 
   <td>Hantera mallar som de skapar eller mallar som delas med dem</td> 
  </tr> 
  <tr> 
   <td>Tidrapporter</td> 
   <td>Fullständig åtkomst</td> 
   <td>Fullständig åtkomst</td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td>Fullständig åtkomst</td> 
   <td> <p>Begränsad åtkomst</p> <p>De kan inte tilldela grupper till användare som de inte är gruppadministratörer för eller grupper som inte är offentliga.</p> <p>De kan inte tilldela användare en åtkomstnivå som är högre än deras egen åtkomstnivå.</p> <p>Om gruppadministratörsåtkomsten är aktiverad på åtkomstnivån och de har utsetts till gruppadministratör för en grupp, kan de återställa lösenordet och logga in som användare i gruppen de administrerar och deras undergrupper. De kan inte återställa lösenordet eller logga in som systemadministratör.<br>Mer information om hur du aktiverar gruppadministrativ åtkomst för användare finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
