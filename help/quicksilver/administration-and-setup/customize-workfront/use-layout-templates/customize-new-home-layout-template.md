---
title: Anpassa startsidan med en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Du kan använda en layoutmall för att konfigurera vad användare ser när de öppnar Hem i Adobe Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '855'
ht-degree: 0%

---

# Anpassa startsidan med en layoutmall

Du kan använda en layoutmall för att konfigurera vad användarna ser när de först öppnar Home.

Du kan konfigurera

* Vilka widgetar som visas på arbetsytan som standard
* Vilken bakgrund är markerad
* Specifika widgetinställningar, inklusive vilka filter och grupper som är tillgängliga för widgetarna Mina projekt, Mina uppgifter och Mina problem, samt deras standardvärden

>[!IMPORTANT]
>
>Slutanvändare kan ändra sin bakgrund och ordna om widgetar på sidan när layoutmallen har tillämpats. De kan inte ta bort widgetar som ingår i en Workfront-administratör.
> 
>Administratörer kan lägga till nya widgetar för användare. Om en användare redan har anpassat sin widgetordning eller bakgrundsurval ändras dock inte dessa anpassningar.

Mer information om Hem finns i [Kom igång med Hem](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

Mer information om hur du skapar layoutmallar finns i [Skapa och hantera layoutmallar](../use-layout-templates/create-and-manage-layout-templates.md).

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

När du har konfigurerat en layoutmall måste du tilldela den till användare för att de ändringar du har gjort ska kunna visas för andra. Mer information om hur du tilldelar en layoutmall till användare finns i [Tilldela användare till en layoutmall](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td><p>Nytt: Standard</p>
  <p> Aktuell: Planera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>För att kunna utföra dessa steg på systemnivå måste du ha åtkomstnivån Systemadministratör.
Om du vill utföra dem för en grupp måste du vara chef för den gruppen.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anpassa startsidan med en layoutmall

Så här anpassar du startsidan med en layoutmall:

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klicka på nedpilen ![nedpilen](assets/dropdown-arrow.png) under **Anpassa det som visas för användarna** och klicka sedan på **Home Workspace**.

1. Klicka på något av följande på flikarna till höger:

   * **Design och layout**: Välj för att välja och ordna widgetar och bakgrunden
   * **Widgetinställningar**: Välj det här alternativet om du vill hantera inställningar för enskilda widgetar, till exempel tillgängliga filter och grupper.

   Följande tabell innehåller information om varje flik:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Design och layout</td> 
      <td>
      <p>Välj vilka widgetar som ska visas på användarens arbetsytor, deras position och välj en bakgrund.</p> 
      <p>Observera att även om användare inte kan ta bort de markerade widgetarna kan de flytta och ändra storlek på dem fritt. De kan också lägga till fler widgetar.</p>
      <p>Den här fliken fungerar i stort sett som en förhandsvisning av den arbetsyta i hemmet som användare med den här layoutmallen kommer att uppleva.</p> 
      <p> Gör något av följande: </p>
      <ul><li>Anpassa den här fliken enligt stegen som beskrivs i <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Lägg till, redigera eller ta bort widgetar i Hem</a>. </li>
      <li>Välj widgetar och ordna arbetsytan så som du vill att den ska visas för användarna.</li>
      <li>Om du vill ändra bakgrunden följer du stegen under <b>Bakgrundsanpassning</b> i <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">Kom igång med Hem</a>.</li></p>
      <p>

   >[!NOTE]
   >
   >Det är bara när du flyttar eller ändrar storlek på widgetar i layoutmallen som användarna inte behöver uppdatera sin layout på hemsidorna. Om du lägger till eller tar bort en widget kommer dock en uppdatering av användarnas sidor att utlösas.

   </p>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Widget-inställningar</td> 
      <td>
      <p>Ändra inställningar för enskilda widgetar.</p> 
      <p>

   >[!NOTE]
   >
   >Dessa alternativ sträcker sig inte till panelen Sammanfattning. Du måste konfigurera området på fliken Sammanfattning i layoutmallen.

   </p>
      <p> Välj bland följande widgetar från listan till vänster:</p>
      <ul>
        <li>Mina projekt</li>
        <li>Mina uppgifter</li>
        <li>Mina problem</li>
      </ul>
      <p>När du har valt den widget du vill redigera väljer du de <b>filter</b>, <b>kolumner</b> och <b>grupper</b> som du vill göra tillgängliga för Hem till höger.</p>
      <p> Du kan:</p>
      <ul>
      <li><p>Markera och sortera de filter, kolumner eller grupper som är tillgängliga för användare genom att markera rutan bredvid alternativen i listan. Alternativen som inte är markerade visas inte för användare.</p></li>
      <li> <p>Dra och släpp i listan för att ange en ordning.</p></li>
      <p>

   >[!IMPORTANT]
   >
   >* Alternativen Filter, Kolumner och Grupp är länkade till alternativen för listanpassning i layoutmallen. Ändringar som görs här gäller även för dessa inställningar.
   >* Användarna måste ha minst behörigheten Skapa för vyer för att administratörskolumnen ska kunna användas korrekt på hemsidorna.

   </p>
      <li><p>Ange ett standardfilter eller en standardgrupp för widgeten genom att hålla markören över ett alternativ och klicka på <b>Ange som standard</b>. Den aktuella standardinställningen visar ett blått <b>Default</b>-märke till höger om den.</p></li>
      <li><p>Lägg till ett befintligt filter, en kolumn eller en grupp i listan med tillgängliga alternativ genom att klicka på plustecknet längst ned i varje lista för att lägga till ett alternativ i listan. Observera att endast befintliga filter, fält (för kolumner) eller grupper kan läggas till på det här sättet.</p></li>
      </ul>
      <p>

   >[!NOTE]
   >
   >Om du anger ett standardfilter eller en gruppering för en viss widget med hjälp av en layoutmall kanske det inte börjar gälla omedelbart på grund av befintliga användarinställningar. Om du vill använda det nya filtret eller grupperingen direkt kan du eller användaren behöva återställa sina användarinställningar genom att lägga till &quot;/resetUser&quot; i slutet av URL:en.

   </p>
      </td> 
      </tr>
      </tbody> 
      </table>

1. Fortsätt att anpassa layoutmallen.

   eller

   Om du är klar med anpassningen klickar du på **Spara** i det nedre vänstra hörnet.

   >[!IMPORTANT]
   >
   >Användarna måste uppdatera hemsidan för att kunna se anpassningar från layoutmallen.
