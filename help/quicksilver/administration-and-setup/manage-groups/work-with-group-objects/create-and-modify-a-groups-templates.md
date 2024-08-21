---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Skapa och ändra en grupps projektmallar
description: När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med projektmallar som är kopplade till gruppen och dess undergrupper.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 0%

---

# Skapa och ändra en grupps projektmallar

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med projektmallar som är kopplade till gruppen och dess undergrupper.

Om det finns grupper ovanför gruppen kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst eller senare för de mallar du vill visa och arbeta med</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

+++

## Visa, arbeta med och skapa mallar för din grupp i området Grupper

{{step-1-to-setup}}

1. Klicka på **Grupper** ![](assets/groups-icon.png) i den vänstra panelen.

1. Klicka på namnet på gruppen som du vill skapa eller ändra mallar för.
1. Klicka på **Mallar** i den vänstra panelen för att visa de mallar som är kopplade till gruppen och till eventuella undergrupper.

   Du måste ha behörigheten Visa för en mall för att kunna se den i den här listan. Mer information om den här åtkomsten finns i [Bevilja åtkomst till mallar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Gör något av följande:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Lägga till en mall</td> 
      <td> <p>Klicka på <strong>Ny mall</strong> och konfigurera den sedan med de tillgängliga alternativen. Mer information om de här alternativen finns i <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Skapa en projektmall</a>.</p> <p>Mallen kopplas automatiskt till gruppen.</p> <p>Mer information om hur gruppinställningar gäller för nya mallar finns i <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Hur inställningar gäller för mallar och malluppgifter</a> i den här artikeln.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Redigera en eller flera mallar</td> 
      <td> <p>Välj minst en mall, klicka på ikonen Redigera <img src="assets/edit-icon.png"> och använd sedan något av de tillgängliga alternativen för att konfigurera den. Mer information om de här alternativen finns i <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Redigera projektmallar</a>.</p> <p>Ikonen Redigera är bara tillgänglig om du har behörighet att redigera till alla mallar du väljer. Mer information om den här åtkomsten finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Bevilja åtkomst till mallar</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ta bort en eller flera mallar</td> 
      <td> <p>Välj minst en mall och klicka sedan på ikonen Ta bort <img src="assets/delete.png">.</p> <p>Den här ikonen är bara tillgänglig om du har redigeringsåtkomst till alla mallar som du väljer. Mer information om den här åtkomsten finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Bevilja åtkomst till mallar</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dela en eller flera mallar</td> 
      <td> <p>Välj minst en mall, klicka på delningsikonen <img src="assets/share-icon.png"> och klicka sedan på något av följande alternativ i listrutan:</p> 
       <ul> 
        <li> <p><strong>Mall</strong>: I rutan <strong>Mallåtkomst</strong> som visas lägger du till namn för att ange vilka du vill ha åtkomst till själva mallen.</p> <p>Mer information finns i avsnittet <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Dela en mall</a> i artikeln <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Dela projektmallar</a>.</p> </li> 
        <li><strong>Projekt</strong>: I rutan <strong>Projektåtkomst</strong> som visas lägger du till namn för att ange vilka du vill ha åtkomst till projekt som skapats från mallen</li> 
       </ul> <p>Ikonen Dela är bara tillgänglig om du har delningsåtkomst till alla mallar du väljer. Mer information om den här åtkomsten finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Bevilja åtkomst till mallar</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exportera listan med mallar</td> 
      <td>Klicka på <strong>Exportera</strong> <img src="assets/export.png"> och välj sedan det filformat som du vill använda för den exporterade listan.</td> 
     </tr> 
    </tbody> 
   </table>

## Hur inställningar gäller för mallar och malluppgifter {#how-preferences-apply-to-templates-and-template-tasks}

När du skapar en projektmall konfigureras inställningarna som anges i tabellerna nedan automatiskt av en korrelerande projekt- eller uppgiftsinställning.

>[!NOTE]
>
>Ett projekt på gruppnivå eller på systemnivå eller en uppgiftsinställning påverkar en projektmall, beroende på om du kopplade mallen till en grupp när du skapade den.
>
>Om du har associerat den med en grupp träder inställningen på gruppnivå i kraft. Detta inträffar i följande scenarier:
>
>* Du skapar mallen från området Grupper, vilket förklaras i den här artikeln
>* Du anger en grupp när du skapar mallen med hjälp av en snabbstartfil
>* Du anger en grupp när du skapar mallen med API:t
>
>Om du inte har kopplat den nya mallen till en grupp börjar inställningarna på systemnivå gälla. Detta inträffar i scenarierna nedan. (Om du senare tilldelar en grupp till mallen eller malluppgiften påverkar inte gruppens inställningar den.)
>
>* Du skapar mallen från området Mallar
>* Du anger ingen grupp när du skapar mallen med hjälp av en Kickstart-fil
>* Du anger ingen grupp när du skapar mallen med API:t
>

* [Projektmallsinställningar som konfigurerats av projekt- och uppgiftsinställningar](#project-template-settings-configured-by-project-and-task-preferences)
* [Malluppgiftsinställningar som konfigurerats av uppgiftsinställningarna](#template-task-settings-configured-by-task-preferences)

### Projektmallsinställningar som konfigurerats av projekt- och uppgiftsinställningar {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Resultatindexmetod</p> </td> 
   <td> <p>Konfigureras av projektinställningen "Resultatindexmetod" på gruppnivå om du kopplar den nya mallen till en grupp, eller samma projektinställning på systemnivå om du inte gör det.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Villkorstyp</p> </td> 
   <td> <p>Konfigureras av projektinställningen på gruppnivå"Ange automatiskt projektvillkor baserat på status för förlopp" om du kopplar den nya mallen till en grupp, eller samma projektinställning på systemnivå om du inte gör det.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Schemalägg från</p> </td> 
   <td> <p>Konfigureras av projektinställningen "Schemalägg från" på gruppnivå om du associerar den nya mallen med en grupp, eller samma projektinställning på systemnivå om du inte gör det.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Användaren är ledig</p> </td> 
   <td> <p>Konfigureras av projektinställningen på gruppnivå,"användartid av", om du kopplar den nya mallen till en grupp, eller samma projektinställning på systemnivå om du inte gör det.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Uppdateringstyp</p> </td> 
   <td> <p>Konfigureras av projektinställningen på gruppnivå"Projekttidslinjer omberäknas automatiskt" om du associerar den nya mallen med en grupp, eller med samma projektinställning på systemnivå om du inte gör det.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Inställningar för åtkomstsektion</p> </td> 
   <td> <p>Konfigureras av aktivitetsinställningarna på gruppnivå i avsnittet Åtkomst om du associerar den nya mallen med en grupp, eller samma projektinställning på systemnivå om du inte gör det.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om projektinställningarna i den här tabellen finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Mer information om inställningar för aktivitet och problem finns i [Konfigurera inställningar för åtgärd och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Om du ändrar gruppen som är kopplad till en befintlig projektmall ändras inte mallens inställningar.
>* Om du flyttar en befintlig malluppgift till en annan mall förblir följande inställningar oförändrade i malluppgiften, oavsett vilken grupp som är associerad med den nya mallen:>
>   * Varaktighetstyp
>   * Intäktstyp
>   * Kostnadstyp
>
>  Malluppgiften påverkas dock av inställningen &quot;När någon tilldelas till en uppgift&quot; i den nya mallen. Mer information finns i avsnittet [Åtkomst](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) i artikeln [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* När en administratör sparar ett projekt som en mall ärvs alla inställningar för mallen från projektet, inklusive gruppen.
>
>  När en administratör konverterar en uppgift eller ett problem till ett projekt med hjälp av en mall, bestäms alla inställningar för mallen av vad som redan har sparats i mallen.
>

### Malluppgiftsinställningar som konfigurerats av uppgiftsinställningarna {#template-task-settings-configured-by-task-preferences}

När du skapar en malluppgift konfigureras vissa av dess inställningar automatiskt av en motsvarande uppgiftsinställning. De här inställningarna visas i tabellen nedan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Varaktighetstyp </p> </td> 
   <td> <p>Konfigureras av aktivitetsinställningen "Varaktighetstyp" på gruppnivå om du kopplar mallen till en grupp, eller av samma åtgärd och utleveransinställning på systemnivå om du inte gör det.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Intäktstyp</p> </td> 
   <td> <p>Konfigureras av aktivitetsinställningen "Inkomsttyp" på gruppnivå om du associerar mallen med en grupp, eller av samma åtgärd och utleveransinställning på systemnivå om du inte gör det.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Kostnadstyp </p> </td> 
   <td> <p> Konfigureras av uppgiftsinställningen Kostnadstyp på gruppnivå om du kopplar mallen till en grupp, eller av samma åtgärd och utleveransinställning på systemnivå om du inte gör det.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om uppgiftsinställningarna som anges i den här tabellen finns i [Konfigurera inställningar för aktiviteter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
