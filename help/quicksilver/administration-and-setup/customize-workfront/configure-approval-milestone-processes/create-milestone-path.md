---
title: Skapa en milstolpe-bana
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Som Adobe Workfront-administratör kan du skapa milstolpar som sedan kan användas i alla projekt i systemet. De ändringar du gör i milstolpbanorna i det här området påverkar hela Workfront-systemet.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# Skapa en milstolpe-bana

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Som Adobe Workfront-administratör kan du skapa milstolpar som sedan kan användas i alla projekt i systemet. De ändringar du gör i milstolpbanorna i det här området påverkar hela Workfront-systemet.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Milstolpar och milstolpar

Du kan koppla nyckelåtgärderna i ett projekt till fördefinierade milstolpar. Den här funktionen kan ge chefer och andra intressenter en översikt över hur ett projekt fortskrider.

Summan av alla fördefinierade milstolpar kallas för en milstolpe-bana.

Det första steget i att bygga en milstolpe är att identifiera vilka milstolparna är och att fastställa milstolparna. Eftersom du kan koppla en milstolpe-väg till flera projekt måste milstolpen vara allmänna faser eller faser i alla projekt.

Mer information om hur du associerar en milstolpe-bana med ett projekt och en milstolpe med en uppgift finns i [Koppla milstolpar till uppgifter](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Skapa en milstolpe-bana

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Processer** > **Milstolpbanor**.
1. Klicka **Ny milstolpe-sökväg.**
1. Ange följande information i dialogrutan **Grundläggande information** område:

   <table style="table-layout:auto">
    <tr>
      <td>Sökväg för milstolpe</td>
       <td>Ange ett namn för milstolpebanan.</td>
    </tr>
    <tr>
      <td>Beskrivning</td>
      <td>Ange en beskrivning för att definiera milstolpebanan.</td>
    </tr>
    <tr>
       <td>Är aktiv</td>
      <td>Markera den här kryssrutan om du vill att milstolpen ska vara aktiv. Andra användare kan hitta den här sökvägen och bifoga den till projekt när de skapar eller redigerar projekt. Det går inte att koppla inaktiva milstolpesökvägar till projekt. Detta är aktiverat som standard.</td>
    </tr>
    <tr>
      <td>Grupper</td>
      <td>Markera de grupper som visas så att användare i de här grupperna kan se och använda den här milstolpen i sina projekt. Hemgruppen för den användare som anger milstolpen är markerad som standard.</td>
    </tr>
   </table>

1. Ange följande information i dialogrutan **Milstolpar** område:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td>Skriv beskrivande namn för varje milstolpe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Ange en beskrivning för milstolpen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Färg</td> 
      <td> <p>Välj en färg som du vill associera med din milstolpe. </p> <p>Om du inte väljer någon färg väljs den senaste färgen som användes i en milstolpe-bana. Vi rekommenderar att du väljer en unik färg för varje milstolpe. Färgen används för visuella ändamål och för rapportering.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Lägg till milstolpe** och fortsätta lägga till milstolpar efter behov tills banan är klar.
1. Klicka **Skapa milstolpe-sökväg** för att spara ändringarna.

   Din milstolpe-väg är klar att kopplas till ett projekt.

   Mer information om hur du kopplar milstolpar till projekt och milstolpar till uppgifter finns i [Koppla milstolpar till uppgifter](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).
