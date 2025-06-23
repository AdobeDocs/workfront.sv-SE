---
product-area: requests;user-management
navigation-topic: create-and-manage-request-queues
title: Ge åtkomst till köer för begäranden
description: När du ger åtkomst till en begärandekö avgör du vem i organisationen som kan visa begärandekön i området Förfrågningar i Adobe Workfront.
author: Alina
feature: Work Management
exl-id: eb88c32a-f8b8-42d3-9a3a-72c62fd1dc3a
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Ge åtkomst till begärandeköer

<!-- Audited: 6/2025 -->

När du ger åtkomst till en begärandekö avgör du vem i organisationen som kan visa begärandekön i området Förfrågningar i Adobe Workfront.

Du kan ge olika användare åtkomst till en frågekö beroende på om de är en del av projektteamet, projektgruppen eller projektföretaget. Du kan också ge alla i systemet åtkomst till frågekö.

Detta är användbart i organisationer som bjuder in externa intressenter till Workfront och vill begränsa användarnas tillgång till specifika områden. I det här fallet begränsar en begärandekö som är öppen endast för användare som är associerade med företaget eller gruppen av projektet synligheten till externa intressenter. Genom att ge åtkomst till vem som helst blir begäran synlig för både interna och externa intressenter.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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
   <p>Nytt: Standard </p>
   <p>Aktuell: Planera </p> </td> 
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

## Förutsättningar

Innan begärandekön är tillgänglig för användare i området Begäranden måste du skapa ett projekt med följande inställningar:

* Ange den som en begärandekö. Mer information finns i [Skapa en frågekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
* Uppdatera projektets status till Aktuell.

## Ge åtkomst till en frågekö

1. Gå till det projekt där du vill ge åtkomst till begärandeköerna.

   >[!NOTE]
   >
   >Endast projekt med statusen Aktuell visas i området Förfrågningar.

1. Klicka på **Köinformation** i den vänstra panelen.
1. Välj **Publicera som hjälpbegärandekö** om du vill ange projektet som en begärandekö.
1. Välj bland följande alternativ som visas:

   * **Vem som helst**: Alla användare kan visa och lägga till begäranden i begärandekön.
   * **Personer med visningsåtkomst till det här projektet**: Användare som har visningsbehörighet för projektet kan visa och lägga till begäranden i begärandekön.
   * **Personer i det här projektets företag**: Användare som är associerade med projektets företag kan visa och lägga till begäranden. Det företag som är associerat med projektet står inom parentes bredvid det här alternativet.
   * **Personer i det här projektets grupp**: Användare som är associerade med projektets grupp kan visa och lägga till begäranden. Gruppen som är associerad med projektet visas inom parentes bredvid det här alternativet.

     Gruppköer är användbara när flera avdelningar delar ett Workfront-konto för att uppnå unika organisationsmål. Varje avdelning kan ha egna köer som medlemmar i andra grupper inte ska kunna se.

     Mer information om vem som har behörighet för ett projekt finns i [Dela ett projekt i Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

     Grupper och företag kan associeras med projektet när de redigerar projektet. Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicka på **Spara**.
