---
title: Översikt över AI Assistant
content-type: reference
description: Översikt över AI Assistant
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
source-git-commit: 1517f7480bbe481bc918876441d1b70b09963a97
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Översikt över AI Assistant

>[!IMPORTANT]
>
>Workfront AI Assistant har tagits bort tillfälligt och är tillgänglig vid ett senare tillfälle.

Workfront AI Assistant hjälper dig att slutföra ditt arbete genom att erbjuda information och förslag i appen i en konversation på ett naturligt språk. AI Assistant kan ge dig en smidigare arbetsupplevelse genom att

* Sammanfatta arbetsobjekt eller dokument
* Hitta instruktioner eller referensmaterial för arbetsprocesser
* Generera eller kontrollera formler för beräkningsfält

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Nytt: Alla</p>
       <p>eller</p>
       <p>Aktuell: Inte tillgänglig</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Inte tillgänglig</p></td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).## Förutsättningar för AI-assistenten

Om du vill aktivera AI Assistant för din organisation måste **alla** av följande gälla:

* Din organisation måste ha migrerat till Adobe IMS (Identity Management System)
* Adobe Unified Experience måste aktiveras
* Din organisation måste ha en Select-, Prime- eller Ultimate Workfront-plan
* Adobe måste ha ett signerat Adobe Gen AI-avtal till hands

  Mer information om hur du signerar avtalet finns i [Signera Adobe Gen AI-avtalet](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) i den här artikeln.

## Att tänka på när det gäller AI Assistant

* AI Assistant är sammanhangsberoende för sidan som du har öppen. Om du till exempel anger&quot;Sammanfatta det här projektet&quot; i AI Assistant på en projektsida returneras en sammanfattning av det aktuella projektet.
* Workfront-administratören måste aktivera AI-assistenten för användare i din organisation. AI Assistant aktiveras via åtkomstnivåer.

  Mer information finns i [Aktivera eller inaktivera AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* Workfront Planning AI Assistant har andra funktioner än Workfront AI Assistant.

  Mer information om AI Assistant i Workfront Planning finns i [Översikt över Adobe Workfront Planning AI Assistant](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).


## Funktioner som är tillgängliga i AI Assistant

AI Assistant har för närvarande följande funktioner:

* Sammanfatta projekt, uppgifter, ärenden eller dokument.

  Mer information finns i [Sammanfatta med hjälp av AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Tillhandahåller instruktioner eller referensinformation som hämtas från Workfront dokumentation om Adobe Experience League.

  Mer information finns i [Få hjälp från AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Generera eller förfina formler för beräknade anpassade fält.

  >[!NOTE]
  >
  >Den här funktionen är endast tillgänglig för organisationer som har planer från Prime eller Ultimate Workfront.

  Mer information finns i [Generera eller ändra beräknade fältformler med AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

## Access AI Assistant

1. Klicka på AI Assistant-ikonen ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png) överst på en Workfront-sida.
1. Skriv din fråga eller fråga i panelen till höger på skärmen.

   Om du inte kan skriva på den här panelen har din organisation inget signerat Adobe Gen AI-avtal.

1. Om AI-assistenten inte ger det svar du behöver kan du förfina din fråga och försöka igen.

## Signera Adobe Gen AI-avtalet

Om din organisation inte har ett signerat Adobe Gen AI-avtal kan AI Assistant inte aktiveras för din organisation.

Om en användare försöker använda AI Assistant när Adobe Gen AI-avtalet inte har signerats visas ett meddelande:

* Användare: Användare informeras om att AI Assistant inte har aktiverats för organisationen och att de kan kontakta sin Workfront-administratör för att begära det för sin organisation.
* Administratörer: Administratörer informeras om att det inte finns något signerat Adobe Gen AI-avtal och kan begära att en kopia av avtalet skickas för signering.

Så här begär du AI-avtalet för Adobe Gen:

1. Som Workfront-administratör klickar du på AI Assistant-ikonen ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Börja skriva på AI-assistentpanelen.
1. När Adobe Gen AI-avtalsmeddelandet visas klickar du på **Granska avtal**.
1. Ange namn och e-postadress för den person i organisationen som ska signera avtalet för Adobe Gen AI.

   Avtalet skickas till den här personen för signering. När det har signerats och returnerats aktiveras AI Assistant för din organisation.

