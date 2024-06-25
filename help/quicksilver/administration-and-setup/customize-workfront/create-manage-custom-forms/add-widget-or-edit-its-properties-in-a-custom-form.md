---
title: Lägga till eller redigera en bild eller en annan resurswidget i ett anpassat formulär med det äldre formulärverktyget
description: Du kan lägga till eller redigera egenskaper för följande resurswidgetar, till exempel bilder, videoklipp, PDF-filer och Adobe XD-filer i ett anpassat formulär. Detta är användbart när du behöver inkludera visuellt innehåll som varumärkesbilder, en instruktionsvideo eller en interaktiv prototyp för ett program som du designar.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 0%

---

# Lägga till eller redigera en bild eller en annan resurswidget i ett anpassat formulär med det äldre formulärverktyget

{{form-designer-default}}

Du kan lägga till eller redigera egenskaperna för följande resurswidgetar i ett anpassat formulär:

* Bild
* Video
* PDF-fil
* Adobe XD

Detta är användbart när du behöver inkludera visuellt innehåll som varumärkesbilder, en instruktionsvideo eller en interaktiv prototyp för ett program som du designar.

När ett anpassat formulär som innehåller en widget är kopplat till ett objekt kan användare som arbetar med objektet se det i följande områden:

* Objektets detaljområde (t.ex. området Projektinformation för ett projekt)
* Rutan Redigera för objektet, om det har det nya Adobe Workfront-gränssnittet (t.ex. rutorna Redigera projekt och Redigera uppgift)

Användarna kan för närvarande inte se widgeten i följande områden: &#x200B;

* Listor och rapporter
* Hem och sammanfattning
* Rutan Redigera för objektet, om det inte har det nya Adobe Workfront-gränssnittet (t.ex. rutan Redigera utgift)
* Workfront mobilapp


## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer beviljar den här åtkomsten finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller vilka åtkomstnivåkonfigurationer du har.

## Lägga till eller redigera en resurswidget i ett anpassat formulär

1. Börja arbeta med ett anpassat formulär, enligt beskrivningen i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Med **Lägg till ett fält** Öppna en flik och gör något av följande:

   * Om du lägger till en ny widget väljer du **Bild**, **PDF**, eller **Video** om du vill lägga till det längst ned i formuläret eller dra det där du vill ha det i formuläret.

     ![](assets/add-widget.png)


   * Om du vill lägga till en widget som redan har lagts till i ett annat anpassat formulär klickar du på **Fältbibliotek** klickar du sedan på namnet på widgeten i listan som visas. Mer information finns i [Återanvända ett anpassat fält eller en anpassad widget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * Om du redigerar en widget som redan har lagts till i det anpassade formuläret markerar du den.

1. Ange eller redigera någon av följande egenskaper för widgeten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför widgeten. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Använd inte specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar widgeten.</p> <p>När du konfigurerar widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p> <p><b>VIKTIGT</b>: Även om det går att göra det rekommenderar vi att du inte ändrar det här namnet efter att du eller andra användare har börjat använda det anpassade formuläret i widgeten. Om du gör det kommer systemet inte längre att känna igen widgeten där den nu kan refereras i andra områden av Workfront. </p> <p>Varje widgetnamn måste vara unikt i din organisations Workfront-instans. På så sätt kan du återanvända ett som redan har skapats för ett annat anpassat formulär. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatoriskt) Skriv eller klistra in URL:en för widgeten där den lagras på Internet.</p> 
       <p><strong>Viktigt</strong>: URL:en för måste vara en offentlig URL. </p>
      <p>Om du lägger till en videowidget kan du göra det genom att lägga till följande i URL-rutan:</p> 
      <ul> 
      <li> <p>Länk till YouTube eller Vimeo</p> </li> 
      <li> <p>Google Drive - videolänk</p> </li> 
      <li> <p>Länka till video med MP4- och MOV-tillägg</p> </li> 
      <li> <p>Länk till video som redan har överförts till dokumentområdet i din Workfront-instans. Instruktioner finns i <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Lägga till en videowidget i ett anpassat formulär från området Dokument</a> i den här artikeln.</p> 
      </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instruktioner</td> 
      <td> <p>Skriv in ytterligare information om widgeten. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Storlek</td> 
      <td>Ändra visningsstorleken för widgeten efter behov.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Använd**.
1. Om du vill fortsätta att skapa ditt anpassade formulär på andra sätt kan du fortsätta med någon av följande artiklar:

   * [Placera anpassade fält och widgetar i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Återanvända ett anpassat fält eller en anpassad widget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Lägga till visningslogik och hoppa över logik i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Förhandsgranska och fylla i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## Lägga till en XD fil i ett anpassat formulär

1. Börja arbeta med ett anpassat formulär, enligt beskrivningen i [Skapa eller redigera ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Med **Lägg till ett fält** öppna flik, välja **Adobe XD**.
1. Ange eller redigera någon av följande egenskaper för widgeten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför widgeten. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Använd inte specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>(Obligatoriskt) Det här namnet är det som identifierar widgeten.</p> <p>När du konfigurerar widgeten för första gången och skriver etiketten fylls fältet Namn automatiskt i så att det matchar det. Men fälten Etikett och Namn är inte synkroniserade, vilket ger dig frihet att ändra etiketten som användarna ser utan att behöva ändra namnet som systemet ser.</p> <p><b>VIKTIGT</b>: Även om det går att göra det rekommenderar vi att du inte ändrar det här namnet efter att du eller andra användare har börjat använda det anpassade formuläret i widgeten. Om du gör det kommer systemet inte längre att känna igen widgeten där den nu kan refereras i andra områden av Workfront. </p> <p>Varje widgetnamn måste vara unikt i din organisations Workfront-instans. På så sätt kan du återanvända ett som redan har skapats för ett annat anpassat formulär. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>(Obligatoriskt) Skriv eller klistra in en giltig XD prototyplänk.</p> 
      <p>Obs! Inställningen Länkåtkomst på fliken Dela i Adobe XD måste vara inställd på Vem som helst med länken. Annars kan användarna inte visa prototypen. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instruktioner</td> 
      <td> <p>(Valfritt) Ange ytterligare information om widgeten. När användarna fyller i det anpassade formuläret kan de föra musen över frågeteckenikonen för att visa ett verktygstips som innehåller den information du skriver här.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Storlek</td> 
      <td>(Valfritt) Ändra visningsstorleken för widgeten efter behov.</td> 
     </tr> 
    </tbody> 
   </table>

1. Om du vill fortsätta att skapa ditt anpassade formulär på andra sätt kan du fortsätta med någon av följande artiklar:

   * [Placera anpassade fält och widgetar i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Lägga till ett anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Återanvända ett anpassat fält eller en anpassad widget i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Lägga till beräknade data i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Återanvända ett befintligt beräknat anpassat fält i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Lägga till visningslogik och hoppa över logik i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Förhandsgranska och fylla i ett anpassat formulär](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Lägga till en videowidget i ett anpassat formulär från området Dokument {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>När du lägger till en video i ett anpassat formulär på det här sättet gäller endast de behörigheter som angetts för det anpassade formuläret för videon när användarna öppnar formuläret för ett objekt, inte de behörigheter som angetts för videon i området Dokument.

1. Gå till videon i området Dokument och generera ett korrektur för den enligt beskrivningen i [Skapa ett interaktivt korrektur för en webbplats eller annat webbinnehåll](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Öppna beviset.
1. Högerklicka var som helst i videon och välj sedan **Kopiera videoadress**.
1. Klistra in den kopierade adressen i det anpassade formuläret där du lägger till videowidgeten **URL** box.
