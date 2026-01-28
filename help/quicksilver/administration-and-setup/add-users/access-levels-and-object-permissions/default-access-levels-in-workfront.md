---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: åtkomst,modell,tratt,diagram,nivåer,behörigheter
navigation-topic: access-levels
title: Inbyggda åtkomstnivåer (äldre)
description: Var och en av de sex inbyggda åtkomstnivåerna är utformad för en viss typ av användare, inklusive systemadministratör, planerare, arbetare, granskare, begärare och extern användare. Dessa åtkomstnivåer låter dig styra vad användare kan redigera och visa i systemet. Om du behöver en anpassad åtkomstnivå kan du kopiera en inbyggd åtkomstnivå och ändra den efter den åtkomstnivå du vill ha för de olika Workfront-objekttyperna.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '1656'
ht-degree: 0%

---

# Inbyggda åtkomstnivåer (äldre)

<!--Audited: 01/2024-->

>[!NOTE]
>
>Informationen i den här artikeln avser de äldre åtkomstnivåerna. Mer information om de aktuella åtkomstnivåerna finns i [Översikt över nya åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).


Var och en av de sex inbyggda åtkomstnivåerna är utformad för en viss typ av användare. Dessa åtkomstnivåer låter dig styra vad användare kan redigera och visa i systemet.

Var och en av de sex inbyggda åtkomstnivåerna har utformats för följande typer av användare:

* Systemadministratör
* Planering
* Arbetare
* Granskare
* Begärande
* Extern användare

Beroende på åtkomstnivån är upp till tre inställningar tillgängliga för de flesta Workfront-objekttyper:

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

Om du behöver en anpassad åtkomstnivå för planerare, arbetare, beställare eller granskare kan du kopiera den inbyggda åtkomstnivån och fastställa hur stor åtkomst du vill att den ska tillåta för de olika Workfront-objekttyperna.

>[!TIP]
>
>Du kan inte ändra åtkomstnivåerna för systemadministratören eller den externa användaren.

Mer information om hur du skapar en anpassad åtkomstnivå eller ändrar någon av de inbyggda åtkomstnivåerna finns i [Skapa och ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Vi rekommenderar att du låter de inbyggda åtkomstnivåerna vara oförändrade så att du kan referera till dem när du har konfigurerat användarna.

Allmän information om dessa åtkomstnivåer finns i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Åtkomstnivå för systemadministratör

Den inbyggda åtkomstnivån för systemadministratörer är kopplad till avtalslicensen och är utformad för en användare som ansvarar för att administrera Adobe Workfront-systemet. Du kan inte ändra den här inbyggda åtkomstnivån.

Användare med åtkomstnivån Systemadministratör kan göra allt i Workfront. De kan visa och redigera alla Workfront-objekt och all information som andra användare har angett i Workfront.

De har också fullständig åtkomst till inställningsområdet, där de kan ändra alla inställningar på systemnivå. De har även åtkomst till alla områden på huvudmenyn ![Huvudmenyikonen](assets/main-menu-icon.png) eller huvudmenyikonen ![Huvudmeny](assets/main-menu-icon.png), om den är tillgänglig.

Mer information finns i [Bevilja en användare fullständig administrativ åtkomst](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Åtkomstnivå för plan

Planneråtkomstnivån är även kopplad till avtalslicensen och är utformad för:

* Chefer för grupper, team, projekt och resurser
* Alla som ansvarar för planering, skapande och hantering av uppgifter, projekt, portfolior och program
* Alla som ansvarar för att tilldela arbete (uppgifter och ärenden) till andra användare
* Användare som skapar rapporter och som godkänner tidrapporter, arbetsuppgifter och dokument
* Användare som behöver åtkomst till alla områden på huvudmenyn ![Ikon för huvudmeny](assets/main-menu-icon.png) eller huvudmeny ![ikon för huvudmeny](assets/main-menu-icon.png), om den är tillgänglig

Du kan skapa en anpassad version av den inbyggda åtkomstnivån för planeraren och fastställa hur mycket åtkomst den tillåter för de olika Workfront-objekttyperna. Mer information finns i [Skapa och ändra anpassade åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Följande är de högsta tillgängliga åtkomstinställningarna för objekt på åtkomstnivån Planering:

| Workfront objekttyp | Ingen åtkomst | Visa åtkomst | Redigera åtkomst |
|---|---|---|---|
| Projekt |   |   | ✓ |
| Uppgifter |   |   | ✓ |
| Problem |   |   | ✓ |
| Portföljer |   |   | ✓ |
| Program |   |   | ✓ |
| Rapporter, instrumentpaneler och kalendrar |   |   | ✓ |
| Filter, vyer och grupperingar |   |   | ✓ |
| Dokument |   |   | ✓ |
| Användare |   |   | ✓ |
| Team |   |   | ✓ |
| Mallar |   |   | ✓ |
| Finansiella data |   |   | ✓ |
| Resurshantering |   |   | ✓ |
| Scenarioplan |   |   | ✓ (Standardinställningen är Ingen åtkomst.) |
| Workfront-mål |   |   | ✓ (Standardinställningen är Ingen åtkomst.) |

{style="table-layout:auto"}

## Åtkomstnivå för arbetare

Åtkomstnivån för Worker bifogas till arbetslicensen och är utformad för användare som utför arbetet i Workfront. De planerar inte arbetet, de slutför det.

Användare med den här åtkomstnivån:

* Tilldelas arbetsobjekt där de kan bidra och loggtiden
* Kan godkänna arbete och dokument, men inte tidrapporter
* Kan få åtkomst till och dela rapporter
* Kan kommunicera med andra användare i systemet
* Det går inte att komma åt alla områden på huvudmenyn ![Huvudmenyikon](assets/main-menu-icon.png) eller huvudmenyikonen ![Huvudmeny](assets/main-menu-icon.png), om den är tillgänglig, och deras&quot;Användare&quot;-område heter Teams. I Teams-området kan användare med den här åtkomstnivån bara visa team som de tillhör, tillsammans med arbetet som tilldelats dessa team.
* Har begränsad möjlighet att skapa objekt - de kan inte skapa projekt, portfolior, program eller rapporter.

Du kan skapa en anpassad version av den inbyggda åtkomstnivån för Worker och bestämma hur mycket åtkomst den tillåter för de olika Workfront-objekttyperna. Mer information finns i [Skapa och ändra anpassade åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Följande är de högsta tillgängliga åtkomstinställningarna för objekt på Worker-åtkomstnivån:

| Workfront objekttyp | Ingen åtkomst | Visa åtkomst | Redigera åtkomst |
|---|---|---|---|
| Projekt |   |   | ✓ (Begränsat: användare kan bara dela projektet, skapa aktiviteter och problem i det och redigera data i anpassade formulär som redan är kopplade till det.) |
| Uppgifter |   |   | ✓ |
| Problem |   |   | ✓ |
| Portföljer |   | ✓ (Standardinställningen är Ingen åtkomst.) |   |
| Program |   | ✓ (Standardinställningen är Ingen åtkomst.) |   |
| Rapporter, instrumentpaneler och kalendrar |   | ✓ |   |
| Filter, vyer och grupperingar |   |   | ✓ |
| Dokument |   |   | ✓ |
| Användare |   |   | ✓ |
| Team |   |   | ✓ (begränsad åtkomst) |
| Mallar | ✓ |   |   |
| Finansiella data |   | ✓ (Standardinställningen är Ingen åtkomst. Med visningsinställningen kan användaren bara visa området Ekonomi   i projektinformation.) |   |
| Resurshantering |   | ✓ |   |
| Scenarioplan |   |   | ✓ (Standardinställningen är Ingen åtkomst.) |
| Workfront-mål |   |   | ✓ (Standardinställningen är Ingen åtkomst.) |

{style="table-layout:auto"}

## Åtkomstnivå för granskare

Granskarens åtkomstnivå bifogas granskningslicensen och är utformad för chefer som begär arbete från andra användare och som granskar och godkänner arbetet. Dessa är inte projektägare eller teammedlemmar, men de måste ha tillgång till Workfront för att kunna se de arbetsuppgifter de ansvarar för.

En berörd part med denna åtkomstnivå kan till exempel logga in på Workfront för att delta i en pågående granskning av marknadsföringsmaterial, se arbetsuppdateringar och granska dokument, godkännanden, rapporter och kalendrar.

Användare med åtkomstnivån Reviewer:

* Det går inte att tilldela arbetsobjekt eller godkänna tidrapporter
* Kan komma åt områdena Begäranden och dokument på huvudmenyn ![Ikon för huvudmeny](assets/main-menu-icon.png) eller huvudmeny ![Ikon för huvudmeny](assets/main-menu-icon.png), om sådana finns
* Har begränsad möjlighet att skapa objekt - de kan inte skapa projekt, portfolior, program eller rapporter.

Du kan skapa en anpassad version av den inbyggda åtkomstnivån i Reviewer och bestämma hur mycket åtkomst den tillåter för de olika Workfront-objekttyperna. Mer information finns i [Skapa och ändra anpassade åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Mer begränsat för projekt och uppgifter än Worker-åtkomstnivån, är följande de högsta tillgängliga åtkomstinställningarna för objekt på åtkomstnivån Reviewer:

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
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Uppgifter</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
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
   <td>Rapporter, instrumentpaneler, kalendrar</td> 
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
   <td>Finansiella data</td> 
   <td> </td> 
   <td> <p>✓ (Standardinställningen är Ingen åtkomst. Med visningsinställningen kan användaren bara visa området Ekonomi   i projektinformation.)</p> </td> 
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
   <td>Workfront-mål </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Standardinställningen är Ingen åtkomst.)</td> 
  </tr> 
 </tbody> 
</table>

## Åtkomstnivå för begärande

Åtkomstnivån för begärande är kopplad till begärandelicensen och är utformad för användare som gör och tar emot enkla arbetsförfrågningar i Workfront. Som standard är de begränsade till området Begäranden.

En användare kan t.ex. logga problem i din organisations kö för helpdesk-begäran.

Användare med den här åtkomstnivån:

* Kan göra förfrågningar och uppdatera dem
* Kan överföra och godkänna dokument
* Kan granska status för de utgåvor som de har skickat in
* Det går inte att tilldela arbetsobjekt
* Det går bara att komma åt begäranden från området Förfrågningar på huvudmenyn ![Ikon för huvudmeny](assets/main-menu-icon.png) eller huvudmenyikon ![Huvudmeny](assets/main-menu-icon.png), om den är tillgänglig. Mer information om begärandeköer finns i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Du kan skapa en anpassad version av den inbyggda åtkomstnivån för den begärande och fastställa hur mycket åtkomst den tillåter för de olika Workfront-objekttyperna. Mer information finns i [Skapa och ändra anpassade åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Följande är de högsta tillgängliga åtkomstinställningarna för objekt på åtkomstnivån för begärande:

| Workfront objekttyp | Ingen åtkomst | Visa åtkomst | Redigera åtkomst |
|---|---|---|---|
| Projekt |   | ✓ (Endast sidan Projektinformation) |   |
| Uppgift |   | ✓(Endast sidan Uppgiftsinformation) |   |
| Problem |   |   | ✓ |
| Portföljer | ✓ |   |   |
| Program | ✓ |   |   |
| Rapporter, instrumentpaneler och kalendrar |   | ✓ |   |
| Filter, vyer och grupperingar |   |   | ✓ |
| Dokument |   |   | ✓ |
| Användare |   | ✓ |   |
| Team |   | ✓ |   |
| Mallar | ✓ |   |   |
| Finansiella data | ✓ |   |   |
| Resurshantering | ✓ |   |   |
| Scenarioplan | ✓ |   |   |
| Workfront-mål |   |   | ✓ (Standardinställningen är Ingen åtkomst.) |

{style="table-layout:auto"}

## Åtkomstnivå för externa användare

Åtkomstnivån Extern användare är inte kopplad till en betald Workfront-licens. Det är den mest restriktiva åtkomstnivån, som främst är utformad för medarbetare, t.ex. externa konsulter som inte loggar in på Workfront, men som behöver granska, ladda ned eller visa dokument ibland.

Workfront-användare kan tilldela uppgifter till externa användare även om externa användare inte kan logga in på systemet. Vi rekommenderar dock inte att du tilldelar uppgifter och utgåvor till externa användare, eftersom detta arbete inte skulle kunna lösas i systemet.

Användare med extern användaråtkomst:

* Kan endast visa dokument och kalenderrapporter som delas med dem
* Kan visa användare som delar dokument och kalenderrapporter med sig
* Kan godkänna dokument som delas med dem

Du kan inte ändra den här åtkomstnivån.

>[!IMPORTANT]
>
>Extern användare är bara tillgänglig om alternativet Samarbeta med personer utan Workfront-konton genom att använda deras e-postadress är aktiverat i området Systeminställningar i Inställningar. Mer information finns i [Konfigurera systemsäkerhetsinställningar](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Även om de här inställningarna inte visas i området Åtkomstnivåer för åtkomstnivån Extern användare har en användare med den här åtkomsten den högsta åtkomsten till Workfront-objekttyperna:

| Workfront objekttyp | Ingen åtkomst | Visa åtkomst | Redigera åtkomst |
|---|---|---|---|
| Projekt | ✓ |   |   |
| Uppgift | ✓ | |   |
| Problem | ✓ |   |   |
| Portföljer | ✓ |   |   |
| Program | ✓ |   |   |
| Rapporter, instrumentpaneler och kalendrar |   | ✓ (Endast för kalenderrapporter, det går inte att dela rapporter) |   |
| Filter, vyer och grupperingar | ✓ |   |   |
| Dokument |   | ✓ (utan möjlighet att dela dokument) |   |
| Användare |   | ✓ |   |
| Team |   | ✓ |   |
| Mallar | ✓ |   |   |
| Finansiella data | ✓ |   |   |
| Resurshantering | ✓ |   |   |
| Scenarioplan | ✓ |   |   |
| Workfront-mål | ✓ |   |   |
