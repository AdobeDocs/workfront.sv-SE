---
title: Begär behörighet till en vy eller en Workspace
description: När någon delar en länk till en vy eller arbetsyta som du inte har åtkomst till, kan du begära behörighet för att kunna öppna den. I den här artikeln förklaras stegen för att begära åtkomst till en vy eller arbetsyta när du stöter på en delad länk som du inte kan öppna.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 1e62d5c7eff86432b4914793d75cdf4f835f3d5d
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---


# Begära behörigheter till en vy eller arbetsyta

>[!IMPORTANT]
>
>De funktioner som beskrivs i den här artikeln är bara tillgängliga när din organisation har anslutit sig till Adobe Unified Experience.
>
>Mer information finns i [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).


Du kan begära behörigheter för en vy eller arbetsyta när någon delar en länk med dig till vyn eller arbetsytan som du inte har åtkomst till.

Att begära behörigheter till en vy liknar att begära behörigheter till en arbetsyta.

I den här artikeln beskrivs hur du begär åtkomst till en vy eller arbetsyta när någon delar en länk med dig och du inte har åtkomst till den delade sidan.

Mer information om hur du tilldelar behörigheter till vyer och arbetsytor finns i följande artiklar:

* [Visa](/help/quicksilver/planning/access/share-views.md)
* [Dela arbetsytor](/help/quicksilver/planning/access/share-workspaces.md)


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för Workfront Planning.

Du måste ha följande för att kunna komma åt Workfront Planning:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkter</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan*</p></td> 
   <td> 
<p>Något av följande Workfront-planer:</p> 
<ul><li>Välj</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning är inte tillgängligt för tidigare Workfront-planer</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning*</p></td> 
   <td> 
<p>Alla </p> 
<p>Mer information om vad som ingår i varje Workfront Planning-plan finns i <a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfront priser och paketering</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<p>Din organisations instans av Workfront måste integreras med Adobe Unified Experience för att få tillgång till alla funktioner i Workfront Planning.</p> 
<p><b>VIKTIGT</b></p>
<p>Användarna i din organisation kan begära behörigheter för vyer och arbetsytor endast när din organisation är registrerad på Adobe Unified Experience. </p>
<p>Mer information finns i <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td> 
   <td><p> Standard, Light eller Contributor</p>
   <p>Workfront Planning är inte tillgängligt för tidigare Workfront-licenser</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td> 
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>  <p>När din behörighetsbegäran har beviljats kan du få följande behörigheter:</p>
   <ul><li><p>Visa eller hantera för en vy</p></li>
   <li><p>Visa, Contribute eller Hantera på en arbetsyta</p></li></ul>  
   <p>Endast användare med behörigheten Hantera på en arbetsyta och en vy kan dela en vy offentligt.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutmall</p></td> 
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> </td> 
  </tr> 
</tbody> 
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Begär behörigheter till en vy eller arbetsyta

Att begära behörigheter till en vy liknar att begära behörighet till en arbetsyta.

När någon delar en länk till en arbetsyta eller en vy där du inte har tillgång till den med dig:

1. Klicka på länken som delas med dig för vyn eller arbetsytan.

   En **Du har inte åtkomst**-sida visas som informerar dig om att du inte har åtkomst till vyn eller arbetsytan.

   ![](assets/request-access-to-view.png)

1. (Villkorligt) Om den delade länken är för en vy för en arbetsyta där du har åtkomst klickar du på **Öppna med befintlig vy**. Om du har behörighet att komma åt arbetsytan öppnas posttypssidan i standardvyn.

1. (Valfritt och villkorligt) Om du inte har behörighet att visa arbetsytan lägger du till ett anpassat meddelande i rutan som är tillgänglig och klickar sedan på **Begär åtkomst**.

   Alla användare med behörigheten Hantera för vyn eller arbetsytan får följande meddelanden om åtkomstbegäran:
   * Ett meddelande i appen
     ![](assets/in-app-notification-for-access-request.png)
   * Ett e-postmeddelande
     ![](assets/email-notification-for-access-request.png)

1. (Villkorligt) När arbetsytehanteraren ger dig behörighet till vyn eller arbetsytan får du ett e-postmeddelande och ett meddelande i appen med en bekräftelse på att behörighet har beviljats. <!--check this - I was not able to test this, but Isk confirmed.-->


