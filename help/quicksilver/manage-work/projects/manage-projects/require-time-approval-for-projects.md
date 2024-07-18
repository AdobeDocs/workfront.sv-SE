---
product-area: projects
navigation-topic: manage-projects
title: Kräv tid för godkännande av ett projekt
description: Kräv tid för godkännande av ett projekt
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Kräv tid för godkännande av ett projekt

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

Du kan konfigurera projektet så att det kräver att de timmar som loggas mot projektet godkänns av projektägaren. När timmarna är konfigurerade på det här sättet måste de först godkännas av projektägaren innan de kan användas i en faktureringspost.\
Mer information om faktureringsposter finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>Om du aktiverar det här alternativet tas inte tidrapportgodkännarens möjlighet att godkänna tiden bort från tidrapporten. Om projektägaren inte godkänner eller avvisar tid kan en tidrapportgodkännare fortfarande godkänna tiden på en tidrapport.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Planera att kräva tid för godkännande av projektet</p>
   <p>Granska eller senare för att godkänna timmar som är inloggade på ett projekt</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt eller högre</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter till projektet eller högre</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
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
     <li>Du har en planlicens med administrativ åtkomst till tidrapporter och timmar. I detta fall:
      <ul>
       <li>Du kan godkänna eller avvisa alla timmar i de projekt som du har minst behörighet att visa. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Kräv tid för godkännande av ett projekt

Så här kräver du projektledarens godkännande för timmar i projektet:

1. Gå till projektet där du vill ha godkännande i timmar.
1. Klicka på ikonen **Mer** ![](assets/more-icon.png) till höger om projektnamnet och klicka sedan på **Redigera**.\
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
1. Klicka på området **Timmar** i den vänstra panelen. Detta kan finnas under området **Visa mer**.

1. Timmar som loggats för problem, uppgifter och projektvisning och som ska ha statusen **Skickat**.\
   Klicka i rutan till vänster om timuppgifterna för att välja de timmar som du vill godkänna.

1. Klicka på **Godkänn**.\
   Status för timmarna ändras till **Godkänd**.\
   Om du senare avvisar de godkända timmarna ändras statusen för timmarna till **Inte godkänt**.\
   När du inkluderar de godkända timmarna i en faktureringspost ändras statusen för timmarna till **Fakturerad och godkänd**. Timmar som lagts till i en faktureringspost kan inte tas bort. Mer information om hur du skapar faktureringsposter finns i artikeln [Skapa faktureringsposter](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Valfritt) Klicka på **Avvisa** om du vill avvisa tidsposterna i projektet.\
   Status för timmarna ändras till **Avvisad**.
