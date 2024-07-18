---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Ge åtkomst till begärandeköer
description: När du ger åtkomst till en begärandekö avgör du vem i organisationen som kan visa begärandekön i området Förfrågningar i Adobe Workfront.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Ge åtkomst till begärandeköer

När du ger åtkomst till en begärandekö avgör du vem i organisationen som kan visa begärandekön i området Förfrågningar i Adobe Workfront.

Du kan ge olika användare åtkomst till en frågekö, beroende på om de är en del av projektteamet, projektgruppen eller projektföretaget. Du kan också ge alla i systemet åtkomst till en frågekö. 

Detta är användbart i organisationer som bjuder in externa intressenter till Workfront och vill begränsa användarnas åtkomst till specifika områden - i det här fallet kan en begärandekö som är öppen enbart för användare som är kopplade till företaget eller projektgruppen begränsa synligheten till externa intressenter. Genom att ge åtkomst till vem som helst blir begäran synlig för både interna och externa intressenter.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p> Hantera behörigheter för projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har

## Förutsättningar

Innan begärandekön är tillgänglig för användare i området Begäranden måste du skapa ett projekt med följande inställningar:

* Ange den som en begärandekö. Mer information om hur du skapar en frågekö finns i [Skapa en frågekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Uppdatera projektets status till Aktuell.

## Ge åtkomst till en frågekö

1. Gå till det projekt där du vill ge åtkomst till begärandeköerna.

   >[!NOTE]
   >
   >Endast projekt med statusen Aktuell visas i området Förfrågningar.

1. Klicka på **Köinformation** i den vänstra panelen. Du kan behöva klicka på **Visa mer** och sedan på **Köinformation**.
1. Välj **Publish som kö för hjälpbegäran** om du vill ange projektet som en frågekö.
1. Välj bland följande alternativ:

   * **Vem som helst**: Alla användare kan visa och lägga till begäranden i begärandekön.
   * **Personer med visningsåtkomst till det här projektet**: Användare som har visningsbehörighet för projektet kan visa och lägga till begäranden i begärandekön. 
   * **Personer i det här projektets företag**: Användare som är associerade med projektets företag kan visa och lägga till begäranden. Det företag som är associerat med projektet står inom parentes bredvid det här alternativet. 
   * **Personer i det här projektets grupp**:Användare som är associerade med projektets grupp kan visa och lägga till begäranden. Gruppen som är associerad med projektet visas inom parentes bredvid det här alternativet.

     Gruppköer är användbara när flera avdelningar delar ett Workfront-konto för att uppnå unika organisationsmål. Varje avdelning kan ha egna köer som medlemmar i andra grupper inte ska kunna se.

     Mer information om vem som har behörighet för ett projekt finns i [Dela ett projekt i Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).\
     Grupper och företag kan associeras med projektet när de redigerar projektet. Mer information om hur du redigerar projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicka på **Spara**.
