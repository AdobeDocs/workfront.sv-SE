---
product-area: projects
navigation-topic: manage-tasks
title: Konvertera en uppgift till ett projekt
description: När en uppgift i ett projekt kräver mer arbete än du ursprungligen planerade, kan du konvertera den till ett projekt.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Konvertera en uppgift till ett projekt

När en uppgift i ett projekt kräver mer arbete än du ursprungligen planerade, kan du konvertera den till ett projekt.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p>Visa eller ge senare åtkomst till mallar, vid konvertering till ett projekt med hjälp av en mall</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för en uppgift</p> <p>Visa behörigheter för en mall om du konverterar till ett projekt med hjälp av en mall</p> <p>När du har skapat projektet har du behörigheten Hantera för projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på vid konvertering av uppgifter till projekt

* Den ursprungliga uppgiften tas bort.
* Uppgiftsgodkännanden tas bort.
* Alla underaktiviteter, utgåvor och anteckningar samlas i det nya projektet.
* Dokument, dokumentversioner och korrektur flyttas till det nya projektet.
* Status och procent färdigt av alla underaktiviteter och utgåvor bevaras.
* Delade användare av uppgiften blir delade användare i projektet.
* Startdatumet för projektet är inställt på startdatumet för aktiviteten.
* Om aktivitetsstatusen är &quot;Nytt&quot; ställs projektstatusen in på &quot;Planering&quot;.
* Om aktivitetsstatusen är &quot;Pågår&quot; ställs projektstatusen in på &quot;Aktuell&quot;.
* Om aktivitetsstatusen är Slutförd ställs projektstatusen in på Slutförd.

## Konvertera en uppgift till ett projekt

1. Gå till den uppgift som du vill konvertera till ett projekt.
1. Klicka på **Mer** icon ![](assets/more-icon.png)sedan **Konvertera till projekt**.
1. Välj något av följande alternativ:

   * **Nytt projekt**
   * En mall i **Välj från mallar** section

      ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Klicka **Fortsätt** på meddelandet som visas.
1. I **Konvertera till projekt** Ange följande:

   * **Namn**: Ge projektet ett namn. Standardnamnet är namnet på aktiviteten.
   * (Valfritt) **Beskrivning**: Beskriv syftet med det här projektet.
   * (Valfritt och villkorligt) Om du har valt att skapa ett projekt från en mall uppdaterar du de tillgängliga fälten i **Konvertera till projekt** -dialogrutan.

      Mer information om hur du redigerar fält i projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >Om du vill uppdatera fälten i avsnittet Ekonomi i rutan Konvertera till projekt måste du ha Redigera åtkomst till finansiella data på åtkomstnivån. Om du har Visa åtkomst till finansiella data på din åtkomstnivå överförs all ekonomisk information från mallen till det nya projektet och du kan inte redigera den medan du konverterar problemet. Mer information finns i [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) och [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Valfritt) Lägg till **Anpassad Forms** till det nya projektet.

      >[!TIP]
      Om ett anpassat formulär med flera objekt som är kopplat till uppgiften är konfigurerat för användning med både uppgifter och projekt, behålls all information som sparas i formuläret när du konverterar.
      Om du använder en mall för konverteringen och ett anpassat formulär som är kopplat till mallen innehåller ett anpassat fält som också finns i ett anpassat formulär som är kopplat till uppgiften, används fältvärdet från uppgiften för det nya projektet. Om det anpassade fältet är tomt för uppgiften används dock värdet från mallen.

1. Klicka **Spara ändringar**.
