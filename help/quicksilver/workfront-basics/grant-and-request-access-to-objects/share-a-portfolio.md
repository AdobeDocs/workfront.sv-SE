---
title: Dela en portfölj
description: Du kan dela en portfölj med andra användare om du har behörighet att komma åt den.
author: Courtney
draft: Probably
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: 4ae96f67b15838403ffce32317d871d6904d6d95
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# Dela en portfölj

Din Adobe Workfront-administratör kan ge dig åtkomst att visa eller redigera portföljer när du tilldelar din åtkomstnivå. Du måste ha en planlicens för att kunna redigera en portfölj. Mer information finns i [Bevilja åtkomst till portföljer](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md).

Förutom den åtkomstnivå du har beviljats kan du även få behörighet att visa eller hantera specifika portföljer från användare som kan dela dem med dig. Mer information om åtkomstnivåer och behörigheter finns i [Hur åtkomstnivåer och behörigheter fungerar tillsammans](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Behörigheterna är specifika för ett objekt i Workfront och definierar vilka åtgärder som användare kan vidta för det objektet.


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p> 
   <p>Arbeta eller högre</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst eller senare till de objekt som du vill dela</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter eller högre för de objekt som du vill dela</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när det gäller att dela portföljer

Förutom övervägandena nedan, se även [Översikt över delningsbehörigheter för objekt](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>En Workfront-administratör kan lägga till eller ta bort behörigheter för alla objekt i systemet, för alla användare, utan att vara ägare av dessa objekt.

* Skaparen av en portfölj har som standard behörigheten Hantera.
* Du kan dela en portfölj individuellt eller dela flera portföljer samtidigt. Att dela en portfölj är detsamma som att dela andra objekt i Workfront. Mer information finns i [Dela ett objekt](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Du kan bara bevilja behörigheterna Visa eller Hantera för portföljer.
</span>
* När du delar en portfölj ärver användarna samma behörigheter till alla underordnade objekt som är associerade med portföljen som standard.

Mer information om objekthierarkin i Workfront finns i [Förstå objekt i Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Du kan ta bort ärvda behörigheter från Portfolio. Mer information om hur du tar bort behörigheter från objekt finns i [Ta bort behörigheter från objekt](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Dela en portfölj

{{step1-to-portfolios}}

1. På sidan **Portföljer** väljer du den portfölj du vill dela. Portföljsidan öppnas.

1. Klicka på **Dela** till höger om portföljnamnet. Dialogrutan **Dela [Portfolio-namn]** öppnas.

   ![Knappen Dela portfölj](assets/share-portfolio-button.png)

1. I fältet **Bevilja portföljåtkomst till** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela portföljen med och klickar sedan på namnet i listrutan.

   >[!TIP]
   >
   >Du kan bara dela en portfölj med aktiva användare, team, roller eller företag.


1. (Valfritt) Välj listrutan **Vem har åtkomst** och välj portföljens åtkomstnivå:

   * **Endast inbjudna personer har åtkomst:** Endast användare som är inbjudna till portföljen har åtkomst till den (Standard).
   * **Alla i systemet kan visa**: Alla användare i systemet kan visa portföljen utan en inbjudan.

1. Klicka på listrutan till höger om användarens namn och välj behörighetsnivå för den här portföljen:

   * **Visa**: Användaren kan granska och dela portföljen.
   * **Hantera**: Användaren har fullständig åtkomst till portföljen utan administratörsrättigheter, som ges på åtkomstnivån (inklusive alla visningsbehörigheter).

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har beviljat för att konfigurera specifika behörigheter för portföljen.

   ![Konfigurerade avancerade behörighetsalternativ](assets/advanced-options-icon.png)

1. (Valfritt) Om du snabbt vill dela portföljen med hjälp av en länk klickar du på **Kopiera länk** och vidarebefordrar den till mottagaren.

1. Klicka på **Spara**.

## Dela portfolior i grupp

{{step1-to-portfolios}}

1. Markera rutan till vänster om varje portfölj som du vill dela på sidan **Portföljer** och klicka sedan på ikonen **Dela** ![Dela](assets/share-icon.png) överst på sidan. Delningen modal öppnas.

   ![Dela flera portföljer](assets/bulk-share-portfolios.png)

1. I fältet **Bevilja portföljåtkomst till** börjar du skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela portföljerna med och klickar sedan på namnet i listrutan.

   >[!TIP]
   >
   >Du kan bara dela portföljer med aktiva användare, team, roller eller företag.


1. (Valfritt) Välj listrutan **Vem har åtkomst** och välj portföljens åtkomstnivå:

   * **Endast inbjudna personer har åtkomst:** Endast användare som är inbjudna till portföljerna har åtkomst till dem (Standard).
   * **Alla i systemet kan visa**: Alla användare i systemet kan visa portföljerna utan en inbjudan.


1. Klicka på listrutan till höger om användarens namn och välj behörighetsnivå för portföljerna:

   * **Visa**: Användaren kan granska och dela portföljer.
   * **Hantera**: Användaren har fullständig åtkomst till portföljerna utan administratörsbehörighet, som ges på åtkomstnivån (inklusive alla visningsbehörigheter).

1. (Valfritt) Klicka på ikonen för avancerade alternativ bredvid behörighetsnivån som du har tilldelat för att konfigurera specifika behörigheter för portföljerna.

   ![Konfigurerade avancerade behörighetsalternativ](assets/advanced-options-icon.png)

1. Klicka på **Spara**.


## Portfolio-behörigheter

Tabellen nedan visar vilka behörigheter du kan ge användare när de får visa eller hantera en Portfolio:

| **Åtgärder** | **Hantera** | **Visa** |
|---|---|---|
| Redigera Portfolio-information | ✓ |   |
| Se en Portfolio | ✓ | ✓ |
| Ta bort en Portfolio | ✓ |   |
| Bifoga ett eget formulär | ✓ |   |
| Redigera ett anpassat fält | ✓ |   |
| Lägg till eller ta bort ett program&#42; | ✓ |   |
| Lägg till eller ta bort ett projekt&#42; | ✓ |   |
| Godkänn ett projekt | ✓ |   |
| Portfolio-optimering&#42; | ✓ |   |
| Lägg till en dokumentmapp &#42; | ✓ | ✓ |
| Lägga till ett dokument | ✓ | ✓ |
| Uppdateringar/kommentarer | ✓ | ✓ |
| Dela | ✓ | ✓ |
| Dela hela systemet |   | ✓ |

*Behörigheterna styrs av åtkomstnivån och behörigheterna för andra objekt, som projekt, program och dokument.
