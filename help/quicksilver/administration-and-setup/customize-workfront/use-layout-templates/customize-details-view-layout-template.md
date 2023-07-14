---
title: Anpassa detaljvyn med hjälp av en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Som Workfront-administratör kan du använda en layoutmall för att avgöra vilken information som visas när en användare väljer detaljavsnittet i den vänstra panelen när han eller hon visar en uppgift, ett problem, ett dokument, ett program eller en portfölj.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Anpassa detaljvyn med hjälp av en layoutmall

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Som Adobe Workfront-administratör kan du använda en layoutmall för att bestämma vilken information som ska visas när en användare klickar på ikonen Detaljer ![](assets/project-details-icon.png) i den vänstra panelen när du visar en uppgift, ett problem, ett dokument, ett program eller en portfölj.

<!--
or billing record
-->

Du kan också ändra ordningen på den information som informationen visas i. För alla uppgifter som användarna ser kan du till exempel flytta anpassad Forms-information högst upp i detaljvyn för alla uppgifter som användarna ser.

Mer information om hur du skapar layoutmallar finns i [Skapa och hantera layoutmallar](../use-layout-templates/create-and-manage-layout-templates.md).

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

När du har konfigurerat en layoutmall måste du tilldela den till användare för att de ändringar du har gjort ska kunna visas för andra. Mer information om hur du tilldelar en layoutmall till användare finns i [Tilldela användare till en layoutmall](../use-layout-templates/assign-users-to-layout-template.md).

De ändringar du gör i detaljvyn för ett objekt avgör också tillgängligheten och ordningen för fält som användarna ser i följande områden:

* rutor för&quot;nytt objekt&quot;, t.ex. Ny uppgift och Nytt problem

  ![](assets/new-task-dialog.png)

* Skärmar som&quot;Redigera objekt&quot;, till exempel Redigera aktivitet, Redigera problem och Redigera projekt

  ![](assets/edit-task-screen.png)


* &quot;Redigera objekt&quot; skärmar när flera objekt redigeras samtidigt. För närvarande stöds detta för att redigera flera projekt samtidigt.

  ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* Sammanfattning ![](assets/summary-panel-icon.png) panel för listor över uppgifter och problem

  ![](assets/summary-area.png)

  >[!NOTE]
  >
  >Ändringar av layoutmallarna påverkar bara ordningen och tillgängligheten för fält på panelen Sammanfattning för de uppgifter och ärenden som tilldelats den inloggade användaren.

* Konverteringsrutor, som Konvertera till uppgift eller Konvertera till projektrutor.

  ![Konvertera problem till aktivitetsruta](assets/convert-issue-to-task-box.png)

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Åtkomstkrav

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
   <td> <p>För att kunna utföra dessa steg på systemnivå måste du ha åtkomstnivån Systemadministratör.
Om du vill utföra dem för en grupp måste du vara gruppchef</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassa det som användarna ser i detaljvyn

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicka på nedpilen ![](assets/dropdown-arrow-12x12.png) under **Anpassa det användarna ser** och sedan klicka **Projekt**, **Uppgift**, **Problem**, **Program**, eller **Portfolio.**
<!--
, or billing record
-->

1. I **Detaljer** gör du något av följande för att anpassa vad användarna ser i detaljvyn:

   * Dra avsnittsrubriker ![](assets/move-icon---dots.png) för att ändra deras ordning.
   * Aktivera eller inaktivera alternativ under **Översikt** och **Anpassad Forms** för att visa eller dölja dem.

     Om du döljer alla fält i ett av dessa avsnitt, döljs hela avsnittet.

     Alla fält är aktiverade som standard.

1. Fortsätt att anpassa layoutmallen.

   eller

   Om du är klar med anpassningen klickar du på **Spara**.

   >[!TIP]
   >
   >Du kan klicka på Spara när som helst för att spara förloppet och sedan fortsätta att ändra mallen senare.
