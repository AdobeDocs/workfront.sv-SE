---
title: Översikt över åtkomstnivåer
user-type: administrator
content-type: reference
product-area: system-administration
keywords: åtkomst,nivå,system,administratör,standard,ljus,medarbetare
navigation-topic: access-levels
description: Alla användare måste ha en åtkomstnivå för att kunna logga in och arbeta i Workfront. Du använder åtkomstnivån för att styra vad en användare kan se och göra med vissa Workfront-objekt och -områden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 0%

---

# Översikt över åtkomstnivåer

>[!NOTE]
>
>Informationen i den här artikeln hänvisar till de aktuella åtkomstnivåerna. Mer information om de äldre åtkomstnivåerna finns i [Översikt över åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Som Adobe Workfront-administratör tilldelar du en åtkomstnivå till en användare för två syften:

* Alla användare måste ha en åtkomstnivå för att kunna logga in och arbeta i Workfront.
* Du använder åtkomstnivån för att styra vad en användare kan se och göra med vissa Workfront-objekt och -områden.

## Nya inbyggda åtkomstnivåer i Adobe Workfront {#built-in-access}

Workfront har fem nya inbyggda åtkomstnivåer:

* Systemadministratör
* Standard
* Ljus
* Medarbetare
* Extern

Beroende på åtkomstnivån är upp till tre behörigheter tillgängliga för de flesta Workfront-objekttyperna:

<table style="table-layout:auto">
    <tr>
        <td>Redigera</td>
        <td>Användare kan skapa, redigera, ta bort och dela Workfront-objekt</td>
    </tr>
    <tr>
        <td>Visa</td>
        <td>Användare kan granska och dela Workfront-objekt</td>
    </tr>
    <tr>
        <td>Ingen åtkomst</td>
        <td>Användare har inte åtkomst till Workfront-objektet</td>
    </tr>
</table>

Om du behöver en anpassad åtkomstnivå kan du kopiera den inbyggda åtkomstnivån och justera hur mycket åtkomst du vill ha för de olika Workfront-objekttyperna. Mer information om hur du skapar en anpassad åtkomstnivå finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Vi rekommenderar att du låter de inbyggda åtkomstnivåerna vara oförändrade så att du kan referera till dem när du har konfigurerat användarna.

### Åtkomstnivå för systemadministratör

Denna inbyggda åtkomstnivå är kopplad till standardlicensen och är utformad för en användare som ansvarar för att administrera Adobe Workfront-systemet. Du kan inte ändra den här inbyggda åtkomstnivån.

Användare med åtkomstnivån Systemadministratör kan göra allt inom Workfront. De kan visa och redigera alla Workfront-objekt och all information som andra användare har angett i Workfront.

De har även tillgång till hela inställningsområdet, där de kan ändra alla inställningar på systemnivå och komma åt alla områden på huvudmenyn.

Mer information finns i [Bevilja en användare fullständig administrativ åtkomst](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Standardåtkomstnivå

Den här åtkomstnivån är även kopplad till standardlicensen och är utformad för användare som:

* Planera, skapa och spåra alla projekt på ett ställe
* Automatisera rutinprocesserna
* Hantera resurser
* Spåra och samarbeta vid förfrågningar
* Spåra och rapportera om projektekonomi
* Kicka inkommande arbetsförfrågningar
* Samarbeta om projekt, uppgifter och ärenden

>[!NOTE]
>
>Du kan skapa en anpassad version av den inbyggda standardåtkomstnivån och justera åtkomstnivån för de olika Workfront-objekttyperna. Mer information om hur du skapar en anpassad åtkomstnivå finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Åtkomstinformation**

Följande är de högsta tillgängliga åtkomstinställningarna för objekt på standardåtkomstnivån:

| Workfront objekttyp | Ingen åtkomst | Visa åtkomst | Redigera åtkomst |
|---|---|---|---|
| Projekt |   |   | ✓ |
| Uppgifter |   |   | ✓ |
| Problem |   |   | ✓ |
| Portföljer |   |   | ✓ |
| Program |   |   | ✓ |
| Rapporter (inklusive instrumentpaneler och kalenderrapporter) |   |   | ✓ |
| Filter, vyer och grupperingar |   |   | ✓ |
| Dokument |   |   | ✓ |
| Användare |   |   | ✓ |
| Mallar |   |   | ✓ |
| Finansiella uppgifter |   |   | ✓ |
| Resurshantering |   |   | ✓ |
| Scenarioplan |   |   | ✓ (Standardinställningen är Ingen åtkomst.) |
| Mål |   |   | ✓ |

{style="table-layout:auto"}

### Ljus åtkomstnivå

Den här åtkomstnivån är kopplad till Light-licensen och är utformad för användare som:

* Visa alla artiklar och uppdateringar som är kopplade till arbetet
* Godkänn projekt, uppgifter och ärenden
* Visa instrumentpaneler och rapporter
* Spåra tid för projekt, uppgifter och ärenden och godkänn tidrapporter
* Skapa och hantera problem

Användare med åtkomstnivån Light:

* Kan tilldelas arbetsobjekt men kan inte slutföra dem.
* Kan komma åt förfrågningar och dokument på huvudmenyn.
* Har begränsad möjlighet att skapa objekt - de kan inte skapa projekt, portfolior, program eller rapporter.
* Det går bara att logga tiden på projektnivå när Redigera-åtkomst är aktiverat. De kan inte skapa, redigera, ta bort eller dela projekt.

>[!NOTE]
>
>Du kan skapa en anpassad version av den inbyggda åtkomstnivån Light (Ljus) och justera åtkomstnivån för de olika Workfront-objekttyperna. Mer information om hur du skapar en anpassad åtkomstnivå finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Åtkomstinformation**

Följande är de högsta tillgängliga åtkomstinställningarna för objekt på åtkomstnivån Ljus:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront objekttyp</th> 
   <th>Ingen åtkomst</th> 
   <th>Visa åtkomst</th> 
   <th>Redigera åtkomst</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekt</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (för loggningstid på projektnivå)</td> 
  </tr> 
  <tr> 
   <td>Uppgifter</td> 
   <td> </td> 
   <td></td> 
   <td>✓ (begränsad)</td> 
  </tr> 
  <tr> 
   <td>Problem</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Portföljer</td> 
   <td> </td> 
   <td>✓ (Standardinställningen är Ingen åtkomst.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Program</td> 
   <td> </td> 
   <td>✓ (Standardinställningen är Ingen åtkomst.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Rapporter (inklusive instrumentpaneler och kalenderrapporter)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filter, vyer och grupperingar</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dokument</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Användare</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
    <tr> 
   <td>Team</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr>
  <tr> 
   <td>Mallar</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Finansiella uppgifter</td> 
   <td></td> 
   <td> <p>✓(standardinställningen är Ingen åtkomst)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Resurshantering</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Scenarioplan </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Standardinställningen är Ingen åtkomst.)</td> 
  </tr>

<tr>   
   <td>Mål </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Standardinställningen är Ingen åtkomst)</td> 
 </tbody> 
</table>

### Åtkomstnivå för deltagare

Den här åtkomstnivån är kopplad till Contributor-licensen och är utformad för användare som:

* Skicka begäranden
* Spåra förfrågningar
* Uppdatera och granska förfrågningar
* Godkänn begäranden

Användare med denna inbyggda åtkomstnivå:

* Kan göra förfrågningar och uppdatera dem
* Kan överföra och godkänna dokument
* Kan godkänna projekt, uppgifter och ärenden

  >[!NOTE]
  >
  >Medarbetare kan delta i godkännanden, men kan inte öppna fliken Godkännanden för att visa eller hantera godkännandeprocesser.

* Kan granska status för de utgåvor som de har skickat in
* Kan tilldelas arbetsobjekt men kan inte slutföra dem
* Kan bara komma åt begäranden från huvudmenyn. Mer information om begärandeköer finns i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Du kan skapa en anpassad version av den inbyggda åtkomstnivån för Contributor och justera den åtkomstnivå som tillåts för de olika Workfront-objekttyperna. Mer information om hur du skapar en anpassad åtkomstnivå finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Åtkomstinformation**

Följande är de högsta tillgängliga åtkomstinställningarna för objekt på åtkomstnivån för Contributor:

| Workfront objekttyp | Ingen åtkomst | Visa åtkomst | Redigera åtkomst |
|---|---|---|---|
| Projekt |   | ✓ (begränsat) |   |
| Uppgift |   | ✓(begränsad) |   |
| Problem |   |   | ✓ |
| Portföljer |   | ✓ |   |
| Program |   | ✓ |   |
| Rapporter (inklusive instrumentpaneler och kalenderrapporter) |   | ✓ (Endast fliken Detaljer) |   |
| Filter, vyer och grupperingar |   |   | ✓ |
| Dokument |   |   | ✓ |
| Användare |   | ✓ |   |
| Team |   | ✓ |   |
| Mallar | ✓ |   |   |
| Finansiella uppgifter | ✓ |   |   |
| Resurshantering | ✓ |   |   |
| Scenarioplan | ✓ |   |   |
| Mål |   |   | ✓ (Standardinställningen är Ingen åtkomst) |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>Från och med version 24.7 har medverkande som standard åtkomst till Program och portföljer.
>
> 
>Medverkande som anlitas före version 24.7 har som standard fortfarande ingen åtkomst till Program och portföljer. Du kan uppdatera deras åtkomst för att visa dem manuellt om det behövs.

### Åtkomstnivå för externa användare

Den här åtkomstnivån är inte kopplad till en betald Workfront-licens. Det är den mest restriktiva åtkomstnivån, som främst utformats för medarbetare som externa konsulter som inte loggar in på Workfront, men som behöver granska, ladda ned eller visa dokument ibland.

Användare med extern användaråtkomst:

* Kan endast visa dokument och kalenderrapporter som delas med dem
* Visa de användare som delar dokument och kalenderrapporter med sig
* Godkänn de dokument som delas med dem

Externa användare kan inte tilldelas till arbetsobjekt.

Du kan inte ändra den här åtkomstnivån.

>[!IMPORTANT]
>
>Extern användare är bara tillgänglig om alternativet Samarbeta med personer utan Workfront-konton genom att använda deras e-postadress är aktiverat i området Systeminställningar i Inställningar. Mer information finns i [Konfigurera systemsäkerhetsinställningar](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **Åtkomstinformation**

Följande är de högsta tillgängliga åtkomstinställningarna för objekt på åtkomstnivån Extern användare.

| Workfront objekttyp | Ingen åtkomst | Visa åtkomst | Redigera åtkomst |
|---|---|---|---|
| Projekt | ✓ |   |   |
| Uppgift | ✓ |   |   |
| Problem | ✓ |   |   |
| Portföljer | ✓ |   |   |
| Program | ✓ |   |   |
| Rapporter (inklusive instrumentpaneler och kalenderrapporter) |   | ✓ (Endast för kalenderrapporter, det går inte att dela rapporter) |   |
| Filter, vyer och grupperingar | ✓ |   |   |
| Dokument |   | ✓ (Det går inte att dela dokument) |   |
| Användare |   | ✓ |   |
| Team | ✓ |   |   |
| Mallar | ✓ |   |   |
| Finansiella uppgifter | ✓ |   |   |
| Resurshantering | ✓ |   |   |
| Scenarioplan | ✓ |   |   |
| Mål | ✓ |   |   |


## Hur åtkomstnivåer och behörigheter fungerar tillsammans

Åtkomstnivåer definierar vad användare kan se och göra med allmänna objekttyper och områden i systemet, t.ex. projekt, uppgifter och problem. Behörigheter definierar vad du har tillgång till på specifika objekt som skapats av andra personer i systemet, till exempel ett projekt som skapats för att köra en marknadsföringskampanj.

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

De aktiviteter som en användare kan utföra med ett objekt definieras genom en kombination av åtkomstnivå och behörigheter som användaren får.

![Säkerhetsmodellhierarki](assets/security-model-hierachy-copy.png)

### Bevilja behörigheter genom att dela objekt

Användare får åtkomst till enskilda objekt när andra användare delar och ger vissa behörigheter för dessa objekt.

>[!NOTE]
>
>* Om en användare delar ett objekt med vissa behörigheter och det objektet har underordnade objekt under sig, ärver mottagaren samma behörigheter för dessa underordnade objekt.
>* Om en åtkomstnivå begränsar användare från att ta bort vissa objekt, hindras de inte från att ta bort underordnade objekt som finns i dessa objekt.

En användare kan ge mottagaren någon av följande behörigheter till det enskilda objektet:

* **Visa**: Den här behörighetsnivån tillåter mottagaren att dela objektet på något av följande sätt:

   * System-wide så att alla användare kan se det (inte tillgängligt för alla objekt)
   * Med externa användare som inte har någon Workfront-licens (inte tillgänglig för alla objekt)
   * Med en e-postadress (endast tillgängligt för dokument och kalendrar)

* **Contribute**: (inte tillgängligt för alla objekt)
* **Hantera**: När någon delar ett objekt bestäms mottagarens rättigheter till objektet av en kombination av mottagarens åtkomstnivå och behörigheterna till objektet som har beviljats av delningslisten. Den lägsta åtkomstnivån som är tillgänglig i den kombinationen är vad som avgör vad mottagaren kan göra med objektet.

### Exempel på scenarier

#### **Scenario 1**

Om mottagarens åtkomstnivå inte tillåter projektredigering kan den personen inte redigera eller ta bort ett projekt även om den som delar har gett behörighet att hantera det.

Eller, om mottagarens åtkomstnivå tillåter projektredigering, men användaren bara har gett behörighet att visa ett projekt, kan användaren inte redigera eller ta bort projektet.

#### **Scenario 2**

När Olivia delar ett Workfront-projekt med Tony bestäms Tony av en kombination av två saker:

* Tony&#39;s access level, som tilldelats av Workfront-administratören
* Tony&#39;s permissions to the project, specified by Olivia

Tony kan begränsa sitt arbete i projektet ytterligare, men det får inte vara obegränsat utöver det som är tillåtet på hans åtkomstnivå:

* Om Tony inte har behörighet att skapa uppgifter kan han inte lägga till uppgifter i projektet, även om Olivia gett honom behörighet att lägga till uppgifter i det.
* Om Tony på sin åtkomstnivå tillåter sig att skapa uppgifter, men Olivia inte gav behörighet att lägga till uppgifter i projektet, kan han inte lägga till uppgifter i projektet, men han kan lägga till uppgifter i andra projekt där han har fått tillstånd att göra det.
