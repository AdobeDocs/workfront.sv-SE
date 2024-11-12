---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Skapa köämnen
description: Köämnen fungerar tillsammans med routningsregler för att automatiskt tilldela inkommande arbete till en användare, en jobbroll, ett team eller för att placera det i ett projekt. Köämnen definierar villkoren som måste finnas för att routningsregeln ska implementeras.
author: Lisa
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: e9d1e35a9c94143a84eb2007985a42f0960a09f7
workflow-type: tm+mt
source-wordcount: '842'
ht-degree: 0%

---

# Skapa köämnen

<!-- Audited: 12/2023 -->

Köämnen fungerar tillsammans med routningsregler för att automatiskt tilldela inkommande arbete till en användare, en jobbroll, ett team eller för att placera det i ett projekt. Köämnen definierar villkoren som måste finnas för att routningsregeln ska implementeras.

Det finns ingen gräns för hur många köämnen som kan tilldelas till en ämnesgrupp eller ett projekt. Köämnen är objekttyper som kan rapporteras.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<!--drafted - replace table with P&P:

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
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
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

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa ett köämne

1. Skapa en routningsregel, en ämnesgrupp och ett anpassat formulär om du tänker associera dem med ditt köämne.\
   Mer information om hur du skapar routningsregler, ämnesgrupper eller anpassade formulär finns i följande artiklar:

   * [Skapa routningsregler](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [Skapa ämnesgrupper](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)

1. Gå till det projekt som du valde att aktivera som en kö för hjälpbegäran och där du vill skapa ett nytt köämne.\
   Mer information om hur du anger ett projekt som en kö för hjälpbegäranden finns i [Skapa en kö för begäranden](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Du kan ordna relaterade köämnen under en ämnesgrupp. Då får den som gjorde begäran en serie listrutor.

   eller

   Du kan kapsla in köämnen direkt under projektet som angetts som en kö för hjälpbegäran, utan någon ämnesgrupp.

   Mer information om hur du skapar ämnesgrupper finns i [Skapa ämnesgrupper](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. Klicka på **Köa ämnen** i den vänstra panelen. Du kan behöva klicka på **Visa fler** och sedan på **Köämnen**.
1. Klicka på **Nytt köämne**.
1. Ange följande i formuläret **Nytt köämne**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Namn</strong> </td> 
      <td> Namn på köämne.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beskrivning</strong> </td> 
      <td>Beskriv begärandekön. Beskrivningen visas när användare väljer ett köämne när en ny begäran skickas. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Lägg till i ämnesgrupp</strong> </td> 
      <td> Om det inte finns några ämnesgrupper i projektet blir projektets namn som ämnesgrupp.<br>Om du vill skapa ytterligare ämnesgrupper härifrån väljer du <strong>Skapa ny ämnesgrupp</strong> i listrutan.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Anpassad Forms</strong> </td> 
      <td>Välj de anpassade formulär som du vill associera med köavsnittet. Du måste skapa anpassade formulär för problem innan du kan koppla dem till köämnen. Mer information om hur du skapar anpassade formulär finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Skapa ett anpassat formulär</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardgodkännande</strong></td> 
      <td> <p>Associera en godkännandeprocess med det här köavsnittet. Endast godkännandeprocesser för problem visas i den här listrutan. Alla utleveranser som skickas till den här kön kommer att associeras med den här godkännandeprocessen. Adobe Workfront-administratören måste definiera godkännandeprocesser på systemnivå innan du kan koppla dem till köämnen. <span>En användare med administrativ åtkomst till godkännandeprocesser kan också skapa gruppspecifika godkännandeprocesser.</span> Mer information om hur du skapar godkännandeprocesser finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Skapa en godkännandeprocess för arbetsobjekt</a>.<br></p> 
       <div> 
        <p>Viktigt: Om projektgruppen ändras blir den gruppspecifika godkännandeprocess som är kopplad till befintliga problem en godkännandeprocess för engångsbruk. Mer information om hur ändringar i projektgruppen eller ändringar i godkännandeprocessen påverkar godkännandeinställningarna finns i <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Hur ändringar i grupp- och godkännandeprocessen påverkar tilldelade godkännandeprocesser</a>.</p> 
        <p>Tänk på följande när du lägger till godkännandeprocesser i köämnen: </p> 
        <ul style="list-style-type: circle;"> 
         <li>Endast aktiva godkännandeprocesser visas i listan. </li> 
         <li> <p>Systemomfattande och gruppspecifika godkännandeprocesser visas i listan. En godkännandeprocess som är associerad med en annan grupp än den som projektet har visas inte i listan.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardvaraktighet</strong> </td> 
      <td>Detta är standardlängden på begäran och det planerade slutförandedatumet för begäran beräknas utifrån det här värdet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardflöde</strong> </td> 
      <td>Ange den routningsregel som du vill koppla till köämnet. Du måste skapa routningsregeln innan du kan koppla den till ett köämne. Mer information finns i <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md">Skapa routningsregler</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Begärantyper</strong> </td> 
      <td> <p>Välj vilken typ av begäranden som lagras i det här köavsnittet. De synliga alternativen anges på fliken <strong>Köinformation</strong> i projektet. Detta är ett obligatoriskt fält. </p>

   <p><b>OBS</b>:

   Typer visas bara som ett urval i området Begäranden om frågetypen har valts både på sidorna Köinformation och på sidorna Köämne. Mer information om hur du konfigurerar området Köinformation för ett projekt finns i <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Skapa en frågekö</a>. </p> <p>Välj bland följande typer:</p>
   <ul>
   <li>Felrapport</li>
   <li>Ändra ordning</li>
   <li>Problem</li>
   <li>Begäran</li>
   </ul> <p>Din Workfront-administratör kan ha bytt namn på några av dessa alternativ. </p> </td>
   </tr> 
    </tbody> 
   </table>

   ![Ny ämnesruta för kö](assets/new-queue-topic-box.png)

1. Klicka på **Spara**.\
   Köämnet är nu tillgängligt att använda och visas i området Begäranden i Workfront när en frågekö och en ämnesgrupp har valts.
