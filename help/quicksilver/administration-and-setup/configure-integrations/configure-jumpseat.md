---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Konfigurera JumpSeat-integrering
description: Du kan integrera [!DNL JumpSeat] med [!DNL Workfront] för att skapa anpassad produktvägledning.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Nolan, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Konfigurera JumpSeat-integrering

Du kan integrera [!DNL JumpSeat] med [!DNL Workfront] för att skapa anpassad produktvägledning.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Du måste ha en aktiv [!DNL JumpSeat]-plan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p> Du måste vara en [!DNL Workfront]-administratör. Mer information om [!DNL Workfront] administratörer finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

+++

## Förutsättningar

Innan du börjar måste du

* Lägg till och aktivera [!DNL Workfront] som ett program i [!DNL JumpSeat]. Mer information finns i [Lägga till eller ta bort ett program](https://support.jumpseat.io/article/how-to-add-an-application/).

## Konfigurera integreringen av [!DNL JumpSeat]

Vi rekommenderar att du konfigurerar en [!DNL JumpSeat]-integrering i både förhandsgransknings- och produktionsmiljöer.

>[!TIP]
>
>Du måste lägga till och aktivera två separata [!DNL Workfront]-program i [!DNL JumpSeat] - ett för Förhandsgranska och ett för Produktion. Mer information finns i [Lägga till eller ta bort ett program](https://support.jumpseat.io/article/how-to-add-an-application/).

Så här konfigurerar du integreringen av [!DNL JumpSeat]:

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL System]** > **[!UICONTROL [!DNL JumpSeat] Integration]** i den vänstra panelen.
1. Ange din **[!UICONTROL [!DNL JumpSeat] URL]** som finns på din tilläggsikon i [!DNL JumpSeat].

   **Exempel:** [!DNL https]://{mycompanyname}.hoppseat.io

1. Ange **[!UICONTROL [!DNL JumpSeat] integration token]**. Du kan hitta detta på sidan **[!UICONTROL Configuration]** i [!DNL JumpSeat].

   **Exempel:** $2y$10$BevsKeQ8...OYR.LurSg2U64O

1. Klicka på **[!UICONTROL Test configuration]**.
1. Välj om du vill att integreringen ska vara **[!UICONTROL Active]** eller **[!UICONTROL Inactive]**.

   >[!IMPORTANT]
   >
   >Konfigurationstestet som utförs i steg 5 måste gå igenom för att integreringen ska aktiveras.

   ![JumpSeat-integreringssida](assets/jumpseat-integration-page.png)

1. Klicka på **[!UICONTROL Save]**.

>[!TIP]
>
>Mer information om hur du konfigurerar [!DNL JumpSeat]-integreringen finns i [!DNL JumpSeat]-dokumentationen för [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
