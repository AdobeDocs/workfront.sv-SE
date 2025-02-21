---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Skapa ett statiskt korrektur för en webbplats eller annat webbinnehåll
description: Du kan generera ett nytt statiskt korrektur eller en ny version av ett befintligt statiskt korrektur för webbinnehåll. Webbinnehåll kan innehålla bl.a. annonser med direktuppspelad video, HTML-animeringar eller interaktiva banners, men det kommer att delas in i flera skärmbilder för statisk korrektur.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# Skapa ett statiskt korrektur för en webbplats eller annat webbinnehåll

Du kan generera ett nytt statiskt korrektur eller en ny version av ett befintligt statiskt korrektur för webbinnehåll. Webbinnehåll kan innehålla bl.a. annonser med direktuppspelad video, HTML-animeringar eller interaktiva banners, men det kommer att delas in i flera skärmbilder för statisk korrektur.

Tänk på följande när du skapar statiska korrektur för en webbplats eller annat webbinnehåll:

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

+++

## Skapa ett statiskt korrektur för en webbplats eller annat webbinnehåll

Om du vill skapa ett statiskt bevis måste webbplatsen vara tillgänglig för alla (inte bakom en brandvägg), eller så måste din organisations tillåtelselista innehålla Workfront-domänen. Workfront kan inte spara en lösenordsskyddad webbplats som ett statiskt korrektur.

>[!TIP]
>
>Vi rekommenderar interaktiv korrektur i stället för statisk korrektur för interna sidor som kräver behörighet och lösenordsskyddade sidor. Mer information finns i [Översikt över korrektur för interaktivt innehåll](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Gå till projektet, uppgiften eller utgåvan där du vill skapa ett nytt korrektur för en webbplats eller en ny version av ett befintligt.
1. Klicka på **Dokument** i den vänstra panelen.
1. (Villkorligt) Om du skapar ett nytt korrektur klickar du på **Lägg till nytt** och sedan på **Korrektur** på menyn som visas.
1. (Villkorligt) Om du skapar en ny version av ett befintligt korrektur:

   1. För musen över det URL-korrektur som du vill skapa en ny version för och markera det sedan genom att klicka i den ljusblå bakgrunden runt det.

      ![Select_proof_by_selection_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Klicka på **Lägg till ny** > **Version** > **Korrektur**.

1. Skriv webbadressen till den webbplats som du vill korrekturgranska i området **Lägg till filer** och tryck sedan på **Retur**.

   >[!NOTE]
   >
   > URL:en får inte innehålla fler än 2 000 tecken.

1. Klicka på den URL som du har lagt till.

   Alternativen för att konfigurera korrekturet för webbplatsen visas.

   ![Interaktivt korrektur](assets/interactive-proof-radio-btn-area-350x199.png)

1. (Valfritt) Om du vill ändra namnet på korrekturet från webbplatsens URL till något annat anger du ett **korrekturnamn.**
1. Kontrollera att **Skärmbilden** för hämtning är markerad och använd något av följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Skärmbildupplösning</strong> </td> 
      <td> <p>Justera upplösningen för materialet när granskarna visar korrekturet så att de kan se hur det ser ut på enheter av olika storlek, t.ex. telefoner, surfplattor och bildskärmar.</p> <p>Om du väljer flera upplösningar skapas ett separat korrektur för varje upplösning som du väljer.</p> <p>Obs! När en granskare kommenterar korrekturet innehåller kommentaren den upplösning som visades när kommentaren gjordes, så att andra granskare vet vilken upplösning som är associerad med kommentaren. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Leta efter undersidor</strong> </td> 
      <td> <p>Spara webbplatsens undersidor och dess huvudsidor. Du kan klicka på Markera alla om du vill ta med alla sidor, eller klicka bara på vissa sidor som du vill ta med. Med plus- och minusknapparna kan du expandera och stänga undersidesområdena på webbplatsen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Du kan inte ändra inställningen för skärmbild i Capture för efterföljande versioner av korrekturet som du skapar.

1. Klicka på **Klar**.

   Om du valde flera skärmbildupplösningar i steg 8 innehåller listan en uppsättning skärmbilder för varje upplösning. Du kan generera skärmbilderna som separata korrektur eller kombinera dem till ett enda korrektur (se  in .). Vi rekommenderar att du kombinerar dem, särskilt om du skapar ett statiskt webbplatskorrektur.

   >[!NOTE]
   >
   >Om du lägger till en ny version till ett befintligt URL-korrektur behålls alla alternativ som konfigurerats på det ursprungliga korrekturet eller den tidigare versionen i den här versionen.

1. Klicka på **Skapa korrektur** om du vill skapa ett enkelt korrektur utan någon granskningsprocess.\
   eller\
   Fortsätt genom att konfigurera ett avancerat korrektur:

   * [Skapa ett avancerat korrektur med ett grundläggande arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
