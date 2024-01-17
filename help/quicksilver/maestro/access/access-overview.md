---
title: Åtkomstöversikt
description: Det finns begränsningar för licens- och delningsbehörighet för att använda Adobe Maestro-funktionerna.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 99fac041-a235-4991-b826-d19944164bc9
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->
<!--update the title and the metadata title if Maestro is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Åtkomstöversikt

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe Workfront.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder. Du måste vara Workfront-kund för att få tillgång till Maestro.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](/help/quicksilver/maestro/maestro-overview.md).

Det finns begränsningar för licens- och delningsbehörighet för att använda Adobe Maestro-funktionerna.

## Åtkomstkrav

Du måste ha följande inställningar för att kunna använda Adobe Maestro:

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
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Maestro stängt. </p>
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
   Användarna måste ha följande licens för att skapa arbetsytor: 
   <ul><li><p>Nytt: Standard</p> </li>
   <li><p>Aktuell: Arbetare eller högre</p> </li></ul>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Åtkomstnivåkonfiguration</p></td>
   <td> <p>Det finns inga åtkomstnivåkontroller för Maestro-objekt</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektbehörigheter</p></td>
   <td>
   <p>Contribute eller högre behörigheter för arbetsytor och vyer som du inte skapat för att redigera, ta bort eller dela dem</p>
    <p>Systemadministratörer kan hantera arbetsytor och vyer som de inte skapade </p>
   <p>Mer information om att dela behörigheter för Maestro-objekt finns i  
   <a href="../access/sharing-permissions-overview.md">Översikt över delningsbehörigheter i Adobe Maestro</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutmall</p></td>
   <td> <p>Systemadministratören måste lägga till Maestro-området på huvudmenyn i layoutmallen.</p> 
   <p>Mer information finns i <a href="../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md">Anpassa huvudmenyn med hjälp av en layoutmall</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

*Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Dela Maestro-området på huvudmenyn med andra

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

När din organisation har registrerats i betaprogrammet för Maestro kan du lägga till Maestro-området på huvudmenyn för alla användare med hjälp av en layoutmall.

1. Logga in på **Workfront** som Workfront-administratör.

1. Lägg till **Maestro** icon ![](assets/maestro-icon.png) till **Huvudmeny** med **Layoutmall**.

   Mer information finns i [Anpassa huvudmenyn med hjälp av en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Tilldela layoutmallen till de användare som du vill ska ha tillgång till Maestro.

   Mer information finns i [Tilldela användare till en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Alla användare som är tilldelade mallen kan nu komma åt Maestro på huvudmenyn.

   Användare kan börja skapa arbetsytor, posttyper, poster och fält.

## Ge åtkomst

Det finns inga åtkomstkontroller för Maestro.

Användare med alla typer av licenser har tillgång till Maestro.

## Bevilja behörigheter

Du måste ge användare som inte är systemadministratörer behörighet till arbetsytor och vyer som du skapar för att de ska kunna komma åt dem.

Mer information finns i [Översikt över delningsbehörigheter i Adobe Maestro](/help/quicksilver/maestro/access/sharing-permissions-overview.md).


