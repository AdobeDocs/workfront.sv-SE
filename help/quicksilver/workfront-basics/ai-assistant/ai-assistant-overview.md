---
title: AI Assistant i Workfront
content-type: reference
description: Läs om AI-assistenten i Adobe Workfront
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: e8e10f02f77f6c1df9f0af380eb16cc6bbc3b5d1
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---

# AI Assistant i Workfront

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

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Förutsättningar för AI-assistenten

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

* AI Assistant finns för närvarande bara på engelska.


## Funktioner som är tillgängliga i AI Assistant

AI Assistant har för närvarande följande funktioner:

* Sammanfatta projekt, uppgifter, ärenden eller dokument.

  Mer information finns i [Sammanfatta med hjälp av AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Tillhandahålla instruktioner eller referensinformation som hämtats från Workfront dokumentation om Adobe Experience League.

  Mer information finns i [Få hjälp från AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Hitta specifika objekt i Workfront.

  Mer information finns i [Använd AI-assistenten för att arbeta med projekt, uppgifter och problem](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

* Generera eller förfina formler för beräknade anpassade fält.

  >[!NOTE]
  >
  >Den här funktionen är endast tillgänglig för organisationer som har Prime- eller Ultimate Workfront-planer.

  Mer information finns i [Generera eller ändra beräknade fältformler med AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

* Sammanfatta uppdateringar, överförda dokument och andra betydande ändringar av dina projekt inom följande tidsramar: 24 timmar, 3 dagar, 7 dagar i prioritetsordning.

Mer information finns i [Kom igång med arbetet i Prioriteringar](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).


## Objekttyper tillgängliga för AI Assistant

AI-assistenten kan fråga efter data som är kopplade till följande objekttyper om användaren har de giltiga behörigheterna i Workfront:

* Portföljer
* Program
* Projekt
* Uppgifter
* Problem
* Egna formulär
* Användare
* Workfront Planning - poster


## Få tillgång till AI-assistenten

1. Klicka på AI Assistant-ikonen ![AI Assistant](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png) överst på en Workfront-sida.
1. Skriv din fråga eller fråga i panelen till höger på skärmen.

   Om du inte kan skriva på den här panelen har din organisation inget signerat Adobe Gen AI-avtal.

1. Om AI-assistenten inte ger det svar du behöver kan du förfina din fråga och försöka igen.

## Signera Adobe Gen AI-avtalet

Om din organisation inte har ett signerat Adobe Gen AI-avtal kan AI Assistant inte aktiveras för din organisation.

Om en användare försöker använda AI Assistant när Adobe Gen AI-avtalet inte har signerats visas ett meddelande:

* Användare: Användare informeras om att AI Assistant inte har aktiverats för organisationen och att de kan kontakta sin Workfront-administratör för att begära det för sin organisation.
* Administratörer: Administratörer informeras om att det inte finns något signerat Adobe Gen AI-avtal och kan begära att en kopia av avtalet skickas för signering.

Så här begär du avtalet för Adobe Gen AI:

1. Som Workfront-administratör klickar du på ikonen för AI-assistenten ![AI-assistenten](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png) .
1. Börja skriva på AI-assistentpanelen.
1. När meddelandet Adobe Gen AI-avtal visas klickar du på **Granska avtal**.
1. Ange namn och e-postadress för den person i organisationen som ska signera Adobe Gen AI-avtalet.

   Avtalet skickas till den här personen för signering. När avtalet har signerats och returnerats granskas det av Adobe och sedan aktiveras AI Assistant för din organisation.

   >[!NOTE]
   >
   >Det kan ta 1-3 arbetsdagar innan Adobe har signerat och skickat tillbaka avtalet att granska och aktivera AI Assistant.

## Tips för att skapa uppmaningar i AI Assistant

Använd följande nyckelord i dina uppmaningar för att ge kontext och hjälp med att hitta rätt information. Nyckelord är inte skiftlägeskänsliga.

Inkludera frasen `using (keyword)` när du anger din fråga.

| Nyckelord | Effekt |
| --- | --- | 
| `workfront` | Interagera med Workfront. |
| `planning` | Interagerar med Workfront Planning. |
| `help` | Returnerar information från Experience League-dokumentation. |
| `formula` | Kontrollerar och returnerar formler för användning i Planning, Setup eller anpassade formulär. |
| `health` | Kontrollerar projektets hälsa med Project Health Advisor. |
| `summarize` | Sammanfattar objekt, t.ex. när du överför en fil eller sammanfattar ett projekt. |

>[!NOTE]
>
> Alla nyckelord är inte tillgängliga i alla områden.
>
>* Nyckelordet `formula` är bara tillgängligt i Planning, Setup och Custom Form Builder.
>* Nyckelordet `planning` är bara tillgängligt från Workfront Planning.





