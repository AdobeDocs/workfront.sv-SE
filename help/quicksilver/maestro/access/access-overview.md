---
title: Åtkomstöversikt
description: Det finns begränsningar för licens- och delningsbehörighet för att använda Adobe Workfront-planering.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront planning. This article describes the levels of access that users could have to Adobe Workfront planning. -->
<!--update the title and the metadata title if Workfront planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Åtkomstöversikt

{{maestro-important-intro}}

Det finns begränsningar för licens- och delningsbehörighet för att använda Adobe Workfront-planering.

## Åtkomstkrav

Du måste ha följande inställningar för att kunna använda Adobe Workfront-planering:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Workfront planerar stängda. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens*</p></td>
   <td>
   <p>Alla</p>
   <p>Om du vill skapa arbetsytor måste du ha följande licens:</p>
   <ul>
   <li>
   Nytt: Standard
   </li>
   <li>
   Aktuell: Arbetare eller högre
   </li>
   </ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Adobe Workfront-planering</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektbehörigheter</p></td>
   <td>
   <p>Contribute eller högre behörigheter för arbetsytor och vyer som du inte skapat för att redigera, ta bort och dela dem samt för att skapa, redigera eller ta bort posttyper och poster.</p>
    <p>Systemadministratörer kan hantera arbetsytor som de inte skapade. </p>
    <p>Systemadministratörer kan inte hantera vyer som de inte skapade. </p>
   <p>Mer information om att dela behörigheter för att planera funktionsobjekt finns i  
   <a href="../access/sharing-permissions-overview.md">Översikt över delningsbehörigheter i Adobe Workfront-planeringen</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Alla användare, inklusive Workfront-administratörer, måste tilldelas en layoutmall som innehåller planeringsområdet på huvudmenyn. </p> <p>Mer information finns i <a href="/help/quicksilver/maestro/access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Dela planeringsområdet på huvudmenyn med andra

<!--First, contact your account manager to obtain access to the current Workfront planning closed beta program.-->

När din organisation har registrerats i betaprogrammet för Workfront-planering kan du lägga till planeringsområdet på huvudmenyn för alla användare med hjälp av en layoutmall.

1. Logga in på **Workfront** som Workfront-administratör.

1. Lägg till **Planering** icon ![](assets/maestro-icon.png) till **Huvudmeny** med **Layoutmall**.

   Mer information finns i [Anpassa huvudmenyn med hjälp av en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Tilldela layoutmallen till de användare som du vill ska ha tillgång till Workfront-planeringen.

   Mer information finns i [Tilldela användare till en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Alla användare som är tilldelade mallen kan nu komma åt Workfront-planering på huvudmenyn.

   Användare kan börja skapa arbetsytor, posttyper, poster och fält.

## Ge åtkomst

Det finns inga åtkomstkontroller för Workfront-planering.

Användare med alla typer av licenser har tillgång till Workfront planering.

Information om hur du beviljar åtkomst i Workfront finns i [Skapa och ändra anpassade åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Bevilja behörigheter

Du måste ge användarna behörigheter till arbetsytor och vyer som du skapar för att de ska kunna komma åt dem.

Mer information finns i [Översikt över delningsbehörigheter i Adobe Workfront-planeringen](/help/quicksilver/maestro/access/sharing-permissions-overview.md).

Din Adobe Workfront-licenstyp fungerar tillsammans med dina planeringsbehörigheter för Workfront så att du kan visa, bidra till eller hantera Workfront planeringsobjekt.

Mer information om hur licenstyper påverkar behörighetsnivåer för Workfront planeringsobjekt finns i [Översikt över licenstyp vid användning av Adobe Workfront-planering](/help/quicksilver/maestro/access/license-type-overview.md).


