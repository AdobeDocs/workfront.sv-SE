---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Skapa routningsregler
description: Routningsregler styr vad Adobe Workfront gör med problem när de skickas till en frågekö. Mer information om hur du skapar begärandeköer finns i Skapa en begärandekö.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Skapa routningsregler

<!-- Audited: 12/2023 -->

Routningsreglerna styr vad Adobe Workfront gör med problem när de skickas till en begärandekö. Mer information om hur du skapar frågeköer finns i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Routningsregler skickar problem till specifika användare eller jobbroller som är bäst utrustade för att lösa det skickade problemet eller den skickade förfrågan. Routningsregler är vanligtvis associerade med köämnen, som används för att kontrollera vilken routningsregel som ska användas för utgåvan eller förfrågan.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<!--drafted - replace the table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
    <p>Nytt: Standard</p>
    <p>eller</p>
    <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p> Hantera behörigheter för projektet</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en hanteringsregel

1. Gå till det projekt där du vill lägga till routningsreglerna för dina begäranden.
1. Klicka **Routningsregler** till vänster. Du kan behöva klicka **Visa fler** sedan **Routningsregler**.
1. Klicka **Ny hanteringsregel** för att lägga till den nya regeln.
1. Ange följande information för hanteringsregeln:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Namn</strong> </td> 
      <td>Namnet på routningsregeln. Du kan se routningsregeln om du har tillgång till den här informationen i projektet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beskrivning</strong> </td> 
      <td>Lägg till en beskrivning för routningsregeln.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardtilldelning*</strong> </td> 
      <td>Lägg till en aktiv användare eller en aktiv jobbroll som de nya utgåvorna ska tilldelas till. Du kan bara ha en standardtilldelare i det här fältet. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardteam*</strong> </td> 
      <td>Lägg till ett aktivt team som den nya utgåvan ska tilldelas till. Du kan bara ha ett standardteam i det här fältet.

   <p><b>ANMÄRKNING</b></p>

   När utgåvan har skickats in kan du redigera uppdragen och tilldela andra användare, roller eller team. Mer information finns i  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Tilldela ärenden</a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Flöde till projekt</strong> </td> 
      <td>Det här är projektet där problemet läggs till.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*Om en användare, en jobbroll eller ett team inaktiveras efter att de har associerats med en routningsregel dirigeras förfrågningarna vidare till dem. Du måste regelbundet inventera alla routningsregler och ersätta inaktiverade tilldelningar med aktiva.

   När du dirigerar ett problem till ett projekt får användare med behörigheter för det aktuella projektet de behörigheter som angetts för det projektet. Mer information om hur du ställer in behörigheter för projekt finns i [Dela ett projekt i Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![Ny ruta för hanteringsregel](assets/new-routing-rule-box.png)

1. Klicka **Spara**.

   Den här processen definierar bara routningsregeln. Du måste välja routningsregeln på **Köinformation** flik under **Standardflöde**.

   Mer information om hur du lägger till en standardflöde i en begärandekö finns i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Om du vill associera flera routningsregler med begärandekön måste du skapa flera köämnen och associera vart och ett med en separat routningsregel. Mer information om hur du skapar ett köämne finns i [Skapa köämnen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
