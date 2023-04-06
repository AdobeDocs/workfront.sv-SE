---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: åtkomst,modell,tratt,diagram,nivåer,behörigheter
navigation-topic: access-levels
title: Inbyggda åtkomstnivåer i Adobe Workfront
description: Var och en av de sex inbyggda åtkomstnivåerna är utformad för en viss typ av användare, inklusive systemadministratör, planerare, arbetare, granskare, begärare och extern användare. Dessa åtkomstnivåer låter dig styra vad användare kan redigera och visa i systemet. Om du behöver en anpassad åtkomstnivå kan du kopiera den inbyggda åtkomstnivån och fastställa hur mycket åtkomst du vill ha för de olika Workfront-objekttyperna.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 1bd454246419e199e5cfd0d8d1d73cd30c0b13b1
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 0%

---

# Inbyggda åtkomstnivåer i Adobe Workfront

Var och en av de sex inbyggda äldre åtkomstnivåerna är utformade för en viss typ av användare:

* Systemadministratör
* Planering
* Arbetare
* Granskare
* Begärande
* Extern användare

Beroende på den äldre åtkomstnivån är upp till tre inställningar tillgängliga för de flesta Workfront-objekttyper:

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

Om du behöver en anpassad åtkomstnivå för Planering, Arbetare, Beställare eller Granskare kan du kopiera den inbyggda äldre åtkomstnivån och fastställa hur mycket åtkomst du vill ha för de olika Workfront-objekttyperna. Mer information om hur du skapar en anpassad åtkomstnivå eller ändrar någon av de inbyggda äldre åtkomstnivåerna finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Vi rekommenderar att du låter de inbyggda äldre åtkomstnivåerna vara oförändrade så att du kan hänvisa till dem när du har konfigurerat användarna.

Allmän information om dessa åtkomstnivåer finns i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Åtkomstnivå för systemadministratör

Denna inbyggda äldre åtkomstnivå är kopplad till avtalslicensen och är utformad för en användare som ansvarar för att administrera Adobe Workfront-systemet. Du kan inte ändra den här inbyggda åtkomstnivån.

Användare med äldre systemadministratörsbehörighet kan göra allt inom Workfront. De kan visa och redigera alla Workfront-objekt och all information som andra användare har angett i Workfront.

De har även tillgång till hela inställningsområdet, där de kan ändra alla inställningar på systemnivå. Och de kan komma åt alla områden på huvudmenyn ![](assets/main-menu-icon.png).

Mer information finns i [Bevilja användaren fullständig administrativ åtkomst](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Åtkomstnivå för äldre plan

Den här åtkomstnivån är även kopplad till avtalslicensen och är utformad för:

* Chefer för grupper, team, projekt och resurser
* Alla som ansvarar för planering, skapande och hantering av uppgifter, projekt, portfolior och program
* Alla som ansvarar för att tilldela arbete (uppgifter och ärenden) till andra användare
* Användare som skapar rapporter och som godkänner tidrapporter, arbetsobjekt och dokument
* Användare som behöver åtkomst till alla områden på huvudmenyn ![](assets/main-menu-icon.png)

Du kan skapa en anpassad version av den inbyggda äldre åtkomstnivån för planeraren och fastställa hur stor åtkomst den tillåter för de olika Workfront-objekttyperna. Mer information finns i [Inbyggda åtkomstnivåer i Adobe Workfront](#Customiz) i den här artikeln.

Följande är de högsta tillgängliga åtkomstinställningarna för objekt på den äldre åtkomstnivån för planering:

| Workfront objekttyp | Ingen åtkomst | Visa åtkomst | Redigera åtkomst |
|---|---|---|---|
| Projekt |   |   | ✓ |
| Uppgifter |   |   | ✓ |
| Problem |   |   | ✓ |
| Portfolio |   |   | ✓ |
| Program |   |   | ✓ |
| Rapporter (inklusive instrumentpaneler och kalenderrapporter) |   |   | ✓ |
| Filter, vyer och grupperingar |   |   | ✓ |
| Dokument |   |   | ✓ |
| Användare |   |   | ✓ |
| Mallar |   |   | ✓ |
| Finansiella uppgifter |   |   | ✓ |
| Resurshantering |   |   | ✓ |
| Scenarioplan |   |   | ✓ (Standardinställningen är Ingen åtkomst.) |
| Workfront-mål |   |   | ✓ (Standardinställningen är Ingen åtkomst.) |

{style="table-layout:auto"}

## Åtkomstnivå för arbetare

Denna åtkomstnivå är kopplad till arbetslicensen och är utformad för användare som ska utföra arbetet i Workfront. De planerar inte arbetet. de slutför det.

Användare med den här åtkomstnivån:

* Tilldelas arbetsobjekt där de kan bidra och loggtiden
* Kan godkänna arbete och dokument, men inte tidrapporter
* Kan få åtkomst till och dela rapporter
* Kan kommunicera med andra användare i systemet
* Kan komma åt alla områden på huvudmenyn ![](assets/main-menu-icon.png), men deras&quot;Användare&quot; heter Teams. I Teams-området kan användare med den här åtkomstnivån bara visa team som de tillhör, tillsammans med arbetet som tilldelats dessa team.
* Har begränsad möjlighet att skapa objekt - de kan inte skapa projekt, portfolior, program eller rapporter.

Du kan skapa en anpassad version av den inbyggda äldre åtkomstnivån för Worker och fastställa hur stor åtkomst den tillåter för de olika Workfront-objekttyperna. Mer information finns i [Inbyggda åtkomstnivåer i Adobe Workfront](#Customiz) i den här artikeln.

Följande är de högsta tillgängliga åtkomstinställningarna för objekt på Worker-åtkomstnivån:

| Workfront objekttyp | Ingen åtkomst | Visa åtkomst | Redigera åtkomst |
|---|---|---|---|
| Projekt |   |   | ✓ (begränsad: -användare kan bara dela projektet, skapa uppgifter och problem i det och redigera data i anpassade formulär som redan är kopplade till det.) |
| Uppgifter |   |   | ✓ |
| Problem |   |   | ✓ |
| Portfolio |   | ✓ (Standardinställningen är Ingen åtkomst.) |   |
| Program |   | ✓ (Standardinställningen är Ingen åtkomst.) |   |
| Rapporter (inklusive instrumentpaneler och kalenderrapporter) |   | ✓ |   |
| Filter, vyer och grupperingar |   |   | ✓ |
| Dokument |   |   | ✓ |
| Användare |   |   | ✓ |
| Mallar | ✓ |   |   |
| Finansiella uppgifter |   | ✓ (Standardinställningen är Ingen åtkomst. Med visningsinställningen kan användaren bara visa området Ekonomi i projektinformationen.) |   |
| Resurshantering |   | ✓ |   |
| Scenarioplan |   |   | ✓ (Standardinställningen är Ingen åtkomst.) |
| Workfront-mål |   |   | ✓ (Standardinställningen är Ingen åtkomst.) |

{style="table-layout:auto"}

## Granska äldre åtkomstnivå

Denna åtkomstnivå är kopplad till granskningslicensen och är utformad för chefer som begär arbete från andra användare och som granskar och godkänner arbetet. Dessa är inte projektägare eller teammedlemmar, men de måste ha tillgång till Workfront för att kunna se de arbetsuppgifter de ansvarar för.

En berörd part med denna åtkomstnivå kan till exempel logga in på Workfront för att delta i en pågående granskning av marknadsföringsmaterial, se arbetsuppdateringar och granska dokument, godkännanden, rapporter och kalendrar.

Användare med åtkomstnivån Reviewer:

* Det går inte att tilldela arbetsobjekt eller godkänna tidtabeller
* Kan komma åt förfrågningar och dokument på huvudmenyn ![](assets/main-menu-icon.png).
* Har begränsad möjlighet att skapa objekt - de kan inte skapa projekt, portfolior, program eller rapporter.

Du kan skapa en anpassad version av den inbyggda äldre åtkomstnivån i Reviewer och bestämma hur mycket åtkomst den tillåter för de olika Workfront-objekttyperna. Mer information finns i [Inbyggda åtkomstnivåer i Adobe Workfront](#Customiz) i den här artikeln.

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
   <td>Portfolio</td> 
   <td> </td> 
   <td>✓</td> 
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
   <td>Mallar</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Finansiella uppgifter</td> 
   <td> </td> 
   <td> <p>✓ (Standardinställningen är Ingen åtkomst. Med visningsinställningen kan användaren bara visa området Ekonomi i projektinformationen.)</p> </td> 
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

## Begärande äldre åtkomstnivå

Den här åtkomstnivån bifogas till Request-licensen och är utformad för användare som gör och tar emot enkla arbetsförfrågningar i Workfront. Som standard är de begränsade till området Begäranden.

En användare kan t.ex. logga problem i din organisations kö för helpdesk-begäran.

Användare med den här åtkomstnivån:

* Kan göra förfrågningar och uppdatera dessa förfrågningar
* Kan överföra och godkänna dokument
* Kan granska status för de utgåvor som de har skickat in
* Det går inte att tilldela arbetsobjekt
* Kan bara komma åt begäranden från huvudmenyn ![](assets/main-menu-icon.png). Mer information om köer finns i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Du kan skapa en anpassad version av den inbyggda äldre åtkomstnivån för beställaren och fastställa hur stor åtkomst den tillåter för de olika Workfront-objekttyperna. Mer information finns i [Inbyggda åtkomstnivåer i Adobe Workfront](#Customiz) i den här artikeln.

Följande är de högsta tillgängliga åtkomstinställningarna för objekt på åtkomstnivån för begärande:

| Workfront objekttyp | Ingen åtkomst | Visa åtkomst | Redigera åtkomst |
|---|---|---|---|
| Projekt |   | ✓ (endast sidan Projektinformation) |   |
| Uppgift |   | ✓(Endast informationssidan) |   |
| Problem |   |   | ✓ |
| Portfolio | ✓ |   |   |
| Program | ✓ |   |   |
| Rapporter (inklusive instrumentpaneler och kalenderrapporter) |   | ✓ (Endast detaljsidan) |   |
| Filter, vyer och grupperingar |   |   | ✓ |
| Dokument |   |   | ✓ |
| Användare |   | ✓ |   |
| Mall | ✓ |   |   |
| Finansiella uppgifter | ✓ |   |   |
| Resurshantering | ✓ |   |   |
| Scenarioplan | ✓ |   |   |
| Workfront-mål |   |   | ✓ (Standardinställningen är Ingen åtkomst.) |

{style="table-layout:auto"}

## Åtkomstnivå för äldre externa användare

Den här åtkomstnivån är inte kopplad till en betald Workfront-licens. Det är den mest restriktiva åtkomstnivån, som främst är utformad för medarbetare, t.ex. externa konsulter som inte loggar in på Workfront, men som behöver granska, ladda ned eller visa dokument ibland.

Workfront-användare kan tilldela uppgifter till externa användare även om externa användare inte kan logga in på systemet. Men vi avråder från detta eftersom arbetet skulle förbli olöst i systemet.

Användare med åtkomstnivå Extern användare:

* Kan endast visa dokument och kalenderrapporter som delas med dem
* Se vilka användare som delar dokument och kalenderrapporter med sig
* Godkänn de dokument som delas med dem

Du kan inte ändra den här åtkomstnivån.

>[!IMPORTANT]
>
>Extern användare är bara tillgänglig om alternativet Samarbeta med personer utan Workfront-konton genom att använda deras e-postadress är aktiverat i området Systeminställningar i Inställningar. Mer information finns i [Konfigurera säkerhetsinställningar för system](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Följande är de högsta tillgängliga åtkomstinställningarna för objekt på åtkomstnivån Extern användare.

| Workfront objekttyp | Ingen åtkomst | Visa åtkomst | Redigera åtkomst |
|---|---|---|---|
| Projekt | ✓ |   |   |
| Uppgift | ✓ | ✓ |   |
| Problem | ✓ |   |   |
| Portfolio | ✓ |   |   |
| Program | ✓ |   |   |
| Rapporter (inklusive instrumentpaneler och kalenderrapporter) |   | ✓ (Endast för kalenderrapporter. ingen möjlighet att dela rapporter) |   |
| Filter, vyer och grupperingar | ✓ |   |   |
| Dokument |   | ✓ (utan möjlighet att dela dokument) |   |
| Användare |   | ✓ |   |
| Mall | ✓ |   |   |
| Finansiella uppgifter | ✓ |   |   |
| Resurshantering | ✓ |   |   |
| Scenarioplan | ✓ |   |   |
| Workfront-mål | ✓ |   |   |
