---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Anpassa vilka fält som visas på ett kort
description: Du kan anpassa vilka fält som ska visas på ett kort genom att inaktivera ett fält så att det inte visas i det fullständiga kortet eller den komprimerade vyn, eller genom att dölja ett fält i den komprimerade kortvyn.
author: Lisa
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: 63d043a85c2e5300d8b5872b2ec7983de4ba1f50
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# Anpassa vilka fält som visas på ett kort

Som standard visas alla tillgängliga fält på ett kort, både i den fullständiga vyn när kortet är öppet och i den komprimerade kortvyn på kortet. Du kan anpassa vilka fält som visas av:

* Inaktivera ett fält så att det inte visas i någon av vyerna
* Dölja ett fält i den komprimerade kortvyn

Om ett fält innehåller ett värde och du inaktiverar fältet behålls värdet om du aktiverar fältet igen senare.

Avsnitt (som visas som alternativ för vänster navigering på kortinformationen) kan också visas och döljas.

Du kan även visa anpassade fält som tidigare skapats. Du kan inte designa och skapa nya anpassade fält på en anslagstavla.

>[!NOTE]
>
>Alla fältanpassningar du gör gäller bara för den styrelse du arbetar i.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr>
   </tbody> 
</table>

&#42;Kontakta din [!DNL Workfront] administratör.

## Konfigurera kort {#configure-cards}

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Boards]**.
1. Gå till en styrelse. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka [!UICONTROL **Konfigurera**] till höger om ritytan för att öppna panelen Konfigurera.
1. Expandera [!UICONTROL **Kort**].

   De flesta fält och avsnitt är aktiverade som standard.

1. Stäng av ett fält eller avsnitt för att inaktivera det i båda kortvyerna.
1. Klicka på ikonen Dölj ![Dölj ikon](assets/eye-hide-icon.png) bredvid ett fält eller avsnitt för att dölja det i den komprimerade vyn.
1. Om du vill visa alla fält och avsnitt i båda vyerna klickar du på [!UICONTROL **Återställ alla fält till standard**].
1. Klicka [!UICONTROL **Dölj konfigurera**] för att stänga panelen Konfigurera.

## Lägg till anpassade fält till kort

Anpassade fält är tillgängliga på anslutna kort. De visas bara i helskärmsläge, inte i den komprimerade vyn.

Informationen i anpassade fält kan redigeras på kortet, men vissa anpassade element kan bara redigeras i det ursprungliga fältet och inte på kortet.

1. Gå till en anslagstavla och klicka [!UICONTROL **Konfigurera**] för att öppna panelen Konfigurera.
1. Expandera [!UICONTROL **Kort**].
1. Under [!UICONTROL Card Fields], klicka [!UICONTROL **Lägg till anpassat fält**].
1. Välj [!UICONTROL **Uppgift**] eller [!UICONTROL **Problem**].

   Kategorierna för tillgängliga fält för uppgifter eller ärenden visas. Expandera en kategori om du vill visa alla fält. Du kan också söka efter ett fält.

   ![Sök efter anpassat fält](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Följande fälttyper kan inte läggas till i kort: Adobe XD, Image, PDF, Video.

1. Markera fältnamnet.
1. (Valfritt) Klicka på **[!UICONTROL Field value]** om du vill ändra det här anpassade fältet till ett annat.
1. (Valfritt) Ändra **[!UICONTROL Field label]** till det fältnamn som du vill ska visas på kort.
1. När du är klar med ändringarna klickar du [!UICONTROL **Spara fält**].

   ![Eget fältvärde och etikett](assets/save-custom-field-value-label.png)

   Det anpassade fältet läggs till i listan med tillgängliga fält och aktiveras som standard. Du kan inaktivera det anpassade fältet enligt stegen i [Konfigurera kort](customize-fields-on-card.md#configure-cards) ovan, redigera fältet eller ta bort det från alla kort.

>[!NOTE]
>
>Om du senare byter namn på det anpassade fältet i Workfront måste du redigera fältetiketten på konfigurationspanelen så att den matchar, annars visas inte fältet på korten.
