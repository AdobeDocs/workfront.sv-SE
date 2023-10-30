---
product-area: projects
navigation-topic: manage-tasks
title: Konvertera en uppgift till ett projekt
description: När en uppgift i ett projekt kräver mer arbete än du ursprungligen planerade, kan du konvertera den till ett projekt.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: b781687b175167784367a2fdec158d97fb3fd6a4
workflow-type: tm+mt
source-wordcount: '1142'
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
   <td> <p>Hantera behörigheter för en uppgift</p> <p>Visa behörigheter för en mall om du konverterar till ett projekt med en mall</p> <p>När du har skapat projektet har du behörigheten Hantera för projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på vid konvertering av uppgifter till projekt

* Du kan konvertera en uppgift till ett tomt projekt eller till ett projekt med hjälp av en mall.
* Den ursprungliga uppgiften tas bort.
* Alla underaktiviteter, utgåvor och anteckningar samlas i det nya projektet.
* Dokument, dokumentversioner och korrektur flyttas till det nya projektet.
* Status och procent färdigt av alla underaktiviteter och utgåvor bevaras.
* Delade användare av uppgiften blir delade användare i projektet.
* Startdatumet för projektet är inställt på startdatumet för aktiviteten.
* I följande tabell visas projektinformation och om den överförs från mallen eller från uppgiften:

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>Beskrivning</td> 
    <td> <p>Beskrivning av uppgiftsöverföringar till det nya projektet. </p> <p> Om det inte finns någon beskrivning av uppgiften överförs beskrivningen från mallen till projektet. </p> <p>Om fältet Beskrivning är tomt både för uppgiften och för mallen är fältet tomt i projektet. </p> </td> 
    </tr> 
    <tr> 
    <td>Status</td> 
    <td> Standardstatus vald för gruppen i mallen. Om mallen inte är associerad med gruppen, ställs projektstatusen in på den standardstatus som anges av Workfront-administratören i området Projektinställningar i installationsprogrammet. Mer information finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md">Konfigurera systemomfattande projektinställningar</a>

  Följande scenarier finns för att uppdatera projektets status:
  <ul>
    <li> Om aktivitetsstatusen är "Nytt" ställs projektstatusen in på "Planering".</li>
    <li> Om aktivitetsstatusen är "Pågår" ställs projektstatusen in på "Aktuell".</li>
    <li> Om aktivitetsstatusen är Slutförd ställs projektstatusen in på Slutförd.</li></ul>

  </td> 
    </tr> 
    <tr> 
    <td>Prioritet</td> 
    <td>Överför från aktiviteten till projektet, eller överför från mallen, om du använder en i konverteringen. </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>URL:en från aktiviteten överförs till det nya projektet. </p> <p> Om ingen URL har angetts för aktiviteten överförs URL:en från mallen till projektet. </p> <p>Om URL-fältet är tomt både för utgåvan och mallen är fältet tomt i projektet. </p> </td> 
    </tr> 
    <tr> 
    <td>Typ av projektvillkor</td> 
    <td>Överför från mallen.</td> 
    </tr> 
    <tr> 
    <td>Projektvillkor</td> 
    <td>Matchar standardinställningen på systemnivå enligt vad som anges av Workfront-administratören i området Inställningar. Mer information finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md">Ange ett anpassat villkor som standard för projekt</a>
    </td> 
    </tr> 
    <tr> 
    <td>Schemalägg från</td> 
    <td>Överför från mallen.</td> 
    </tr> 
    <tr> 
    <td>Projektdatum</td> 
    <td> 
      <ul> 
      <li> <p><b>Planerat startdatum</b>: Den närmaste arbetstiden baserat på mallschemats arbetstid bör vara förmarkerad, enligt tidszonen för mallens schema. Det här fältet är inaktiverat om fältet Schemalägg från är inställt på Från slutförande. </p> </li> 
      <li> <p><b>Planerat slutförandedatum</b>: Den närmaste arbetstiden baserat på mallschemats arbetstid bör vara förmarkerad, enligt tidszonen för mallens schema. Det här fältet är inaktiverat om fältet Schemalägg från är inställt på Från start. </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td>Portfolio</td> 
    <td>Överför från mallen. Annars är fältet tomt.</td> 
    </tr> 
    <tr> 
    <td>Program</td> 
    <td>Överför från mallen. Annars är fältet tomt.</td> 
    </tr> 
    <tr> 
    <td>Grupp</td> 
    <td><p> Följande scenarier finns:</p>
      <ul><li>Om en grupp anges under konverteringen blir det projektgruppen</li>
      <li>Om du konverterar till ett projekt med hjälp av en mall och det finns en grupp i mallen, och du inte anger någon grupp under konverteringen, blir mallgruppen den nya projektets grupp</li>
      <li> Om det inte finns någon grupp i mallen och du inte anger någon grupp under konverteringen, blir gruppen för den ursprungliga utgåvans projekt grupp i det nya projektet</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>Företag</td>    
    <td>  Överför från mallen. Annars är fältet tomt.</td>

  </tr> 
    <tr> 
    <td>Projektägare</td> 
    <td>Överför från fältet Mallägare i mallen. I annat fall anges den inloggade användaren som utför konverteringen. </td> 
    </tr> 
    <tr> 
    <td>Projektsponsorer</td> 
    <td>Överför från fältet Mallsponsor i mallen. Annars är fältet tomt.</td> 
    </tr> 
    <tr> 
    <td>Resurshanteraren</td> 
    <td>Överför från mallen. Annars är fältet tomt.</td> 
    </tr> 
    <tr> 
    <td>Uppgiftsinställningar</td> 
    <td>Överför från mallen.</td> 
    </tr> 
    <tr> 
    <td>Ärendeinställningar</td> 
    <td>Överför från mallen. </td> 
    </tr> 
    <tr> 
    <td>Åtkomst</td> 
    <td> <p>Överför från Access-avsnittet i mallen. </p> </td> 
    </tr> 
    <tr> 
    <td>Godkännanden</td> 
    <td>Överför från mallen. Godkännandena som är kopplade till uppgiften tas bort under konverteringen. </td> 
    </tr> 
  </tbody> 
  </table>


## Konvertera en uppgift till ett projekt

1. Gå till den uppgift som du vill konvertera till ett projekt.
1. Klicka på **Mer** icon ![](assets/more-icon.png)sedan **Konvertera till projekt**.
1. Välj något av följande alternativ:

   * **Nytt projekt**
   * En mall i **Välj från mallar** section

     ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Klicka **Fortsätt** på meddelandet som visas.
1. I **Konvertera till projekt** Ange följande:

   * **Namn**: Namnge projektet. Standardnamnet är namnet på aktiviteten.
   * (Valfritt) **Beskrivning**: Beskriv syftet med projektet.
   * (Valfritt och villkorligt) Om du har valt att skapa ett projekt från en mall uppdaterar du de tillgängliga fälten i **Konvertera till projekt** -dialogrutan.

     Mer information om hur du redigerar fält i projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

     >[!TIP]
     >
     >Om du vill uppdatera fälten i avsnittet Ekonomi i rutan Konvertera till projekt måste du ha Redigera åtkomst till finansiella data på åtkomstnivån. Om du har Visa åtkomst till finansiella data på din åtkomstnivå överförs all ekonomisk information från mallen till det nya projektet och du kan inte redigera den medan du konverterar problemet. Mer information finns i [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) och [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Valfritt) Lägg till **Anpassad Forms** till det nya projektet.

     >[!TIP]
     >
     Om ett anpassat formulär med flera objekt som är kopplat till uppgiften är konfigurerat för användning med både uppgifter och projekt, behålls all information som sparas i formuläret när du konverterar.
     >
     >
     Om du använder en mall för konverteringen och ett anpassat formulär som är kopplat till mallen innehåller ett anpassat fält som också finns i ett anpassat formulär som är kopplat till uppgiften, används fältvärdet från uppgiften för det nya projektet. Om det anpassade fältet är tomt för uppgiften används dock värdet från mallen.

1. Klicka **Spara ändringar**.
