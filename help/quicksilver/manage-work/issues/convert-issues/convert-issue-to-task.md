---
product-area: projects
navigation-topic: convert-issues
title: Konvertera ett ärende till en uppgift
description: Om du måste göra mer för att slutföra ett problem efter att utgåvan har skickats kan du konvertera det till en uppgift i Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 9d8e50ab-9fed-4ded-83e1-29dc92c37171
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1004'
ht-degree: 0%

---

# Konvertera ett problem till en uppgift

<!--Audited: 08/2025-->

Om du måste göra mer för att slutföra ett problem efter att utgåvan har skickats kan du konvertera det till en uppgift i Adobe Workfront.

Allmän information om hur du konverterar problem finns i [Översikt över hur du konverterar problem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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
   <td> <p>Standard</p>
   <p>Arbeta eller högre</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem, uppgifter och projekt</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter för utgåvan</p> <p>Contribute-behörigheter till projektet</p> <p>Du får behörigheten Hantera för uppgiften när problemet har konverterats</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues, Tasks, and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the issue</p> <p>Contribute permissions to the project</p> <p>You obtain&nbsp;Manage permissions to the task after the issue is converted</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table> -->

## Överväganden

* Bearbetningsgränsen är fem minuter vid konvertering av ett problem till en uppgift. Om ett stort antal dokument har bifogats och inte kan konverteras kan du behöva ta bort några av dokumenten och försöka igen.

## Konvertera ett problem till en uppgift

1. Gå till ett projekt och klicka på [!UICONTROL **Problem**] i den vänstra panelen.
1. Klicka på det problem du vill konvertera för att gå till problemets startsida.
1. Klicka på menyn [!UICONTROL **Mer**] i problemet och sedan på [!UICONTROL **Konvertera till aktivitet**].

   ![Menyn Mer om problem](assets/qs-issue-more-menu-highlighted-350x469.png)

   >[!TIP]
   >
   >Om problemet är kopplat till en godkännandeprocess eller om det redan är kopplat till ett matchande objekt, visar Workfront en varning högst upp i rutan [!UICONTROL Convert to Project] för att meddela dig att godkännandet har tagits bort eller att det matchande objektet skrivs över under konverteringen. Mer information finns i [Översikt över konvertering av problem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. Uppdatera aktivitetsnamnet i avsnittet [!UICONTROL Task Name]. Som standard får aktiviteten samma namn som den ursprungliga utgåvan.

   ![Konvertera till aktivitetsruta](assets/convert-to-task-box-nwe.png)

1. Klicka på [!UICONTROL **Målprojekt**] och börja sedan skriva namnet på projektet där du vill placera den nya aktiviteten i fältet [!UICONTROL **Målprojekt**] och markera den när den visas i listan. Utgåvans projekt är valt som standard.

1. Klicka på [!UICONTROL **Översikt**] och skriv sedan en [!UICONTROL **Beskrivning**] för uppgiften.

   >[!TIP]
   >
   >   En system- eller gruppadministratör kan ändra ordningen på avsnitten i den vänstra panelen i konverteringsrutan genom att ändra layoutmallen.

1. (Valfritt och villkorligt) Klicka på [!UICONTROL **Alternativ**] och välj något av alternativen nedan.

   Workfront-administratören eller gruppadministratören måste aktivera de här inställningarna innan de visas vid konverteringen av problem:

   * [!UICONTROL **Behåll det ursprungliga problemet och koppla dess lösning till den här uppgiften**]

     Om du inte markerar det här alternativet tas den ursprungliga utgåvan bort.

     >[!NOTE]
     >
     >Användare som saknar åtkomst eller behörighet att ta bort problem kan inte ta bort problemet eftersom de konverterar det, oavsett status för den här inställningen. Mer information om åtkomst och behörigheter till problem finns i:
     >   
     >   * [Bevilja åtkomst till utgåvor](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     >   * [Dela ett problem](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)
     >   
     >

   * [!UICONTROL **Tillåt (användarnamn) åtkomst till den här aktiviteten**]

     Om du inte markerar det här alternativet har problemets primära kontakt ingen åtkomst till den nya aktiviteten.

   * [!UICONTROL **Behåll planerat slutdatum för problemet**]

     Om alternativet inte är markerat beräknas [!UICONTROL Planned Completion Date] för den nya aktiviteten från [!UICONTROL Planned Start Date] för aktiviteten. [!UICONTROL Planned Start Date] för den nya aktiviteten anges enligt systeminställningarna för nya uppgifter.

     >[!NOTE]
     >
     >
     >Vilka alternativ som visas här beror på hur Workfront-administratören konfigurerade dem för alla i systemet. Mer information finns i [Konfigurera inställningar för aktiviteter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >Eller, om de översta grupperna i din organisation konfigurerade dem separat, beror alternativen som visas här på vilken grupp som är associerad med projektet som du valde i steg 6. Mer information finns i [Konfigurera aktivitets- och probleminställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. (Valfritt) Klicka på [!UICONTROL **Anpassad Forms**] och bifoga ett anpassat formulär för den nya aktiviteten.

   >[!TIP]
   >
   >* Om ett anpassat formulär med flera objekt som är kopplat till utgåvan är konfigurerat för användning med både utgåvor och uppgifter, behålls all information som sparas i formuläret när du gör konverteringen om fälten finns både i utgåvan och i uppgiftens anpassade formulär.
   >* Om ett anpassat formulär med flera objekt och ett beräknat fält bifogas till utgåvan och till uppgiften, måste utgåvan och uppgiften vara kompatibla med alla fält som refereras i formulärets beräknade anpassade fält. Om det finns inkompatibilitet visas ett meddelande som varnar dig om att göra ändringar. Mer information finns i [Lägga till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
   >* Om målprojektet har några standardformulär definierade i fältet Standardinställd Forms för uppgifter när projektet redigeras, läggs även dessa uppgiftsformulär till i den nya uppgiften. Alla anpassade fält som är gemensamma mellan den ursprungliga utgåvan och fälten i standardaktivitetsformulären är förifyllda med information från utgivningsfälten.


1. Klicka på [!UICONTROL **Konvertera till uppgift**].

   Problemet är nu en uppgift i det angivna projektet om du bestämde dig för att ta bort den ursprungliga utgåvan.

   eller

   Problemet är nu länkat till den nya uppgiften i det projekt du valde, och det slutförs när uppgiften är klar, om du bestämde dig för att behålla det ursprungliga problemet.

   Vissa problemfält överförs till uppgiften. Mer information finns i avsnittet [Visa ursprunglig probleminformation om projekt och uppgifter](#view-original-issue-information-on-projects-and-tasks) i den här artikeln.

1. (Valfritt) Fortsätt redigera uppgiften efter behov.

## Visa ursprunglig probleminformation om projekt och uppgifter {#view-original-issue-information-on-projects-and-tasks}

Du kan visa den ursprungliga utgivningsinformationen i projekt- och uppgiftslistor och rapporter eller i området Projektinformation. Mer information om hur du skapar rapporter finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Tabellen nedan visar vilka problemfält som visas i de konverterade projekten och uppgifterna.

| Ärendefält | Projekt eller aktivitetsfält | Projektlista eller rapport | Området Projektinformation | Uppgiftslista eller rapport | Området Uppgiftsinformation |
|---|---|---|---|---|---|
| [!UICONTROL Issue Name] | [!UICONTROL Converted Issue Name] | ✔ | ✔ | ✔ | ✔ |
| [!UICONTROL Primary Contact] | [!UICONTROL Converted Issue Originator Name] | ✔ | ✔ | ✔ |
| [!UICONTROL Entry Date] | [!UICONTROL Converted Issue Entry Date] | ✔ |  | ✔ |


>[!CAUTION]
>
>Om [!UICONTROL Primary Contact] för ett problem ändras eller om problemet inte längre är länkat från projektet eller aktiviteten efter att problemet har konverterats, uppdateras inte [!UICONTROL Converted Issue Originator Name]och den ursprungliga [!UICONTROL Primary Contact] för problemet visas när problemet konverterades.
