---
product-area: projects
navigation-topic: manage-projects
title: Kräv tid för godkännande av ett projekt
description: Du kan konfigurera projektet så att det kräver att de timmar som loggas mot projektet godkänns av projektägaren. När timmarna är konfigurerade på det här sättet måste de först godkännas av projektägaren innan de kan användas i en faktureringspost.
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 0%

---

# Kräv tid för godkännande av ett projekt

<!--audited: 08/2024-->

Du kan konfigurera projektet så att det kräver att de timmar som loggas mot projektet godkänns av projektägaren. När timmarna är konfigurerade på det här sättet måste de först godkännas av projektägaren innan de kan användas i en faktureringspost.\
Mer information om faktureringsposter finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>Om du aktiverar det här alternativet tas inte tidrapportgodkännarens möjlighet att godkänna tiden bort från tidrapporten. Om projektägaren inte godkänner eller avvisar tid kan en tidrapportgodkännare fortfarande godkänna tiden på en tidrapport.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Så här kräver du tid för att godkänna projektet:</p>
   <ul><li><p>Standard</p></li>
   <li><p>Plan</p></li></ul>

<p>Så här godkänner du timmar som är inloggade i ett projekt:</p>
   <ul><li><p>Ljus eller högre</p></li>
   <li><p>Granska eller högre</p></li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter till projektet eller högre</p>
  </tr> 
  <tr> 
   <td role="rowheader">Ytterligare åtkomst</td> 
   <td> <p>Du måste uppfylla minst ett av följande villkor för att godkänna tiden för ett projekt:</p> 
    <ul> 
     <li>Du är projektägare med den åtkomst och de behörigheter som anges ovan. I det här fallet kan du göra följande om något av villkoren nedan finns: 
      <ul>
       <li>Om du har behörigheten Hantera i projektet kan du godkänna eller avvisa timmar som har loggats in i projektet av någon annan användare.</li>
       <li> Om du har Contribute- eller Visa-åtkomst till projektet kan du bara godkänna eller avvisa de timmar som loggats av dig eller någon annan användare som rapporterar dig.<br></li>
      </ul></li> 
     <li>Du har en planlicens med administrativ åtkomst till tidrapporter och timmar. I detta fall:
      <ul>
       <li>Du kan godkänna eller avvisa alla timmar i de projekt som du har minst behörighet att visa. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>To require time to be approved on the project:</p>
   <ul><li>New: Standard</li>
   <li>Current: Plan</li></ul>
   
   <p>To approve hours logged on a project:</p>
   <ul><li>New: Light or higher</li>
   <li>Review or higher</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects or higher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher</p>
  </tr> 
  <tr> 
   <td role="rowheader">Additional access</td> 
   <td> <p>You must meet at least one of the following conditions to approve time on a project:</p> 
    <ul> 
     <li>You are the Project Owner with the access and permissions specified above. In this case, you can do the following if one of the conditions below exists: 
      <ul>
       <li>If you have Manage permissions on the project, you can approve or reject hours logged on the project by any other user.</li>
       <li> If you have Contribute or View access to the project you will be able to approve or reject only the hours logged by you or any other user that reports you.<br></li>
      </ul></li> 
     <li>You have a Plan license with administrative access to Timesheets &amp; Hours. In this case:
      <ul>
       <li>You can approve or reject any hours on the projects you have at least permissions to View. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>-->

## Kräv tid för godkännande av ett projekt

Så här kräver du projektledarens godkännande för timmar i projektet:

1. Gå till projektet där du vill ha godkännande i timmar.
1. Klicka på ikonen **Mer** ![Mer ](assets/more-icon.png) till höger om projektnamnet och klicka sedan på **Redigera**.\
   Dialogrutan Redigera projekt visas.

1. I avsnittet **Projektinställningar** väljer du **Kräv tid för att godkännas för det här projektet**.
1. Klicka på **Spara**.\
   När tiden loggas och godkänns blir dessa timmar låsta och kan inte ändras av användaren som angav dem i projektet eller tidrapporten. Endast en Workfront-administratör kan justera den registrerade tiden.

## Godkänn och avvisa tid i ett projekt

Som projektledare kan du godkänna eller avvisa timmar som är loggade för uppgifter, ärenden eller projektet.

Att godkänna timmarna på projektnivå påverkar inte tidrapporten för någon av de användare som loggade timmarna. Timmarna i projektet kanske till exempel godkänns av projektledaren, men tidrapporten har ännu inte godkänts av användarens eller tidrapportens godkännare.

Om du ställer in ett projekt för att kräva godkännande på de loggade timmarna måste projektledaren godkänna timmarna för att de ska vara tillgängliga för att inkluderas i en faktureringspost för projektet. Mer information om hur du skapar faktureringsposter finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md).

Så här godkänner eller avvisar du timmar i ett projekt:

1. Gå till projektet.
1. Klicka på området **Timmar** i den vänstra panelen.

1. Timmar som loggats för problem, uppgifter och projektvisning och som ska ha statusen **Skickat**.\
   Klicka i rutan till vänster om timuppgifterna för att välja de timmar som du vill godkänna.

1. Klicka på ikonen **Godkänn** ![Godkänn](assets/approve-hours-icon.png) längst upp i timlistan.\
   Status för timmarna ändras till **Godkänd**.\
   Om du senare avvisar de godkända timmarna ändras statusen för timmarna till **Inte godkänt**.\
   När du inkluderar de godkända timmarna i en faktureringspost ändras statusen för timmarna till **Fakturerad och godkänd**. Timmar som lagts till i en faktureringspost kan inte tas bort. Mer information om hur du skapar faktureringsposter finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Valfritt) Klicka på ikonen **Avvisa** ![Ikonen Avvisa timmar](assets/reject-hours-icon.png) om du vill avvisa tidsposterna i projektet.\
   Status för timmarna ändras till **Avvisad**.

   >[!NOTE]
   >
   >   Om de valda timmarna ingår i en faktureringspost som har markerats som Fakturerad eller Fakturerad och godkänd visas inte ikonerna Godkänn och Avvisa. Du kan bara godkänna timmar som inte redan har fakturerats i en faktureringspost.

