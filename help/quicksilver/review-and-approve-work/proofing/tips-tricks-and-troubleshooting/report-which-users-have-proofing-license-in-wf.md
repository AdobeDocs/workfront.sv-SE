---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Visa en lista över användare som har en korrekturlicens i Adobe Workfront
description: 'Du kan se vilka användare i Adobe Workfront som har alternativet "Användaren kan generera korrektur" aktiverat på något av följande sätt:'
author: Courtney
feature: Digital Content and Documents
exl-id: 4d45ecd9-4348-43a4-9fa7-090b996b4695
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '369'
ht-degree: 0%

---

# Visa en lista över användare som har en korrekturlicens i Adobe Workfront

Du kan se vilka användare i Adobe Workfront som har alternativet &quot;Användaren kan generera korrektur&quot; aktiverat på något av följande sätt:

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Redigera åtkomst till:</p> 
    <ul> 
     <li> <p>Skapa rapporter, instrumentpaneler och kalendrar</p> </li> 
     <li> <p>Skapa filter, vyer och grupperingar</p> </li> 
    </ul> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

## Skapa en användarrapport

Du kan skapa en användarrapport som visar vilka användare som kan generera korrektur:

1. Navigera till området **Rapportering**.
1. Klicka på listrutan **Ny rapport** och sedan på **Användarrapport**.

1. Klicka på **Lägg till en filterregel** på fliken **Filter**.

1. Expandera **Användare** i det tillgängliga fältet och klicka sedan på **Har korrekturlicens**.

1. Välj **Lika med** > **Sant**.

   ![report_prooflicenses.png](assets/report-prooflicenses-350x135.png)

1. Klicka på **Spara+Stäng**.

   I rapporten visas alla användare i Workfront som har tilldelats en språklicens.

## Uppdatera vyn Personer

Du kan lägga till en ny kolumn i vyn Personer för att visa vilka användare som kan generera korrektur:

1. Gå till området **Personer**.
1. Klicka på fliken **Personer**.
1. Gör något av följande i listrutan **Visa**:

   * Om du vill lägga till den här informationen i en befintlig vy markerar du den vy som du vill anpassa och klickar sedan på **Anpassa vy**.
   * Om du vill lägga till den här informationen i en ny vy klickar du på **Ny vy**.

1. Klicka på **Lägg till kolumn**.
1. Expandera **Användare** i det tillgängliga fältet och klicka sedan på **Har korrekturlicens**.

1. Klicka på **Klar** och sedan på **Spara vy** eller **Spara som ny vy**.

   Vyn visar **True** eller **False** beroende på om användaren har tilldelats en språklicens.
