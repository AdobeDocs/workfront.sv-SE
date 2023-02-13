---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Hantera timtyper
description: Du kan associera timtyper med timposterna. Timtyper är etiketter som du använder för att definiera timposterna.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# Hantera timtyper

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Du kan associera timtyper med timposterna. Timtyper är etiketter som du använder för att definiera timposterna.

Det finns två uppsättningar timtyper:

* **Projektspecifika timtyper**: Det här är tid för projekt, uppgifter och ärenden. Projektspecifika timtyper kan associeras med timtransaktioner var som helst i [!DNL Adobe Workfront] där du kan logga tid för projekt, uppgifter och problem.

   När du loggar in [!DNL Workfront], de projektspecifika timtyperna som är tillgängliga beror på konfigurationsalternativen som ställs in på system-, projekt- och användarnivå.

   Följande standardtyper av projektspecifika timmar är alltid tillgängliga:

   * Projekttid
   * Aktivitetstid
   * Utgivningstid

   The [!DNL Workfront] administratören avgör vilka projektspecifika timtyper som blir tillgängliga, enligt beskrivningen i [Definiera timtyper och tillgänglighet för tidrapporter](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   >[!NOTE]
   >
   >Om du aktiverar några projektspecifika timtyper i [!DNL Workfront] måste minst en projektspecifik timtyp aktiveras för varje projekt i systemet. Du kan inte aktivera en projektspecifik timtyp på systemnivå och har inga projektspecifika timtyper tillgängliga på projektnivå.

* **Typer av allmänna timmar**: Allmänna timmar kan inte associeras med ett projekt, en uppgift eller ett ärende och loggas direkt i en tidrapport. Mer information om loggningstid finns i [Loggtid](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Inbyggda timtyper

Workfront levereras med en uppsättning inbyggda timtyper. Dessa timtyper kan inte redigeras och kan inte döljas.

Timtyperna som medföljer [!DNL Workfront] är:

* **[!UICONTROL Sick Time]**: En allmän timtyp som inte kan associeras med timtransaktioner för ett projekt, en uppgift eller en utgåva.
* **[!UICONTROL Vacation Time]**: En allmän timtyp som inte kan associeras med timtransaktioner för ett projekt, en uppgift eller en utgåva.
* **[!UICONTROL General Overhead]**: En allmän timtyp som inte kan associeras med timtransaktioner för ett projekt, en uppgift eller en utgåva. Det kan dock räknas som intäkter i projektplaneringsprocessen.
* **[!UICONTROL Project Time]**: En allmän timtyp som bara kan associeras med timtransaktioner i ett projekt.
* **[!UICONTROL Task Time]**: En allmän timtyp som bara kan associeras med timtransaktioner för en aktivitet.
* **[!UICONTROL Issue Time]**:En allmän timtyp som bara kan associeras med timposter i en utgåva.

## Skapa timtyper

Som [!DNL Workfront] kan du skapa nya timtyper för din organisation på både system- och projektnivå. När du har skapat timtyper på system- och projektnivå kan användarna definiera vilka timtyper som är tillgängliga för specifika projekt och användare. Mer information finns i [Definiera timtyper och tillgänglighet för tidrapporter](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Så här skapar du nya timtyper:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe] Workfront, klicka sedan på **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicka på **[!UICONTROL Timesheet & Hours]** > **[!UICONTROL Hour Types]**.

1. Klicka på **[!UICONTROL New Hour Type].**
1. Ange följande information på **[!UICONTROL New Hour Type]** formulär:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Ge din nya timtyp ett namn som är lätt att känna igen i systemet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Lägg till en beskrivning av timtypen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Ange om timtypen är en allmän eller projektspecifik timtyp genom att välja rätt omfång i listrutan.</p> <p>Allmänna timtyper visas bara i tidrapporter och kan inte associeras med projekt, uppgifter eller problem.</p> <p><b>VIKTIGT</b>: Om du har en anpassad timtyp som är [!UICONTROL Project Specific]och sedan ändra den till [!UICONTROL General], ställs alla befintliga uppgifter, ärenden och projekttimmar in på systemets standardtyper.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count As Revenue]</td> 
      <td>Välj det här alternativet om du vill att timtransaktionen som är kopplad till den här timtypen ska påverka dina intäktsberäkningar.</td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Count As Revenue]**: Välj det här alternativet om du vill att timtransaktionen som är kopplad till den här timtypen ska påverka dina intäktsberäkningar.

1. Klicka på **[!UICONTROL Create Hour Type].**

## Inaktivera timtyper

Om timtyper blir inaktuella och du inte längre vill att användarna ska kunna koppla sina timuppgifter till dem kan du inaktivera timtyperna.

Inaktivering av timtyper döljer timtyperna var som helst i [!DNL Workfront] där timtyper visas.

Så här inaktiverar du en timtyp:

1. Klicka **[!UICONTROL Setup]** nära det övre högra hörnet av [!DNL Adobe Workfront] på det globala navigeringsfältet.

1. Expandera **[!UICONTROL Timesheet & Hours Preferences]** och sedan klicka **[!UICONTROL Hour Types]**.

1. Välj den timtyp som du vill inaktivera.

1. Klicka på **[!UICONTROL Deactivate]**.
