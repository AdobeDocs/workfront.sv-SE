---
product-area: projects
navigation-topic: use-the-home-area
title: Visa objekt i [!UICONTROL Worklist] i hemområdet
description: Varje widget innehåller en egen arbetslista. Arbetslister visar alla arbetsobjekt som är tilldelade dig. Du kan styra vilka objekt som ska visas i [!UICONTROL worklist] genom att använda filter och grupperingar.
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: 41f58261d4f2e6075187886b371a23eb5e97d823
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# Visa objekt i [!UICONTROL worklist] i området [!UICONTROL Home]

<!-- Audited: 1/2024 -->

Varje widget innehåller en egen arbetslista. Arbetslister visar alla arbetsobjekt som är tilldelade dig. Du kan styra vilka objekt som ska visas i [!UICONTROL worklist] genom att använda filter och grupperingar.

>[!IMPORTANT]
>
>* Om du vill visa uppgifter och problem i Home-widgetarna måste det överordnade projektet ha statusen Aktuell eller en status som motsvarar aktuell.
>* Projekt måste också ha statusen Aktuell eller en status som är lika med aktuell att visa i Hem.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens</strong></td> 
   <td><ul><li>[!UICONTROL Contributor] endast för godkännanden</li> <li>[!UICONTROL Standard] eller högre för alla andra objekt</li> <p>eller</p> 
  </ul><ul><li>[!UICONTROL Review] endast för godkännanden</li> <li>[!UICONTROL Work] eller högre för alla andra objekt</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>[!UICONTROL View] eller högre tillgång till projekt, uppgifter, ärenden och dokument</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Contribute-behörigheter eller högre för de uppgifter och problem som du behöver arbeta med</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Krav för arbetsuppgifter som ska visas i arbetslistan

Det finns inbyggda krav för vilka arbetsobjekt visas i en viss widgetarbetslista. Arbetsobjekten måste uppfylla dessa krav för att kunna visas i arbetslistorna för följande widget.

### Widgeten Mina uppgifter

Aktiviteter måste uppfylla följande krav för att kunna visas i widgeten Mina uppgifter:

* Aktivitetsstatusen är inte lika med Fullständig.
* Den inloggade användaren måste tilldelas uppgiften.
* Aktivitetsstatusen är inte lika med Klar.
* Det projekt som aktiviteten tillhör måste ha en status som motsvarar aktuell.


### Widgeten Mina problem

Problem måste uppfylla följande krav för att visas i widgeten Mina problem:

* Den inloggade användaren måste tilldelas utgåvan.
* Utfärdandestatusen är inte lika med Fullständig.
* Det finns inget olöst objekt kopplat till problemet.
* Utgivningsstatusen är inte lika med Klar.
* Det projekt som utgåvan tillhör måste ha en status som motsvarar aktuell.

### Min teamwidget

Team-förfrågningar måste uppfylla följande krav för att visas i My Teams-widgeten:

* Den inloggade användaren tillhör det team som arbetsuppgiften är tilldelad.
* Arbetsuppgiftens status är inte lika med Fullständig.
* Arbetsuppgiften har ingen bifogad godkännandeprocess.
* Arbetsuppgiften är inte en återkommande uppgift.
* Det projekt som arbetsuppgiften tillhör måste ha en status som motsvarar aktuell.

## Filtrera ditt arbete

Du kan filtrera objekt i [!UICONTROL Worklist] för en widget så att endast vissa typer av objekt visas. Du kan t.ex. filtrera arbetsytan [!UICONTROL Worklist] så att endast problem eller förfrågningar visas.

>[!NOTE]
>
>Filteralternativen lagras i webbläsaren. Om du använder samma webbläsare på samma dator (och inte rensar platsdata) på samma sätt, ska du inte ändra det. Om du byter webbläsare eller dator återställs standardalternativet, vilket innebär att alla filter är avmarkerade.

Så här filtrerar du ditt arbete:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Klicka på **Anpassa** om du vill lägga till någon av följande widgetar:

   | Widget | Beskrivning |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Varumärkena | Visar alla anslagstavlor som du har skapat eller har bjudits in att använda |
   | Mitt arbete | Visar uppgifter och ärenden som du har tilldelats |
   | Mina projekt | Visar projekt som du äger eller projekt som du arbetar med |
   | Mina uppgifter | Visar uppgifter som tilldelats dig |
   | Mina problem | Visar problem som du har tilldelats |
   | Mina förfrågningar | Visar alla begäranden som du har skickat in |
   | Mina godkännanden | Visar alla väntande, tilldelade, delegerade och inskickade godkännanden |

1. Klicka på ikonen **Filter** ![Filtrera &#x200B;](assets/filter-nwepng.png) i det övre högra hörnet av widgetens arbetslista.
1. Välj ett **föreslaget**-filter eller ett filter som du har skapat.
Mer information om föreslagna filter finns i [Översikt över filter för hemwidget](/help/quicksilver/workfront-basics/using-home/using-the-home-area/widget-filter-overview-home.md).
1. (Valfritt) Aktivera **Staplingsfilter** om du vill välja flera filteralternativ.

   ![Filtret Min aktivitet är öppet](assets/my-task-filter-open.png)


## Gruppera ditt arbete

Du kan gruppera widgeten [!UICONTROL worklist] för att ordna dina arbetsobjekt.

Så här grupperar du din arbetslista:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Klicka på **Anpassa** om du vill lägga till någon av följande widgetar:

   | Widget | Beskrivning |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Varumärkena | Visar alla anslagstavlor som du har skapat eller har bjudits in att använda |
   | Mitt arbete | Visar uppgifter och ärenden som du har tilldelats |
   | Mina projekt | Visar projekt som du äger eller projekt som du arbetar med |
   | Mina uppgifter | Visar uppgifter som tilldelats dig |
   | Mina problem | Visar problem som du har tilldelats |
   | Mina förfrågningar | Visar alla begäranden som du har skickat in |
   | Mina godkännanden | Visar alla väntande, tilldelade, delegerade och inskickade godkännanden |

1. Klicka på ikonen **Grupp** ![Gruppera &#x200B;](assets/group-icon.png) i det övre högra hörnet av widgetens arbetslista.
1. Välj en **föreslagen** gruppering eller en gruppering som du har skapat.
   ![Gruppering utökad](assets/grouping-expanded.png)


## Anpassa kolumner för arbetslistor

Du kan välja vilka kolumner som ska visas i widgetens arbetslista:

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. (Villkorligt) Klicka på **Anpassa** om du vill lägga till någon av följande widgetar:

   | Widget | Beskrivning |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Varumärkena | Visar alla anslagstavlor som du har skapat eller har bjudits in att använda |
   | Mitt arbete | Visar uppgifter och ärenden som du har tilldelats |
   | Mina projekt | Visar projekt som du äger eller projekt som du arbetar med |
   | Mina uppgifter | Visar uppgifter som tilldelats dig |
   | Mina problem | Visar problem som du har tilldelats |
   | Mina förfrågningar | Visar alla begäranden som du har skickat in |
   | Mina godkännanden | Visar alla väntande, tilldelade, delegerade och inskickade godkännanden |

1. Klicka på ikonen **Kolumn** ![Kolumn &#x200B;](assets/column-icon.png) i det övre högra hörnet i widgetens arbetslista.
1. Aktivera och inaktivera kolumnerna beroende på dina inställningar.
1. (Valfritt) Klicka på ikonen **Dra** ![Dra ikonen &#x200B;](assets/drag-icon.png) för att ändra ordning på kolumnerna.
   ![Kolumner utökade](assets/columns-expanded.png)


## Visa sena artiklar

[!DNL Adobe Workfront] använder följande datum för att avgöra om arbetsförfrågningar är sena:

* **Uppgifter**: [!UICONTROL Planned Completion Date]
* **Problem**: [!UICONTROL Planned Completion Date]
* **Dokument**: [!UICONTROL Submitted date]
* **Tidrapporter**: [!UICONTROL Submitted date]
* **Godkännanden**: [!UICONTROL Submitted date]
* **Korrektur för godkännanden**: [!UICONTROL Proof deadline]


