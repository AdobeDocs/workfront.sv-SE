---
title: Om Adobe Workfront standardlayout
user-type: administrator
content-type: reference;overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Standardlayouten är placeringen av huvudmenyn, den vänstra panelen samt vyerna, grupperingarna och filtren innan en Adobe Workfront-administratör gör några ändringar med hjälp av en layoutmall.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a68bca5e-1cec-432d-bb38-14b426a9c051
source-git-commit: 76797ce2afb6a6a929531f02ed3a3b3f75240602
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# Om Adobe Workfront standardlayout

Standardlayouten är placeringen av huvudmenyikonen ![Huvudmeny](assets/main-menu-icon.png) eller huvudmenyikonen ![Huvudmeny](assets/main-menu-icon.png) (om den är tillgänglig), den vänstra panelen och vyerna, grupperingarna och filtren innan en Adobe Workfront-administratör gör några ändringar med hjälp av en layoutmall.

Information om hur en Workfront-administratör kan ändra en användares standardlayout genom att tilldela användaren en layoutmall finns i [Tilldela användare till en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

>[!NOTE]
>
>Användarna kan ändra sin egen layout genom att redigera sina användarprofilsinställningar. Mer information finns i avsnittet [Inställningar](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#preferences) i [Konfigurera mina inställningar](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

## Standardmenyalternativ för varje licenstyp

Varje användares standardlayout beror på licenstypen. Vissa användare kanske inte ser vissa områden på huvudmenyn eller vissa alternativ på den vänstra panelen, beroende på vilken licenstyp de har tilldelats.

Det finns två typer av licenser som din organisation kan tilldela:

* Nya licenser
* Aktuella licenser

<!--rename the above if we change Current to Legacy-->

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

### Standardhuvudmeny för aktuella licenstyper

I följande tabell visas standardalternativen för Huvudmeny och vad som visas i den vänstra panelen för varje aktuell licenstyp:

<table class="tg"><thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">Område</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">Vänster panelobjekt</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">Systemadministratör</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">Planering</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">Arbetare</span></th>
    <th class="tg-1wig">Granskare</th>
    <th class="tg-1wig">Begärande</th>
    <th class="tg-1wig">Extern användare</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-0lax">Startsida</td>
    <td class="tg-0lax">Hem<br>Prioriteter</td>
    <td class="tg-0lax">✔ (standardstartsida)</td>
    <td class="tg-0lax">✔ (standardstartsida)</td>
    <td class="tg-0lax">✔ (standardstartsida)</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Projekt</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔ </td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Portföljer</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Program</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Rapporter</td>
    <td class="tg-0lax">Mina rapporter<br>Delade med mig<br>Alla rapporter</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔ (Delas med mig och Alla rapporter i den vänstra panelen)</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔ (Delas med mig och Alla rapporter i den vänstra panelen)</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Kontrollpaneler</td>
    <td class="tg-0lax">Mina instrumentpaneler<br>Delade instrumentpaneler<br>Alla instrumentpaneler<br>Kontrollpaneler på arbetsytan*</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Kalendrar</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Resurser</td>
    <td class="tg-0lax">Planering<br>Utjämning av arbetsbelastning<br>Användning<br>Resurspooler</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔ (Planering- och resurspooler i den vänstra panelen)</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Team</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Användare</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Begäranden</td>
    <td class="tg-0lax"><br>Utkast har skickats</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Tidrapporter</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Dokument</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Mallar</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Scenarier</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Varumärkena</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Utkast</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔ (Installationsfunktioner)</td>
    <td class="tg-0lax">✔ (endast funktioner för begäran)</td>
    <td class="tg-0lax">✔ (endast funktioner för begäran)</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Prioriteringar</td>
    <td class="tg-0lax">Hem<br>Prioriteter</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔<br></td>
  </tr>
  <tr>
    <td class="tg-0lax">Inställningar</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔ (begränsad funktionalitet)</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">Mina uppdateringar</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔ (standardstartsida)</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>

</tbody></table>

*Du måste vara registrerad i betaversionen av Canvas Dashboards för att kunna se det här området. Mer information finns i [Betaversionsinformation för arbetsytans kontrollpaneler](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

### Standardhuvudmeny för nya licenstyper

I följande tabell visas standardalternativen för Huvudmeny och vad som visas i den vänstra panelen för varje ny licenstyp:

<table class="tg"><thead>
  <tr>
    <th class="tg-fymr">Område</th>
    <th class="tg-fymr">Vänster panelobjekt</th>
    <th class="tg-fymr">Systemadministratör</th>
    <th class="tg-fymr">Standard</th>
    <th class="tg-fymr">Ljus</th>
    <th class="tg-fymr">Medarbetare</th>
    <th class="tg-fymr">Extern användare</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-0pky">Startsida</td>
    <td class="tg-0pky">Hem<br>Prioriteter</td>
    <td class="tg-0pky">✔ (standardstartsida)</td>
    <td class="tg-0pky">✔ (standardstartsida)</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ (standardstartsida)</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Projekt</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ </td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Portföljer</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Program</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Rapporter</td>
    <td class="tg-0pky">Mina rapporter<br>Delade med mig<br>Alla rapporter</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ (Delas med mig och alla rapporter i den vänstra panelen)</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Kontrollpaneler</td>
    <td class="tg-0pky">Mina instrumentpaneler<br>Delade instrumentpaneler<br>Alla instrumentpaneler<br>Kontrollpaneler på arbetsytan*</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Kalendrar</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Resurser</td>
    <td class="tg-0pky">Planering<br>Utjämning av arbetsbelastning<br>Användning<br>Resurspooler</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Team</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Användare</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Begäranden</td>
    <td class="tg-0pky"><br>Utkast har skickats</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Tidrapporter</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Dokument</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Mallar</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Scenarier</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Varumärkena</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Utkast</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ (Installationsfunktioner)</td>
    <td class="tg-0pky">✔ (endast funktioner för begäran)</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Prioriteringar</td>
    <td class="tg-0pky">Hem<br>Prioriteter</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔<br></td>
  </tr>
  <tr>
    <td class="tg-0pky">Inställningar</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔ (begränsad funktionalitet)</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">Mina uppdateringar</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ (standardstartsida)</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
</tbody></table>

*Du måste vara registrerad i betaversionen av Canvas Dashboards för att kunna se det här området. Mer information finns i [Betaversionsinformation för arbetsytans kontrollpaneler](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

<!--

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area</th> 
   <th> Left panel items </th> 
   <th> System Administrator</th> 
   <th> Planner </th> 
   <th>Worker</th> 
   <th>Reviewer</th> 
   <th>Requestor</th> 
   <th>External User</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2"><strong>Projects</strong> </td> 
   <td><strong>Projects</strong> </td> 
   <td>✔ <br>(Default landing area)</td> 
   <td><span style="font-weight: 400;"> ✔</span> <br>(Default landing area)</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Portfolios</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Reporting</strong> </td> 
   <td><strong>Reports</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dashboards</strong> </p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Calendars</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="5"><strong>People</strong> (renamed to <strong>Teams</strong> for users with a Work license)</td> 
   <td><strong>Teams</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>People</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Planning</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Scheduling</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Requests</strong> </td> 
   <td>New Request </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td><strong>Requests I've Submitted</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ <br>(Default landing area)</td> 
   <td>✔ <br>(Default landing area)</td> 
  </tr> 
  <tr> 
   <td><strong>All Requests</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Timesheet</strong> </td> 
   <td><strong>My Timesheets</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Timesheets I Approve</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>All Timesheets</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Documents</strong> </td> 
   <td>&nbsp;</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Setup</strong> </td> 
   <td>&nbsp;</td> 
   <td>✔ </td> 
   <td>Limited Functionality</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>
-->
