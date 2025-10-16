---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Konfigurera om tid är inloggad i timmar eller dagar
description: Som användare med en planlicens kan du konfigurera om du ska logga in i Adobe Workfront i timmar eller dagar. Systemadministratörer kan konfigurera den här inställningen för enskilda användare eller för flera användare i organisationen. Som standard loggar användarna tid i timmar.
author: Lisa
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b0a3a11a3c04a0969bee99f8e1cea231911f0e6a
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 0%

---

# Konfigurera om tid är inloggad i timmar eller dagar

Som användare med en Standard- eller Plan-licens kan du konfigurera om du ska logga in i Adobe Workfront i timmar eller dagar. Systemadministratörer kan konfigurera den här inställningen för enskilda användare eller för flera användare i organisationen. Som standard loggar användarna tid i timmar. Mer information om hur du loggar tid i Workfront finns i [Loggtid](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Vi rekommenderar loggningstid på samma sätt, antingen timmar eller dagar, i hela organisationen för att säkerställa att rapporteringen är korrekt.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td><p>Standard- och Plan-användare kan konfigurera tiden för sig själva. Endast en Workfront-administratör kan konfigurera tiden för andra användare.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

1. Gör något av följande, beroende på ditt mål och din åtkomstnivå i systemet:

   * **Standardanvändare eller plananvändare som konfigurerar tidsloggning för sig själv:** Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på ditt användarnamn bredvid din profilbild. Eller (om det är tillgängligt) klicka på din profilbild i det övre navigeringsområdet och klicka sedan på **[!UICONTROL Workfront Profile]**. Klicka sedan på ikonen **Mer** bredvid ditt namn och välj **Redigera**.

   * **Systemadministratören konfigurerar tidsloggning för andra:** Börja redigera ett eller flera användarkonton, enligt beskrivningen i [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. I den dialogruta som visas letar du reda på alternativet **Loggtid in** i avsnittet **Resursplanering**.

   ![Logga in med alternativ](assets/user-profile-log-time-options.png)

1. Välj bland följande alternativ för loggningstid:

   | Alternativ | Beskrivning |
   |---|---|
   | **Timmar** | Användarna anger timmar vid loggning i Workfront. |
   | **Dagar** | Användarna anger dagar när de loggar in i Workfront. |

1. (Villkorligt) Om du har valt att logga tid i dagar skriver du antalet timmar som motsvarar en heldag i fältet **Motsvarande timmar för Fullständig Workday**. En dag på en användares tidrapport motsvarar det antal timmar du anger här.

   Tänk på följande när du konfigurerar den här inställningen:

   * Det här alternativet är inte tillgängligt när du konfigurerar loggningstiden i timmar.
   * Det här alternativet används endast för loggningstid. Det här alternativet är inte relaterat till alternativet **Schema** som också är tillgängligt när du redigerar en användare. Alternativet **Schema** används vid beräkning av tidslinjer och i andra områden av Workfront. (Mer information om hur du använder alternativet **Schema** finns i [Skapa ett schema](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).) 

1. Klicka på **Spara ändringar**.
