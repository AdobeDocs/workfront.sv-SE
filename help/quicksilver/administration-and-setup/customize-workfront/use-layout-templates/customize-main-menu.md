---
title: Anpassa huvudmenyn med hjälp av en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Som Adobe Workfront-administratör eller gruppadministratör kan du använda en layoutmall för att konfigurera de alternativ som användare ser när de öppnar huvudmenyn i Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Anpassa huvudmenyn med hjälp av en layoutmall

Som Adobe Workfront-administratör eller gruppadministratör kan du använda en layoutmall för att konfigurera de alternativ som användare ser när de öppnar huvudmenyn i Workfront:

![Alternativ på huvudmenyn](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>De alternativ på huvudmenyn som användarna ser beror på licenstypen och vilka inställningar som har konfigurerats på åtkomstnivån. Vissa användare som kommer att använda den här layoutmallen kanske inte ser alla alternativ som du väljer här. Mer information finns i [Hur åtkomstnivåer och behörigheter fungerar tillsammans](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) och [Konfigurerbar åtkomst till funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Mer information om hur du skapar layoutmallar finns i [Skapa och hantera layoutmallar](../use-layout-templates/create-and-manage-layout-templates.md).

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

När du har konfigurerat en layoutmall måste du tilldela den till användare för att de ändringar du har gjort ska kunna visas för andra. Mer information om hur du tilldelar en layoutmall till användare finns i [Tilldela användare till en layoutmall](../use-layout-templates/assign-users-to-layout-template.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront</strong></td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens</strong></td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>För att kunna utföra dessa steg på systemnivå måste du ha åtkomstnivån Systemadministratör.
Om du vill utföra dem för en grupp måste du vara gruppchef.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassa huvudmenyn

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicka **Ange huvudmeny** nära det övre högra hörnet.

   I rutan Huvudmeny som visas kan du se vilka alternativ som är aktiva på mallens huvudmeny samt vilka alternativ som är tillgängliga att lägga till. Följande är alla möjliga objekt som kan läggas till:

   * Startsida

     >[!TIP]
     >
     >Som standard visas Hem som Mina uppdateringar för användare med granskningslicens, såvida de inte har en layoutmall kopplad till sin profil som innehåller området Mina uppdateringar på huvudmenyn.

   * Portfolio
   * Program
   * Projekt
   * Rapporter
   * Kontrollpaneler
   * Kalendrar
   * Resurser
   * Scenarier

     >[!NOTE]
     >
     >Scenarioplaneraren finns endast i den nya Adobe Workfront-upplevelsen och kräver ytterligare en licens. Mer information om Workfront Scenario Planner finns i [Översikt över scenarioplanen](../../../scenario-planner/scenario-planner-overview.md).

   * Team
   * Användare

     >[!NOTE]
     >
     >Endast användare med en planlicens kan se Användare ![](assets/users-icon-in-main-menu.png) på huvudmenyn.

   * Begäranden
   * Tidrapporter
   * Dokument
   * Mallar
   * Analyser
   * Korrektur
   * Mål

     >[!NOTE]
     >
     >Detta kräver ytterligare en licens. Mer information om Workfront-mål finns på [Översikt över Adobe Workfront-mål](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * Mina uppdateringar
   * Varumärkena
   * Utkast

1. Gör något av följande:

   * Dölj ![](assets/remove-icon---x-in-circle.png) **Aktiva objekt** som du inte vill visa
   * Visa ![](assets/add-icon-plus-in-circle.png) **Tillgängliga objekt** som du vill visa på huvudmenyn.
   * Dra ![](assets/move-icon---dots.png) **Aktiva objekt** om du vill ändra deras visningsordning på huvudmenyn.

1. Klicka **Klar**.

   Du kan också klicka **Avbryt** om du vill ångra ändringarna.

1. Fortsätt att anpassa layoutmallen.

   eller

   Om du är klar med anpassningen klickar du på **Spara**.

   >[!TIP]
   >
   >Du kan klicka på Spara när som helst för att spara förloppet och sedan fortsätta att ändra mallen senare.

Mer information om layoutmallar finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
