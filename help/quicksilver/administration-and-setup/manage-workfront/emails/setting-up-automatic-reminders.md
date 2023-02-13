---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: Ställ in automatiska påminnelser
description: Ställ in automatiska påminnelser
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 0%

---

# Ställ in automatiska påminnelser

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Som Adobe Workfront-administratör kan du ställa in automatiska påminnelser som utlöser e-postmeddelanden när alla åtgärder eller problem förfaller, förfaller eller ligger nära det planerade slutförandedatumet. När du har konfigurerat de här inställningarna kan användarna inte inaktivera automatiska påminnelser.

För sena meddelanden skickas e-postmeddelandet varje natt tills uppgiften eller utgåvan har slutförts.

En automatisk påminnelse kan skickas till en eller flera av följande:

* Användare som tilldelats en uppgift eller ett problem
* Användarens chef
* Direktörens chef

>[!NOTE]
>
>Du kan inte ändra innehållet eller ämnesraden i e-postmeddelandet som utlöses av en automatisk påminnelse.

## Åtkomstkrav

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Systemadministratör</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ställ in automatiska påminnelser

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **E-post** >**Automatiska påminnelser**.

1. I **Skicka ett sent meddelande till** markerar du något av följande alternativ:

   <table>
    <tr>
        <td>Användaren"Tilldelad till"</td>
        <td>Välj det här alternativet om du vill att användaren som tilldelats en aktivitet eller utgåva ska få ett sent meddelande om att arbetsuppgiften är sen.</td>
        <td></td>
    </tr>
    <tr>
        <td>Användarens chef</td>
        <td>Välj det här alternativet om du vill att användarens chef ska få ett sent meddelande om att den direkta rapportens arbetsuppgift är sen.</td>
        <td></td>
    </tr>
    <tr>
        <td>Chefen</td>
        <td>Välj det här alternativet om du vill att den som ansvarar för den direkta rapporten ska få ett sent meddelande om att en av deras användare är sen med en arbetsuppgift.</td>
        <td></td>
    </tr>
    <tr>
        <td>Användaren"Tilldelad till"</td>
        <td>(I dialogrutan <b>Skicka påminnelse om deadline till</b> område.) Välj det här alternativet om du vill att användaren som tilldelats en uppgift eller en utgåva ska få ett meddelande om att arbetsuppgiften närmar sig förfallodatumet.</td>
        <td></td>
    </tr>
</table>

1. Välj den tidpunkt då den automatiska påminnelsen ska skickas genom att välja hur lång tid som ska gå före eller efter förfallodatumet för arbetsuppgiften.

   Tiden beräknas utifrån det planerade slutförandedatumet för aktiviteten eller utgåvan.

   Ange antalet minuter, timmar, dagar, veckor eller månader som du vill lägga till tid till det planerade slutförandedatumet för aktiviteterna eller problemen. Välj **Förflutna minuter**, **Förflutna timmar**, **Förflutna dagar**, eller **Förflutna veckor** för att lägga till tid som omfattar helger, helger och ej arbetstid enligt ditt schema.

   Om en uppgift till exempel tilldelas på fredag och har en varaktighet på 3 förflutna dagar, är aktivitetens slutförandedatum inställt på måndag (förutsatt att lördag och söndag är en helg). Om aktiviteten har en varaktighet på 3 dagar (inte förfluten), är datumet för aktivitetens slutförande inställt på onsdag.

   ![](assets/time-increments-for-automatic-reminder.png)

1. Klicka **Spara**.

## Få automatiska påminnelser

Om du är angiven enhet i ett meddelande om automatisk påminnelse får du ett e-postmeddelande när den angivna tidsgränsen har uppnåtts. För sena meddelanden skickas e-postmeddelandet varje natt tills uppgiften eller utgåvan har slutförts.

Uppgifter med vissa beroendetyper kan levereras efter det angivna startdatumet, även om de är förfallna. Om en aktivitet till exempel har en föregångare med ett avslutsdatum (fs)-beroende, inkluderas den inte i e-postmeddelandet, även om det har passerat det angivna startdatumet, eftersom du inte kan starta aktiviteten förrän föregående har slutförts.

Mer information om hur du tar emot e-postmeddelanden med automatiska påminnelser finns i [Automatiska påminnelser](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) avsnitt i [Adobe Workfront-meddelanden](../../../workfront-basics/using-notifications/wf-notifications.md).

## Skicka automatiska påminnelser

Automatiska påminnelser skickas så snart den tidpunkt som valts av Workfront-administratören är klar.

Om du vill utlösa att automatiska påminnelser skickas manuellt kan du göra det med Diagnostik. Mer information om hur du använder diagnostik i Workfront finns i [Använd diagnostik för att starta automatiserade processer](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
