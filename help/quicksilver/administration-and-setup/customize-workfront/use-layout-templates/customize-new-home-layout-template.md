---
title: Anpassa nytt hem med en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Du kan använda en layoutmall för att konfigurera vad användarna ser när de öppnar nya Hem.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 21e81e6395680e3ea7ffd05424217e5352fff0f6
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 0%

---

# Anpassa nytt hem med en layoutmall

Du kan använda en layoutmall för att konfigurera vad användarna ser när de öppnar nya Hem första gången.

Du kan konfigurera

* Vilka widgetar som visas på arbetsytan som standard
* Vilken bakgrund är markerad
* Specifika widgetinställningar, inklusive vilka filter och grupper som är tillgängliga för widgetarna Mina projekt, Mina uppgifter och Mina problem, samt deras standardvärden

>[!IMPORTANT]
>
>Slutanvändare kan ändra sin bakgrund och ordna om widgetar på sidan när layoutmallen har tillämpats. De kan inte ta bort widgetar som ingår i en Workfront-administratör.
> <br>
>Administratörer kan lägga till nya widgetar för användare. Om en användare redan har anpassat sin widgetordning eller bakgrundsurval ändras dock inte dessa anpassningar.



Mer information om nya Hem finns i [Kom igång med nya Hem](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

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

## Anpassa nytt hem med en layoutmall

Så här anpassar du Nytt hem med en layoutmall:

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klicka på nedpilen ![](assets/dropdown-arrow.png) under **Anpassa det som visas för användarna** och klicka sedan på **Home Workspace**.

1. På flikarna till höger klickar du antingen på **Design &amp; layout** för att välja och ordna widgetar och bakgrund, eller på **Widget-inställningar** för att hantera inställningar för enskilda widgetar som tillgängliga filter och grupper.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Design och layout</td> 
      <td>
      <p>Välj vilka widgetar som ska finnas på användarens arbetsytor, deras position och välj en bakgrund. Observera att även om användare inte kan ta bort de markerade widgetarna kan de flytta och ändra storlek på dem fritt samt lägga till ytterligare widgetar.</p>
      <p>Den här fliken fungerar i stort sett som en liten ny hemarbetsyta. Den kan därför anpassas enligt stegen som beskrivs i <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Lägg till, redigera eller ta bort widgetar i nytt hemgränssnitt</a>. Välj widgetar och ordna arbetsytan så som du vill att den ska visas för användarna.</p>
      <p>Om du vill ändra bakgrunden följer du stegen under <b>Anpassa bakgrunden</b> i <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">Kom igång med nytt hem</a>.</p>
      <p>

>[!NOTE]
>
>Det är bara när du flyttar eller ändrar storlek på widgetar i layoutmallen som användarna inte längre behöver uppdatera sin layout på hemsidorna. Om du lägger till eller tar bort en widget kommer dock en uppdatering av användarnas sidor att utlösas.

</p>
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
      <p>När du har valt den widget du vill redigera visas tillgängliga alternativ till höger. Dessa alternativ omfattar <b>Filter</b>, <b>Kolumner</b> och <b>Grupper</b>. Du kan:</p>
      <ul>
      <li><p><b>Välj och beställa filter, kolumner eller grupper som är tillgängliga för användarna:</b></p>
      <p>Markera rutan bredvid alla alternativ i listan som du vill att användarna ska kunna använda. Dessa alternativ sträcker sig inte till panelen Sammanfattning. Du måste konfigurera området på fliken Sammanfattning i layoutmallen. Alternativen som inte är markerade visas inte för användare. Dra och släpp i listan för att ange en ordning.</li></p>
      <p>

>[!IMPORTANT]
>
>Användarna måste ha minst behörigheten Skapa för vyer för att administratörskolumnen ska kunna användas korrekt på de nya hemsidorna.

</p>
      <li><p><b>Ange ett standardfilter eller en standardgrupp för widgeten:</b></p>
      <p>Håll muspekaren över ett alternativ så visas en knapp som gör att du kan ange det alternativet som standard för användarna. Den aktuella standardinställningen kommer att ha ett blått standardmärke till höger.</li></p>
      <li><p><b>Lägg till ett befintligt filter, en befintlig kolumn eller en grupp i listan med tillgängliga alternativ:</b></p>
      <p>Klicka på plustecknet längst ned i varje lista för att lägga till ett alternativ i den listan. Observera att endast befintliga filter, fält (för kolumner) eller grupper kan läggas till på det här sättet.</p></li>
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


>[!NOTE]
>
>Administratörer som anpassar sin egen layoutmall måste uppdatera sidan för att kunna se ändringarna.