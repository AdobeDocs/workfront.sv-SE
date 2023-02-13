---
product-area: projects
navigation-topic: convert-issues
title: Koppla lösningen av ett problem manuellt till andra problem, uppgifter eller projekt
description: Du kan koppla en problemlösning manuellt till en lösning på ett projekt, en uppgift eller ett problem utan att konvertera problemet. Problemet blir ett av de objekt som kan lösas i projektet, uppgiften eller problemet som du väljer. När du gör detta ändras statusen för projektet, aktiviteten eller utgåvan av statusen för den ursprungliga utgåvan.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 0%

---

# Koppla lösningen av ett problem manuellt till andra problem, uppgifter eller projekt

Du kan koppla en problemlösning manuellt till en lösning på ett projekt, en uppgift eller ett problem utan att konvertera problemet. Problemet blir ett av de objekt som kan lösas i projektet, uppgiften eller problemet som du väljer. När du gör detta ändras statusen för projektet, aktiviteten eller utgåvan av statusen för den ursprungliga utgåvan.

>[!TIP]
>
>När du kopplar en problemlösning till ett annat objekts upplösning kan du inte längre manuellt redigera status för det ursprungliga problemet.

Mer information om att lösa och lösa objekt finns i [Översikt över upplösta och upplösta objekt](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till problem, uppgifter, projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för det problem du länkar till ett annat problem, en annan uppgift eller ett annat projekt</p> <p>Visa eller högre behörigheter för det problem, den uppgift eller det projekt som du lägger till i det befintliga problemet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar måste du:

* Har ett problem vars lösning du vill koppla till en lösning på ett annat problem, en annan uppgift eller ett annat projekt

* Har ytterligare ett problem, en uppgift eller ett projekt

## Bind lösningen av ett problem till en lösning av ett annat problem, en annan uppgift eller ett annat projekt

1. Navigera till ett problem vars lösning du vill koppla till en lösning på ett annat problem eller en uppgift eller ett projekt.
1. Klicka på **Ärendeinformation** > **Översikt** område.

   ![](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Gå till **Översikt** området i **Ärendeinformation** -avsnitt.
1. Klicka på **Löst av** och välj bland följande typer av matchande objekt:  

   * **Projekt**
   * **Uppgift**
   * **Problem**

1. Fältet för det matchande objektet visas.
1. När du har markerat objektet börjar du skriva namnet på ett visst projekt, en viss uppgift eller ett visst fel i det tillgängliga fältet och markerar det när det visas i listrutan.
1. Klicka **Spara** **Ändringar**.\
   Det ursprungliga problemet blir ett löstagbart objekt för det projekt, den uppgift eller det problem som du valde i steg 4 och 5. Detta innebär att det ursprungliga problemet slutförs när det matchande objektet (projektet, aktiviteten eller problemet som du länkade det till) har slutförts.

   >[!NOTE]
   >
   >Ett projekt, en aktivitet eller ett problem kan ha flera problem som upplösbara objekt.

 
