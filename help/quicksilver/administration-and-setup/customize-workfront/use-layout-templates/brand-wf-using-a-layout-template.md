---
title: Varumärk Adobe Workfront med en layoutmall
user-type: administrator
product-area: system-administration;templates
navigation-topic: layout-templates
description: Som Adobe Workfront-administratör eller gruppadministratör kan du använda en layoutmall för att anpassa logotyperna i det övre navigeringsområdet och på huvudmenyn för vissa grupper, team, jobbroller och användare. Detta är särskilt användbart för grupper i en stor organisation som har sina egna varumärken.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ded9ab1e-c5f4-476b-ac81-0497dbe6b24d
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Varumärk Adobe Workfront med en layoutmall

>[!IMPORTANT]
>
>Den procedur som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till [!DNL Adobe Experience Cloud].
>
> Om din organisation har anslutit sig till [!DNL Adobe Experience Cloud], branding is not available.

Du kan använda en layoutmall för att anpassa logotyperna i det övre navigeringsområdet och på huvudmenyn för vissa grupper, team, jobbroller och användare. Detta är särskilt användbart för grupper i en stor organisation som har sina egna varumärken.

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

>[!NOTE]
>
>En Workfront-administratör kan göra samma anpassningar för hela organisationen på systemnivå, vilket förklaras i [Varumärk din Adobe Workfront-instans](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md). Men om du använder varumärke i en layoutmall åsidosätts varumärkningen på systemnivå.
><!--
>Maybe add a section about deleting these 2 settings to revert to default branding?
>-->

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

## Varumärk Adobe Workfront med en layoutmall

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicka på nedpilen ![](assets/dropdown-arrow.png) under **Anpassa det användarna ser** och sedan klicka **Varumärke**.
1. Gör någon av följande ändringar för att anpassa Workfront med varumärkesbilder för dem som har tilldelats den här layoutmallen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Varumärkesikonen <span style="font-weight: normal;">(visas längst till vänster i det övre navigeringsområdet)</span></p> </td> 
      <td> <p>I <strong>Övre navigeringsområde</strong> avsnitt, under <strong>Ikonen Hem</strong>, klickar du var som helst i rutan och letar upp och väljer logotypbilden. Eller dra en bild till rutan.</p> <p>Om du vill beskära bilden använder du rullningskontrollerna och drar bilden till den plats du vill ha inuti det förskrivna utrymmet.</p> <p>Vi rekommenderar en bild på 120 x 120. Den kan ha något av följande format: GIF, JPG, PNG, SVG.</p> <p>Den här ikonen visas även i rapporter, listor, kontrollpaneler och levererade rapporter som användare exporterar som PDF-filer.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Märk huvudmenyn <img src="assets/main-menu-icon.png"> logo <span style="font-weight: normal;">(visas i det övre högra hörnet av huvudmenyn)</span></p> </td> 
      <td> <p> <p> <p>I <strong>Övre navigeringsområde</strong> avsnitt, under <strong>Main Menu logo</strong>, klickar du var som helst i rutan och letar upp och väljer logotypbilden. Eller dra en bild till rutan.</p> <p>Om du vill beskära bilden använder du rullningskontrollerna och drar bilden till den plats du vill ha inuti det förskrivna utrymmet.</p> <p>Vi rekommenderar en bild på 300 x 120 pixlar. Den kan ha något av följande format: GIF, JPG, PNG, SVG.</p> </p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fortsätt att anpassa layoutmallen.

   eller

   Om du är klar med anpassningen klickar du på **Spara**.

   >[!TIP]
   >
   >Du kan klicka på Spara när som helst för att spara förloppet och sedan fortsätta att ändra mallen senare.

1. Klicka **Spara**.

Mer information om layoutmallar finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
