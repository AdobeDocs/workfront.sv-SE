---
user-type: administrator
product-area: system-administration
navigation-topic: run-diagnostics
title: Använd diagnostik för att starta automatiserade processer
description: Du kan använda Diagnostik för att manuellt aktivera automatiserade processer, som tidsbaserade skript, omberäkningar eller e-postmeddelanden.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 9243ee60-006b-4628-bde7-5b037dde7511
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 0%

---

# Använd diagnostik för att starta automatiserade processer

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Du kan använda Diagnostik för att manuellt aktivera automatiserade processer, som tidsbaserade skript, omberäkningar eller e-postmeddelanden.

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
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Systemadministratör</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Använd diagnostik för att starta automatiserade processer

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på ikonen **Konfigurera** ![Nätövertoningsinställningar](assets/gear-icon-settings.png) .

1. Expandera **System** och klicka sedan på **Diagnostik**.
1. Välj något av följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Skicka förfallna meddelanden</td> 
      <td> <p>Skickar automatiskt påminnelsemeddelanden manuellt för förfallna uppgifter och problem. </p> <p>Mer information om hur du ställer in automatiska påminnelser finns i <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Konfigurera automatiska påminnelser</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Skicka tidiga meddelanden</td> 
      <td> <p>Skickar automatiskt påminnelsemeddelanden manuellt för uppgifter och ärenden som närmar sig förfallodatum.</p> <p>Mer information om hur du ställer in automatiska påminnelser finns i <a href="../../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md" class="MCXref xref">Konfigurera automatiska påminnelser</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Skicka påminnelsemeddelanden</td> 
      <td> <p>Skickar påminnelsemeddelanden manuellt. </p> <p>Mer information om hur du ställer in påminnelsemeddelanden finns i <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Konfigurera påminnelsemeddelanden</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kontrollera alla POP-konton</td> 
      <td>Kontrollerar om det finns nya e-postmeddelanden som har skickats till POP-konton som är länkade till Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beräkna om tidslinjer</td> 
      <td> <p>Beräknar om tidslinjen för alla projekt i Workfront som har statusen Aktuell. </p> <p>Mer information om hur du beräknar tidslinjen för projekt automatiskt eller manuellt finns i <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">Beräkna om projekttidslinjer</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Återställ standardkundrapporter</td> 
      <td>Återställer standardrapporterna som ursprungligen levererades med Workfront, så att de visas i avsnittet <strong>Rapporter</strong> för alla användare.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Generera tidrapporter</td> 
      <td>Skapar tidrapporter för användare baserat på deras återkommande tidrapportprofiler. Det här alternativet behöver bara köras om tidrapportprofilen har ändrats avsevärt efter att den har tilldelats användare, och endast efter att aktuella och framtida tidrapporter har tagits bort.</td> 
     </tr> 
    </tbody> 
   </table>
