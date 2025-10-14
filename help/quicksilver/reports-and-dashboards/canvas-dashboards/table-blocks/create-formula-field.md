---
title: Skapa ett formelfält i Rapporteringsarbetsyta
description: Skapa ett formelfält i Rapporteringsarbetsyta
hidefromtoc: true
hide: true
exl-id: 22a2c3d7-39db-4f5d-94f3-222ca3ee0615
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# Skapa ett formelfält i Rapporteringsarbetsyta

Med fältverktyget i Rapportera arbetsyta kan du skapa fält som utför anpassade beräkningar.

## Förutsättningar

Innan du börjar måste du registrera dig för betaversionen av Reporting Canvas. Mer information finns i [Betaversion av arbetsyta för rapportering: översikt](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Skapa ett formelfält

1. Skapa eller navigera till ett tabellblock enligt beskrivningen i [Lägg till eller redigera ett tabellblock i Rapporteringsarbetsyta](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md).
1. Klicka på ikonen **Redigera** ![Redigera &#x200B;](assets/edit-icon.png) på tabellrubriken i rapporten.

   ![Ikonen Redigera i tabellrubriken](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Om du just har skapat tabellen och ännu inte har lagt till några fält klickar du i stället på knappen Redigera mitt i tabellen.

1. Klicka på **Nytt +** överst i listan **Fält** på den högra panelen.
1. Klicka på ikonen **Redigera** ![Redigera](assets/edit-icon.png) bredvid fältnamnet i det övre vänstra hörnet för att ändra formelfältets namn på den nya sidan som öppnas.
1. Dra **Funktioner** eller **Fält** från den vänstra panelen till fältverktyget i mitten för att lägga till dem i formelfältet.


   >[!TIP]
   >
   >När du skapar formelfältet visas exempel på det resulterande fältet i **fältförhandsvisningen** till höger.

   Varje funktion innehåller ett antal tomma prickade rektanglar som används som argument vid beräkningen av ett resultat. Dessa kan fyllas i genom att du anger statisk text eller siffror, drar och släpper ett fält från den vänstra panelen (med fältets värde i beräkningen) eller genom att dra och släppa en annan funktion (skapa en kapslad funktion). Möjliga funktioner:

   | Funktion | Beskrivning | Utdata |
   |---|---|---|
   | IF | Jämför två argument baserat på en vald modifierare och utför sedan en angiven åtgärd baserad på det resulterande värdet för Sant (Är sant:) eller Falskt (Är falskt:). Obs! För närvarande kan det andra argumentet inte vara ett statiskt True- eller False-värde. I stället kan du använda en kapslad funktion som ISBLANK (projektnamn) som alltid returnerar False som en tillfällig lösning. | True/False, Date, Number eller String |
   | KONKAT | Sammanfoga två eller flera strängar från början till slut för att skapa en ny sträng. | Sträng |
   | INNEHÅLLER | Utvärdera om ett strängargumentfält (söktext) finns i ett annat strängargumentfält (inom text). | Sant/falskt |
   | IN | Utvärdera om värdet i ett argumentfält (Sök) matchar värdet i minst ett annat argumentfält (Inom) | Sant/falskt |
   | ISBLANK | Utvärdera om ett argumentfält är tomt. | Sant/falskt |
   | LEN | Mät längden (i antal tecken) på ett argumentfält. | Nummer |
   | ROUND | Returnerar ett avrundat tal baserat på den valda precisionen. | Nummer |
   | FLOG | Returnerar närmaste heltal, avrundat nedåt. | Nummer |
   | NUMMER | Returnerar det största heltalet mindre än värdet för ett numeriskt argument (identiskt med en Floor-funktion). | Nummer |
   | STRÄNG | Konverterar innehållet i ett argumentfält till en sträng | Sträng |
   | ÄMNE | Skapa en ny sträng från en större sträng, som innehåller tecknen mellan ett indexnummer (Start) och ett annat (End). | Sträng |
   | VÄNSTER | Skapa en ny sträng från en större sträng, som innehåller tecken som börjar med det vänstra och räknar ett antal tecken (längd) åt höger. | Sträng |
   | HÖGER | Skapa en ny sträng från en större sträng, som innehåller tecken som börjar längst till höger och räknar ett antal tecken (längd) åt vänster. | Sträng |
   | SUM | Lägg ihop värdena för två eller flera argumentfält. | Nummer |
   | SUB | Subtrahera värdena i två eller flera argumentfält (från vänster till höger). | Nummer |
   | PROD | Multiplicera värdena i två eller flera argumentfält tillsammans. | Nummer |
   | DIV | Dividera värdet för två eller flera argumentfält (från vänster till höger). | Nummer |
   | MÅNAD | Returnerar ett tal som är lika med månadsvärdet för ett datum. | Nummer |
   | ÅR | Returnerar ett tal som är lika med årsvärdet för ett datum. | Nummer |
   | DATEDIFF | Beräknar det totala antalet dagar mellan två datum, avrundat till en decimal. | Nummer |
   | VECKDAYDIFF | Beräknar antalet veckodagar mellan två datum, avrundat till en decimal. | Nummer |

   {style="table-layout:auto"}

1. Klicka på pilen **Gå tillbaka** i det övre vänstra hörnet av skärmen för att gå tillbaka till tabellen.
