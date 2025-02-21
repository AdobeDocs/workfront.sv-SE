---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Skapa ett interaktivt korrektur för en webbplats eller annat webbinnehåll
description: Du kan generera ett nytt interaktivt korrektur eller en ny version av ett befintligt interaktivt korrektur för webbinnehåll. Det kan vara en webbplats eller andra typer av interaktivt innehåll, som annonser med direktuppspelad video eller ljud, HTML-animeringar och interaktiva banners.
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# Skapa ett interaktivt korrektur för en webbplats eller annat webbinnehåll

Du kan generera ett nytt interaktivt korrektur eller en ny version av ett befintligt interaktivt korrektur för webbinnehåll. Det kan vara en webbplats eller andra typer av interaktivt innehåll, som annonser med direktuppspelad video eller ljud, HTML-animeringar och interaktiva banners.

I ett interaktivt korrektur kan granskarna navigera och interagera som vanligt med webbplatsen eller annat webbinnehåll.

>[!IMPORTANT]
>
>Se till att webbplatsen eller det interaktiva innehållet är tillgängligt för dem som ska granska den. De har bara tillgång till det i korrekturläsningen om de även kan använda det på internet.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Gammal plan: Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
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

## Skapa ett interaktivt korrektur för en webbplats eller annat webbinnehåll

1. Gå till projektet, uppgiften eller utgåvan där du vill skapa ett nytt korrektur för en webbplats eller en ny version av ett befintligt.
1. Klicka på **Dokument** i den vänstra panelen.
1. (Villkorligt) Om du skapar ett nytt korrektur klickar du på **Lägg till nytt** och sedan på **Korrektur** på menyn som visas.

1. (Villkorligt) Om du skapar en ny version av ett befintligt korrektur visas sidan **Nytt korrektur**:

   1. Håll pekaren över det URL-korrektur som du vill skapa en ny version för och markera det sedan genom att klicka i den ljusblå bakgrunden runt det.

      ![Select_proof_by_selection_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)


   1. I listrutan **Lägg till ny** klickar du på **Version** > **Korrektur**.

1. I avsnittet **Lägg till filer** skriver du webbadressen till den webbplats som du vill korrekturgranska och trycker sedan på **Retur**.  Du kan upprepa den här processen om du vill lägga till flera webbplatser som ska korrektur.

   ![proof_website.png](assets/proof-website-350x65.png)


   >[!NOTE]
   >
   > URL:en får inte innehålla fler än 1 000 tecken.

1. Klicka på den URL som du har lagt till.

   ![Klicka på URL](assets/click-url-350x137.png)

1. (Valfritt) Om du vill ändra namnet på korrekturet från webbplatsens URL till något annat anger du ett **korrekturnamn**.
1. Välj **Interaktiv** och klicka sedan på **Klar**.

   >[!NOTE]
   >
   >Om du lägger till en ny version till ett befintligt URL-korrektur behålls alla alternativ som konfigurerats på det ursprungliga korrekturet eller den tidigare versionen i den här versionen.

1. Klicka på **Skapa korrektur** om du vill skapa ett enkelt korrektur utan någon granskningsprocess.\
   eller\
   Fortsätt genom att konfigurera ett avancerat korrektur:

   * [Skapa ett avancerat korrektur med ett grundläggande arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
