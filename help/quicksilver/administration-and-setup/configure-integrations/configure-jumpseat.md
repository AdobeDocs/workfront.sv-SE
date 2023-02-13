---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Konfigurera JumpSeat-integrering
description: Ni kan integrera [!DNL JumpSeat] med [!DNL Workfront] för att ta fram skräddarsydd produktvägledning.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 2%

---

# Konfigurera JumpSeat-integrering

Ni kan integrera [!DNL JumpSeat] med [!DNL Workfront] för att ta fram skräddarsydd produktvägledning.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Produkt</strong></td> 
   <td>Du måste ha en aktiv [!DNL JumpSeat] plan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p> Du måste vara en [!DNL Workfront] administratör. För information om [!DNL Workfront] administratörer, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Förutsättningar

Innan du börjar måste du

* Lägg till och aktivera [!DNL Workfront] som ett program i [!DNL JumpSeat]. Mer information finns i [Lägga till eller ta bort ett program](https://support.jumpseat.io/article/how-to-add-an-application/).

## Konfigurera [!DNL JumpSeat] integration

Vi rekommenderar att du skapar en [!DNL JumpSeat] integrering i både förhandsgransknings- och produktionsmiljöer.

>[!TIP]
>
>Du måste lägga till och aktivera två separata [!DNL Workfront] program i [!DNL JumpSeat]- en för Preview och en för Production. Se [Lägga till eller ta bort ett program](https://support.jumpseat.io/article/how-to-add-an-application/) för mer information.

Så här konfigurerar du [!DNL JumpSeat] integrering:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Setup]**.
1. Klicka på i den vänstra panelen **[!UICONTROL System]** > **[!UICONTROL [!DNL JumpSeat] Integration]**.
1. Ange **[!UICONTROL [!DNL JumpSeat] URL]**.

   **Exempel:** [!DNL https]://{mycompany name}.hoppseat.io

1. Ange **[!UICONTROL [!DNL JumpSeat] integration token]**. Du hittar den här på **[!UICONTROL Configuration]** sida in [!DNL JumpSeat].

   **Exempel:** $2 y$10$BevsKeQ8....OYR.LurSg2U64O

1. Klicka på **[!UICONTROL Test configuration]**.
1. Välj om du vill att integreringen ska vara **[!UICONTROL Active]** eller **[!UICONTROL Inactive]**.

   >[!IMPORTANT]
   >
   >Konfigurationstestet som utförs i steg 5 måste gå igenom för att integreringen ska aktiveras.

   ![JumpSeat Integration page](assets/jumpseat-integration-page.png)

1. Klicka på **[!UICONTROL Save]**.
