---
title: Skapa ett team från inställningsområdet
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: Som Adobe Workfront-administratör kan du skapa ett team under Konfigurera.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

# Skapa ett team från inställningsområdet

Som Adobe Workfront-administratör kan du skapa ett team under Konfigurera. Mer information om team finns i [Teams overview](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* En gruppadministratör kan skapa ett team för en grupp som de administrerar under Konfigurera. Mer information finns i [Skapa och ändra en grupps team](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* En användare med en Standard- eller Plan-licens kan också skapa ett team från Teams-området. Mer information finns i [Skapa ett team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa ett team

{{step-1-to-setup}}

1. Klicka på **Team** och sedan på **Nytt team**.

1. Ange följande information i rutan **Nytt team** som visas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Teamnamn</td> 
      <td>Skriv ett namn för teamet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Grupp</td> 
      <td> <p>Om du vill associera gruppen med en grupp börjar du skriva namnet på gruppen och väljer sedan namnet när den visas.</p> <p>Du kan kontrollera att du associerar rätt grupp med gruppen genom att hålla markören över den och klicka på informationsikonen <img src="assets/info-icon.png"> som visas bredvid den. Här visas ett verktygstips med information om gruppen, till exempel hierarkin för grupper ovanför och dess administratörer.</p> <p><b>Obs!</b> När ett team tilldelas en grupp eller undergrupp kan alla gruppadministratörer i den gruppen eller undergruppen hantera teamet utan att vara medlem i gruppen. Gruppadministratörer kan gå till Teams-området från huvudmenyn och klicka på pilen Byt team <img src="assets/switch-team-icon.png" alt="Byt ikon för team"> för att lista alla team som är tilldelade de grupper som de hanterar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Teammedlemmar</td> 
      <td> <p>Börja skriva namnet på en användare som ska vara med i teamet och markera sedan namnet när det visas i listrutan. Upprepa den här processen om du vill lägga till flera användare i teamet.</p> <p>Det finns ingen gräns för hur många användare du kan lägga till i ett team. Vi rekommenderar dock att du inte har ett alltför stort antal användare i ett team eftersom teamets hantering kan bli alltför komplex.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Skriv en beskrivning för teamet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kalender</td> 
      <td>Välj vilken kalenderflik som ska visas för teamet.</td> 
     </tr> 
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">Det här är ett Agile Team</td> 
      <td>Välj det här objektet om du vill konfigurera det nya teamet som ett Agile-team. Mer information om Agile-team finns i <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Skapa ett Agile-team</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeta på den</td> 
      <td>Ändra knappen Arbeta på den till en Start-knapp. När en användare klickar på Start uppdateras objektets status automatiskt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Knappen Klar</td> 
      <td>Välj den status som du vill ange för objekt när du klickar på knappen Klar.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Skapa team**.

## Teamägare

När du skapar ett team blir du som standard teamets ägare.

Du kan visa teamägare för alla team när du skapar en rapport för team och inkludera fältet Ägarnamn i rapporten. (Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
