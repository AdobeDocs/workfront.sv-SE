---
title: Hur äldre åtkomstnivåer och behörigheter fungerar tillsammans
user-type: administrator
content-type: reference
product-area: system-administration
keywords: åtkomst,modell,tratt,diagram,nivåer,behörigheter
navigation-topic: access-levels
description: Adobe Workfront-administratören avgör vilken åtkomstnivå varje användare ska ha. Åtkomstnivån definierar vad användare kan se och göra med objekttyper och områden i systemet.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Hur äldre åtkomstnivåer och behörigheter fungerar tillsammans

>[!NOTE]
>
>Informationen i den här artikeln avser de äldre åtkomstnivåerna. Mer information om de aktuella åtkomstnivåerna finns i [Översikt över nya åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

Adobe Workfront-administratören avgör vilken åtkomstnivå varje användare ska ha. Åtkomstnivån definierar vad användare kan se och göra med objekttyper och områden i systemet.

Användarna får även åtkomst till enskilda objekt när andra användare delar och ger vissa behörigheter för dessa objekt.


![Säkerhetsmodellhierarki](assets/security-model-hierachy.png)

Om din åtkomstnivå till exempel anger att du kan skapa uppgifter, men de behörigheter du får i ett visst projekt inte tillåter att du lägger till uppgifter i det, kan du inte lägga till uppgifter i projektet trots att du kan skapa uppgifter någon annanstans i Workfront.

Den här artikeln förklarar hur den här kombinationen fungerar.

## Åtkomstnivå

Åtkomstnivån som tilldelats varje användare av en Workfront-administratör krävs för att logga in på Workfront.

Standardåtkomstnivåerna är:

* Systemadministratör (kopplad till avtalslicensen)
* Planering (bifogad till planlicensen)
* Arbetare (kopplad till arbetslicensen)
* Granskare (bifogad till granskningslicensen)
* Begärande (bifogad till begärandelicensen)
* Extern användare (kopplad till den externa e-postlicensen)

Workfront-licensen för varje standardåtkomstnivå avgör vad som är tillgängligt och konfigurerbart på åtkomstnivån. Mer information om Workfront-licenser finns i [Översikt över Adobe Workfront-licenser](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

För de användare som är tilldelade till den anger en åtkomstnivå vad de kan se och göra med följande objekttyper och områden i Workfront:

* Projekt
* Uppgifter
* Problem
* Portföljer
* Rapporter, instrumentpaneler och kalendrar
* Filter, vyer och grupperingar
* Dokument
* Andra användare
* Mallar
* Finansiella data
* Resurshantering
* Scenarioplan
* Workfront-mål

På en anpassad åtkomstnivå kan du konfigurera inställningarna för dessa objekt och områden för att ändra hur mycket åtkomst användarna har till dem. Beroende på vilken licens som är kopplad till åtkomstnivån, samt typen av objekt eller område, kan du konfigurera åtkomstnivån så att ingen åtkomst, åtkomst eller redigering tillåts till ett objekt eller område.

>[!IMPORTANT]
>
>Vi rekommenderar att du låter de inbyggda åtkomstnivåerna vara oförändrade så att du kan referera till dem när du har konfigurerat användarna. Om du vill anpassa en åtkomstnivå kopierar du standardåtkomstnivån och ändrar kopian. (Du kan göra detta för alla åtkomstnivåer förutom systemadministratör och extern användare.)

En detaljerad förklaring av alla standardåtkomstnivåer finns i [Inbyggda åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Instruktioner om hur du tilldelar en åtkomstnivå till en användare finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Behörigheter

När du delar ett objekt med någon i systemet kan en användare ge mottagaren någon av följande behörigheter till objektet.

* **Visa**: Den här behörighetsnivån tillåter mottagaren att dela objektet på något av följande sätt:

   * System-wide så att alla användare kan se det (inte tillgängligt för alla objekt)
   * Med externa användare som inte har någon Workfront-licens (inte tillgänglig för alla objekt)
   * Med en e-postadress (endast tillgängligt för dokument)

* **Contribute**: (inte tillgängligt för alla objekt)
* **Hantera**: När någon delar ett objekt bestäms mottagarens rättigheter till objektet av en kombination av mottagarens åtkomstnivå och behörigheterna till objektet som har beviljats av delningslisten. Den lägsta åtkomstnivån som är tillgänglig i den kombinationen är vad som avgör vad mottagaren kan göra med objektet.

  >[!INFO]
  >
  >**Exempel:** Om mottagarens åtkomstnivå inte tillåter projektredigering kan den personen inte redigera eller ta bort ett projekt även om den som delar har gett behörighet att hantera det.
  >
  >Eller, om mottagarens åtkomstnivå tillåter projektredigering, men användaren bara har gett behörighet att visa ett projekt, kan användaren inte redigera eller ta bort projektet.

I följande tabell jämförs en användares allmänna åtkomst till objekt (som definieras av användarens åtkomstnivå) med behörigheter för ett specifikt delat objekt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>Åtkomstnivå </th> 
   <th>Behörigheter </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Beviljad av en Workfront-administratör på en användares åtkomstnivå</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Beviljas av en användare som delar ett objekt på objektnivå</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Ärvs från ett delat objekt med högre rankning 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Om en användare delar ett objekt med vissa behörigheter och det objektet har underordnade objekt under sig, ärver mottagaren samma behörigheter för dessa underordnade objekt.
>* Om en åtkomstnivå begränsar användare från att ta bort vissa objekt, hindras de inte från att ta bort underordnade objekt som finns i dessa objekt.
>

## Fler exempelscenarier

När Olivia delar ett Workfront-projekt med Tony bestäms Tony av en kombination av två saker:

* Tony&#39;s access level, som tilldelats av Workfront-administratören
* Tony&#39;s permissions to the project, specified by Olivia

Tony kan begränsa sitt arbete i projektet ytterligare, men det får inte vara obegränsat utöver det som är tillåtet på hans åtkomstnivå:

* Om Tony inte har behörighet att skapa uppgifter kan han inte lägga till uppgifter i projektet, även om Olivia gett honom behörighet att lägga till uppgifter i det.
* Om Tony på sin åtkomstnivå tillåter sig att skapa uppgifter, men Olivia inte gav behörighet att lägga till uppgifter i projektet, kan han inte lägga till uppgifter i projektet, men han kan lägga till uppgifter i andra projekt där han har fått tillstånd att göra det.
