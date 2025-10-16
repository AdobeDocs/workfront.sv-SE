---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Ändra interaktiv korrekturupplösning i korrekturläsaren
description: Du kan förhandsgranska hur ett interaktivt korrektur ser ut på olika enheter, så att du kan se hur innehållet visas och svarar baserat på olika upplösningar.
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: 385f4a6663cacfdcf519bf5699fc1840c2cb2adc
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Ändra interaktiv korrekturupplösning i korrekturläsaren

Du kan förhandsgranska hur ett interaktivt korrektur ser ut på olika enheter, så att du kan se hur innehållet visas och svarar baserat på olika upplösningar.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Korrekturroll </td> 
   <td>Granskare, granskare och godkännare, författare, moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Enhets- och upplösningsvyer i Desktop Proofing Viewer jämfört med Web Proofing Viewer

Din Adobe Workfront-administratör har konfigurerat ditt system så att du kan granska interaktivt innehåll antingen i Desktop Proofing Viewer eller, som paketerat innehåll i en ZIP-fil, i Web Proofing Viewer:

* I Desktop Proofing Viewer kan du visa hur innehåll visas och svarar både i olika upplösningar och på olika enheter. När en granskare anger en viss enhet ser innehållet ut som på den enheten, med enhetens gränssnittsspecifikationer. En röd knapp på ett varumärke i smarttelefonen kan till exempel vara blå på ett annat varumärke.

* I Web Proofing Viewer kan du visa interaktivt innehåll så som det visas i upplösningar för de olika enheterna. Men Web Proofing Viewer emulerar inte innehållet med gränssnittsspecifikationer på dessa enheter, till exempel knappfärg.

  >[!NOTE]
  >
  >Din Workfront-administratör kan konfigurera anpassade enheter för användare i din organisation enligt beskrivningen i [Konfigurera anpassade enheter för korrektur](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#configure-custom-devices-for-proofs) i artikeln [Konfigurera korrekturinställningar för din organisation](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

## Visa ett korrektur med en förinställd enhet eller upplösningsinställning

1. Gå till dokumentlistan som innehåller det korrektur som du vill öppna.
1. Håll pekaren över dokumentet och klicka sedan på **Öppna korrektur**.
1. Klicka på **Responsiv** i mitten av korrekturläsaren.

   ![Resolution_option_in_DPV.png](assets/resolution-option-in-dpv-350x64.png)

1. Klicka på önskad enhet i listan över enheter och upplösningar i Desktop Proofing Viewer.

   eller

   I Web Proofing Viewer klickar du på önskad upplösning i listan med upplösningar.

   Om du behöver information om hur dessa två visningsprogram skiljer sig läser du [Skillnader mellan Web Proofing Viewer och Desktop Proofing Viewer.](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

   Det interaktiva korrekturet återges i den upplösning du väljer.

## Visa ett korrektur med en anpassad upplösningsinställning

1. Gå till dokumentlistan som innehåller det korrektur som du vill öppna.
1. Håll pekaren över dokumentet och klicka sedan på **Öppna korrektur**.
1. Klicka på **Responsiv** i mitten ned i korrekturläsaren.
1. Ange en anpassad **responsiv**-upplösning.

   ![Type_a_custom_resolution_DPV.png](assets/type-a-custom-resolution-dpv.png)

   eller

   För musen över det interaktiva innehållet och dra den blå kanten längst ned till höger eller höger eller längst ned till önskad upplösning.

   ![Drag_blue_edges_for_resolution.png](assets/drag-blue-edges-for-resolution-350x251.png)

   Den anpassade upplösningen visas på följande platser:

   * I panelen **Upplösning** längst ned i mitten av visningsprogrammet.\
     ![Screenshot_2018-05-15_10-27-54.png](assets/screenshot-2018-05-15-10-27-54.png)

   * I kommentarer lägger granskarna till korrekturet. Varje kommentar innehåller den skärmupplösning som valdes när granskaren skapade kommentaren.
