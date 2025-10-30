---
title: Märk Adobe Workfront med en layoutmall
user-type: administrator
product-area: system-administration;templates
navigation-topic: layout-templates
description: Som Adobe Workfront-administratör eller gruppadministratör kan du använda en layoutmall för att anpassa logotyperna i det övre navigeringsområdet och på huvudmenyn för vissa grupper, team, jobbroller och användare. Detta är särskilt användbart för grupper i en stor organisation som har sina egna varumärken.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ded9ab1e-c5f4-476b-ac81-0497dbe6b24d
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Varumärk Adobe Workfront med en layoutmall

<!--Audited: 09/2024-->

{{preview-fast-release-general}}

>[!IMPORTANT]
>
>Den procedur som beskrivs på den här sidan gäller endast för organisationer som ännu inte har anslutit till [!DNL Adobe Experience Cloud].
>
> Om din organisation har anslutit sig till [!DNL Adobe Experience Cloud] är varumärkning inte tillgängligt.

Du kan använda en layoutmall för att anpassa logotyperna i det övre navigeringsområdet och på huvudmenyn för vissa grupper, team, jobbroller och användare. Detta är särskilt användbart för grupper i en stor organisation som har sina egna varumärken.

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

>[!NOTE]
>
>En Workfront-administratör kan göra samma anpassningar för hela organisationen på systemnivå, vilket förklaras i [Varumärket din Adobe Workfront-instans](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md). Men om du använder varumärke i en layoutmall åsidosätts varumärkningen på systemnivå.

<!-- Maybe add a section about deleting these 2 settings to revert to default branding? -->

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

## Varumärk Adobe Workfront med en layoutmall

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicka på nedpilen ![nedpilen](assets/dropdown-arrow.png) under **Anpassa det som visas för användarna** och klicka sedan på **Varumärkning**.
1. Gör någon av följande ändringar för att anpassa Workfront med varumärkesbilder för dem som har tilldelats den här layoutmallen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Förse hemikonen <span style="font-weight: normal;"> (visas längst till vänster i det övre navigeringsområdet)</span></p> </td> 
      <td> <p>I avsnittet <strong>Övre navigering</strong>, under <strong>Hem-ikonen</strong>, klickar du var som helst i rutan och söker sedan efter och väljer logotypbilden. Eller dra en bild till rutan.</p> <p>Om du vill beskära bilden använder du rullningskontrollerna och drar bilden till den plats du vill ha inuti det förskrivna utrymmet.</p> <p>Vi rekommenderar en bild på 120 x 120. Den kan ha något av följande format: GIF, JPG, PNG, SVG.</p> <p>Den här ikonen visas även i rapporter, listor, kontrollpaneler och levererade rapporter som användare exporterar som PDF-filer.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Märk huvudmenylogotypen <img src="assets/main-menu-icon.png"> <span style="font-weight: normal;"> (visas i det övre högra hörnet av huvudmenyn)</span></p> </td> 
      <td> <p> <p> <p>I avsnittet <strong>Övre navigering</strong>, under <strong>Huvudmenylogotyp</strong>, klickar du var som helst i rutan och letar sedan reda på och väljer logotypbilden. Eller dra en bild till rutan.</p> <p>Om du vill beskära bilden använder du rullningskontrollerna och drar bilden till den plats du vill ha inuti det förskrivna utrymmet.</p> <p>Vi rekommenderar en bild på 300 x 120 pixlar. Den kan ha något av följande format: GIF, JPG, PNG, SVG.</p> </p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. <span class="preview">I förhandsvisningsmiljön: Fortsätt anpassa layoutmallen. Du kan klicka på **Använd** när som helst för att spara förloppet.</span>

   <span class="preview">eller</span>

   <span class="preview">Om du är klar med anpassningen klickar du på **Spara och stäng**.</span>

1. I produktionsmiljön: Fortsätt att anpassa layoutmallen.

   eller

   Klicka på **Spara** om du är klar med anpassningen.

   >[!TIP]
   >
   >Du kan klicka på **Spara** när som helst för att spara förloppet och sedan fortsätta att ändra mallen senare.

Mer information om layoutmallar finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
