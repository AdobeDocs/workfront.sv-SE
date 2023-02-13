---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Konfigurera om tid är inloggad i timmar eller dagar
description: Som användare med en planlicens kan du konfigurera om du ska logga in i Adobe Workfront i timmar eller dagar. Systemadministratörer kan konfigurera den här inställningen för enskilda användare eller för flera användare i organisationen. Som standard loggar användarna tid i timmar.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Konfigurera om tid är inloggad i timmar eller dagar

Som användare med en planerarlicens kan du konfigurera om du ska logga in i Adobe Workfront i timmar eller dagar. Systemadministratörer kan konfigurera den här inställningen för enskilda användare eller för flera användare i organisationen. Som standard loggar användarna tid i timmar. Mer information om hur du loggar tid i Workfront finns i [Loggtid](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Vi rekommenderar loggningstid på samma sätt, antingen timmar eller dagar, i hela organisationen för att säkerställa att rapporteringen är korrekt.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Planerare kan konfigurera tiden för sig själva. Endast en Workfront-administratör kan konfigurera tiden för andra användare.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

1. Gör något av följande, beroende på ditt mål och din åtkomstnivå i systemet:

   * **Planeraranvändare konfigurerar tidsloggning för sig själv:** Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på ditt användarnamn bredvid din profilbild. Klicka sedan på **Mer** -ikon bredvid ditt namn och välj **Redigera**.

   * **Systemadministratören konfigurerar tidsloggning för andra:** Börja redigera ett eller flera användarkonton enligt beskrivningen i [Redigera en användares profil](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. I den dialogruta som visas i dialogrutan **Resursplanering** -avsnittet, leta upp **Loggtid in** alternativ.

   ![](assets/new-timesheet-log-hours-350x249.png)

1. (Villkorligt) Om du är systemadministratör och redigerar flera användare samtidigt väljer du **Loggtid in**.
1. Välj bland följande alternativ för loggningstid:

   | Alternativ | Beskrivning |
   |---|---|
   | **Timmar** | Användarna anger timmar vid loggning i Workfront. |
   | **Dagar** | Användarna anger dagar när de loggar in i Workfront. |

1. (Villkorligt) Om du har valt att logga tid i dagar, i dialogrutan **Motsvarande antal timmar för fullständiga Workday** anger du antalet timmar som motsvarar en hel dag. En dag på en användares tidrapport motsvarar det antal timmar du anger här.

   Tänk på följande när du konfigurerar den här inställningen:

   * Det här alternativet är inte tillgängligt när du konfigurerar loggningstiden i timmar.
   * Det här alternativet används endast för loggningstid. Det här alternativet är inte relaterat till **Schema** som också är tillgängligt när du redigerar en användare. The **Schema** används vid beräkning av tidslinjer och i andra områden i Workfront. (Mer information om hur du använder **Schema** alternativ, se [Skapa ett schema](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).) 

1. Klicka **Spara ändringar**.
