---
title: Anpassa nytt hem med en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Du kan använda en layoutmall för att konfigurera vad användarna ser när de öppnar nya Hem.
author: Nolan
feature: System Setup and Administration
role: Admin
source-git-commit: dad055b0901cfa8114f7f6b13b6f689d70b31205
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# Anpassa nytt hem med en layoutmall

Du kan använda en layoutmall för att konfigurera vad användarna ser när de öppnar nya Hem.

Du kan konfigurera

* Vilka widgetar som visas på arbetsytan som standard och deras layout på sidan
* Vilken bakgrund är markerad
* Specifika widgetinställningar, inklusive vilka filter och grupper som är tillgängliga för widgetarna Mina projekt, Mina uppgifter och Mina problem, samt deras standardvärden

>[!IMPORTANT]
>
>Administratörslayoutmallens val som beskrivs på den här sidan åsidosätter enskilda användares anpassningsalternativ.
>
>När ändringar i en layoutmall sparas ändras den nya startsidan för användare som använder den layoutmallen så att den matchar layoutmallen, och deras befintliga widgetval flyttas längst ned på sidan. Widgetar som valts av administratören kan flyttas och storleksändras av en användare, men de kan inte tas bort.

Mer information om nya Home finns i [Kom igång med Nytt hem](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

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
Om du vill utföra dem för en grupp måste du vara chef för den gruppen.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassa nytt hem med en layoutmall

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klicka på nedpilen ![](assets/dropdown-arrow.png) under **Anpassa det användarna ser** och sedan klicka **Arbetsytan Hem**.

1. Klicka på någon av flikarna till höger **Design och layout** för att välja och ordna widgetar och bakgrund, eller **Widget-inställningar** om du vill hantera inställningar för enskilda widgetar, till exempel tillgängliga filter och grupper.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Design och layout</td> 
      <td>
      <p>Välj vilka widgetar som ska finnas på användarens arbetsytor, deras position och välj en bakgrund. Observera att även om användare inte kan ta bort de markerade widgetarna kan de flytta och ändra storlek på dem fritt samt lägga till ytterligare widgetar.</p>
      <p>Den här fliken fungerar i stort sett som en liten ny hemarbetsyta, och kan därför anpassas enligt stegen som beskrivs i <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Lägga till, redigera eller ta bort widgetar i nytt hem</a>. Välj widgetar och ordna arbetsytan så som du vill att den ska visas för användarna.</p>
      <p>Om du vill ändra bakgrunden följer du stegen under <b>Anpassning av bakgrund</b> in <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">Kom igång med Nytt hem</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Widget-inställningar</td> 
      <td>
      <p>Ändra inställningar för enskilda widgetar. För närvarande stöds endast tre widgetar:</p>
      <ul>
        <li>Mina projekt</li>
        <li>Mina uppgifter</li>
        <li>Mina problem</li>
      </ul>
      <p>När du har valt den widget du vill redigera visas tillgängliga alternativ till höger. För närvarande är dessa alternativ <b>Filter</b> och <b>Grupper</b>. Du kan:</p>
      <ul>
        <li><b>Välj vilka filter eller grupper som ska vara tillgängliga för användarna:</b><p>Markera rutan bredvid alla alternativ i listan som du vill att användarna ska kunna använda. Alternativen som inte är markerade visas inte för användare.</li></p>
        <li><b>Ange ett standardfilter eller en standardgrupp för widgeten:</b><p>Håll muspekaren över ett alternativ så visas en knapp som gör att du kan ange det alternativet som standard för användarna. Den aktuella standardinställningen kommer att ha ett blått standardmärke till höger.</li></p>
        <li><b>Lägg till ett befintligt filter eller en befintlig grupp i listan med tillgängliga alternativ:</b><p>Klicka på plustecknet längst ned i varje lista för att lägga till ett alternativ i den listan. Observera att endast befintliga filter eller grupper kan läggas till på det här sättet.</li></p>
      </ul>
      </td> 
     </tr>
    </tbody> 
   </table>

>[!IMPORTANT]
>
>Om du anger ett standardfilter eller en gruppering för en viss widget med hjälp av en layoutmall kanske det inte börjar gälla omedelbart på grund av befintliga användarinställningar. Om du vill använda det nya filtret eller grupperingen direkt kan du eller användaren behöva återställa sina användarinställningar genom att lägga till &quot;/resetUser&quot; i slutet av URL:en.

1. Fortsätt att anpassa layoutmallen.

   eller

   Om du är klar med anpassningen klickar du på **Spara** längst ned till vänster.

