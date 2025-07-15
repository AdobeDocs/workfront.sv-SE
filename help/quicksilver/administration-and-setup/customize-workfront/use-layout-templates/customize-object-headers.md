---
title: Anpassa objektrubriker med hjälp av en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Som Adobe Workfront-administratör eller gruppadministratör kan du använda en layoutmall för att konfigurera de fält som användarna ser i objekthuvudet när de öppnar ett objekts sida.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Anpassa objektrubriker med hjälp av en layoutmall

Som Adobe Workfront-administratör eller gruppadministratör kan du använda en layoutmall för att konfigurera de fält som användarna ser i objekthuvudet när de öppnar ett objekts sida.

>[!IMPORTANT]
>
>Det går för närvarande att anpassa objektrubriker för projekt, uppgifter och ärenden.

![Objektrubrikfält](assets/object-header-fields.png)

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

## Anpassa objektrubriker

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Välj **Projekt**, **Åtgärder** eller **Problem** i den nedrullningsbara menyn **Anpassa vad användare ser**.

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. I avsnittet [!UICONTROL Header fields] för du musen över de fält som visas och gör något av följande:
   * Klicka på ikonen **x** för att ta bort ett fält

     eller

   * Klicka på och håll ned ikonen **gripna** för att dra och släppa fältet på en ny plats.

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![Objektrubrikfält döljer och flyttar ikoner](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. Du kan ha upp till fem fält i ett objekts sidhuvud.
Om du redan har markerat fem fält måste du ta bort ett fält innan du kan lägga till ett nytt.
1. I rutan **Lägg till fält** börjar du skriva namnet på ett icke-redigerbart Workfront-fält som du vill lägga till och markerar det när det visas i listan. Fältet läggs till i det högra hörnet av rutan Lägg till och visas som det första fältet i det övre vänstra hörnet av objektets rubrik.

   >[!TIP]
   >
   >* Du kan bara lägga till fält som visas i området Översikt i objektets informationsavsnitt och som inte går att redigera. Icke-redigerbara fält är fält som användare inte kan redigera manuellt. De beräknas automatiskt av Workfront.
   >
   >* Du kan lägga till redigerbara fält som redan ingår i standardrubrikerna (till exempel Projektägare, Status, Procent färdigt, Uppdrag).
   >
   >* När du lägger till fältet &quot;Löst av&quot; i huvudet på ett problem, ändras fältet till &quot;Lösa problem, Aktivitet eller Projekt&quot;, när det finns ett matchande objekt kopplat till problemet.


   ![Lägg till fält i rubrik](assets/add-field-to-header-in-lt-list.png)


1. (Valfritt) Dra och släpp fält som lagts till i en annan ordning.

1. Fortsätt att anpassa layoutmallen.

   eller

   Klicka på **Spara** om du är klar med anpassningen.

   >[!TIP]
   >
   >Du kan klicka på Spara när som helst för att spara förloppet och sedan fortsätta att ändra mallen senare.
