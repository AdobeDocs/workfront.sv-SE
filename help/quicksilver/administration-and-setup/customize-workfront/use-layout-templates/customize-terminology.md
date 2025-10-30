---
title: Anpassa användargränssnittets terminologi med hjälp av en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Som Adobe Workfront-administratör kan du använda en layoutmall för att ändra etiketterna för vissa objekt som visas i hela Workfront så att de matchar de termer som används i organisationen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# Anpassa användargränssnittsterminologi med hjälp av en layoutmall

{{preview-fast-release-general}}

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
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>För att kunna utföra dessa steg på systemnivå måste du ha åtkomstnivån Systemadministratör.</p>
        <p>Om du vill utföra dem för en grupp måste du vara chef för den gruppen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anpassa användargränssnittets terminologi

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicka på **Ange terminologi** i det övre högra hörnet på sidan.
1. Gör något av följande:

   * Om du vill använda en alternativ term som tillhandahålls av Workfront klickar du på nedpilen ![nedpilen](assets/dropdown-arrow.png) bredvid etiketten och klickar sedan på den alternativa etiketten som du vill använda i listrutan.

     >[!NOTE]
     >
     >Alternativa etiketter i listrutorna stöds i Workfront-versioner som är lokaliserade för andra språk än engelska.

   * Om du vill ange ett eget anpassat alternativ för den etikett som visas för ett objekt klickar du på **Ange anpassat namn** till höger om etiketten och skriver sedan de anpassade termens **Singular**- och **Plural**-former. Du kan klicka på **Återställ** om du ångrar dig.

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
        <td><p>Mer information om de här objekten finns i <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Förstå objekt i Adobe Workfront</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Workfront Goals-objekt</p></td>
        <td>
         <ul>
          <p>Mål</p>
          <p>Resultat</p>
          <p>Aktivitet</p>
         </ul></td>
        <td><p>Dessa objekt kräver ytterligare licens. Mer information finns i <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront-målöversikt</a>.</p></td>
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

1. <span class="preview">I förhandsvisningsmiljön: Fortsätt anpassa layoutmallen. Du kan klicka på **Använd** när som helst för att spara förloppet.</span>

   <span class="preview">eller</span>

   <span class="preview">Om du är klar med anpassningen klickar du på **Spara och stäng**.</span>

1. I produktionsmiljön: Fortsätt att anpassa layoutmallen.

   eller

   Klicka på **Spara** om du är klar med anpassningen.

1. Så här ser du hur terminologin ändras:

   1. Logga ut och in igen på Workfront.
   1. Stäng alla webbläsarflikar som du har öppna för din Workfront-miljö.

   >[!IMPORTANT]
   >
   >Detta är också nödvändigt för alla som använde layoutmallen innan du gjorde terminologinställningarna.

Mer information om layoutmallar finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
