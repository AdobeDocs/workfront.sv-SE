---
title: Anpassa användargränssnittsterminologi med hjälp av en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Som Adobe Workfront-administratör kan du använda en layoutmall för att ändra etiketterna för vissa objekt som visas i hela Workfront så att de matchar de termer som används i organisationen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Anpassa användargränssnittsterminologi med hjälp av en layoutmall

Som Adobe Workfront-administratör kan du använda en layoutmall för att ändra etiketterna för vissa objekt som visas i hela Workfront så att de matchar de termer som används i organisationen.

När du har sparat en layoutmall där du ändrat terminologi, loggat ut från Workfront och sedan in igen, visas de etiketter du ändrat där standardetiketterna finns i de flesta områden i Workfront:

* Huvudmeny
* Alla områden som öppnas från huvudmenyn
* Alla flikar
* Alla menyer
* Report Builder och rapportelement (vyer, filter och grupperingar)
* Spara knappar
* Exporterade filer
* E-post
* Mobilappar

>[!NOTE]
>
>* I området för Outlook-tillägg visas inte de anpassade etiketterna.
>* Du kan stöta på grammatik och andra problem när du anpassar etiketter. Om du till exempel ändrar&quot;Problem&quot; till&quot;Begäran&quot; kan det finnas platser i användargränssnittet där du ser frasen&quot;En begäran&quot;. Mer information finns i [Konsekvenser av anpassning av objektnamn](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) i artikeln [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>

Mer information om layoutmallar finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

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
Om du vill utföra dem för en grupp måste du vara gruppchef.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassa användargränssnittets terminologi

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicka **Ange terminologi** nära sidans övre högra hörn.
1. Gör något av följande:

   * Klicka på nedpilen om du vill använda en alternativ term från Workfront  ![](assets/dropdown-arrow.png) bredvid etiketten och klicka sedan på den alternativa etikett du vill ha i listrutan.

     >[!NOTE]
     >
     >Alternativa etiketter i listrutorna stöds i Workfront-versioner som är lokaliserade för andra språk än engelska.

   * Om du vill ange ett eget anpassat alternativ för etiketten som visas för ett objekt klickar du på **Ange eget namn** till höger om etiketten och skriv sedan **Singular** och **Plural** formulär för den anpassade termen. Du kan klicka **Återställ** om du ändrar dig.

     Du kan anpassa följande objektnamn:

     <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Workfront-objekt</p></td>
        <td>
          <p>Portfolio</p>
          <p>Program</p>
          <p>Projekt</p>
          <p>Uppgift</p>
          <p>Problem</p>
          <p>Mål</p>
          <p>Resultat</p>
          <p>Aktivitet</p>
         </ul></td>
        <td><p>Mer information om dessa objekt finns i <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Förstå objekt i Adobe Workfront</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Workfront Goals-objekt</p></td>
        <td>
         <ul>
          <p>Mål</p>
          <p>Resultat</p>
          <p>Aktivitet</p>
         </ul></td>
        <td><p>Dessa objekt kräver ytterligare licens. Mer information finns i <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Översikt över Adobe Workfront-mål</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront Scenario Planner-objekt</p></td>
        <td>
         <ul>
          <p>Initiative</p>
          <p>Scenario</p>
          <p>Plan </p>
         </ul></td>
        <td><p>Dessa objekt kräver ytterligare licens. Mer information finns i <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Kom igång med scenarioplanen</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. När du är klar klickar du på **Klar**.

   >[!TIP]
   >
   >När du har klickat på Klar (och även efter att du har sparat layoutmallen) kan du alltid gå tillbaka till inställningarna för Ange terminologi och klicka på Återställ bredvid eventuella anpassade termer för att återställa dem till standardläget.

1. Fortsätt att anpassa layoutmallen.

   eller

   Om du är klar med anpassningen klickar du på **Spara**.

1. Så här ser du hur terminologin ändras:

   1. Logga ut och in igen på Workfront.
   1. Stäng alla webbläsarflikar som du har öppna för din Workfront-miljö.

   >[!IMPORTANT]
   >
   >Detta är också nödvändigt för alla som använde layoutmallen innan du gjorde terminologinställningarna.

Mer information om layoutmallar finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
