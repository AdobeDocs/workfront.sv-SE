---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Använd arbetsflöden i integreringen med Experience Manager Assets Essentials
description: Använd arbetsflöden i integreringen med Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 0%

---

# Använda arbetsflöden i Experience Manager Assets-integrering

Ett arbetsflöde är en uppsättning åtgärder som kopplar Workfront till Adobe Experience Manager as a Cloud Service. En Workfront-administratör kan konfigurera arbetsflöden i Workfront och sedan tilldela dem till Projektmallar.

När ett projekt skapas med en projektmall som ett arbetsflöde är tilldelat till, aktiveras de åtgärder som definieras i arbetsflödet.

>[!NOTE]
>
>Arbetsflöden är bara tillgängliga i en Adobe Experience Manager as a Cloud Service-integrering. De är inte tillgängliga i integreringar med Adobe Experience Manager Assets Essentials.


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser</td> 
   <td> 
   <p>Medarbetare eller högre</p> 
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ytterligare produkter</td> 
   <td>Du måste ha Experience Manager as a Cloud Service eller Assets Essentials, och du måste läggas till i produkten som användare i Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager-behörigheter</td> 
    <td>Du måste ha skrivåtkomst till mappen.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar,

* Din Workfront-administratör måste konfigurera arbetsflöden i en Adobe Experience Manager-integrering. Mer information finns i [Konfigurera integreringen med Experience Manager Assets as a Cloud Service](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Lägga till ett arbetsflöde i en mall

Du kan lägga till ett arbetsflöde i en projektmall. Arbetsflödet används för alla projekt som skapas från mallen.

1. Öppna en mall genom att klicka på **Mallar** på huvudmenyn och sedan välja mallen i listan.
1. Klicka på **Experience Manager Assets** i den vänstra navigeringspanelen.

   >[!NOTE]
   >
   >Om Experience Manager Assets-avsnittet inte visas i den vänstra navigeringen har Workfront-administratören inte aktiverat arbetsflöden för din organisation. <!--Is this right?-->

1. I fältet **Välj en integrering för automatiserade arbetsflöden** väljer du integreringen med de arbetsflöden du vill använda för projekt som skapas från den här mallen.
1. (Valfritt) Redigera alla arbetsflödesvärden som du vill använda för projekt som skapas från den här mallen.

   Instruktioner om specifika arbetsflöden finns i [Redigera arbetsflödesvärden i ett projekt](#edit-workflow-values-in-a-project) i den här artikeln.

   Endast arbetsflöden som har aktiverats under Experience Manager finns tillgängliga i mallar eller projekt.

1. Ändringarna sparas automatiskt. <!-- do they though??-->

## Lägga till ett arbetsflöde i ett projekt

Du kan lägga till ett arbetsflöde när du skapar ett projekt eller lägga till ett arbetsflöde i ett befintligt projekt. I båda fallen använder du en projektmall för att lägga till arbetsflödet.

### Lägga till ett arbetsflöde när du skapar ett projekt

1. Börja skapa ett projekt.

   Instruktioner finns i [Skapa ett projekt med en mall](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. När du väljer en mall för projektet väljer du den mall som innehåller de arbetsflöden du vill använda för det här projektet.
1. (Valfritt) Redigera alla arbetsflödesvärden för projektet, enligt beskrivningen i [Redigera arbetsflödesvärden i ett projekt](#edit-workflow-values-in-a-project).

   Endast arbetsflöden som har aktiverats under Experience Manager finns tillgängliga i mallar eller projekt.


### Lägga till ett arbetsflöde i ett befintligt projekt

>[!NOTE]
>
>Arbetsflöden som körs när ett projekt skapas (till exempel när en länkad mapp skapas) körs inte när mallen kopplas till ett befintligt projekt. De körs bara när ett projekt skapas från en mall.

1. Börja lägga till en mall i projektet.

   Instruktioner finns i [Koppla en mall till ett projekt](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. När du väljer en mall för projektet väljer du den mall som innehåller de arbetsflöden du vill använda för det här projektet.
1. (Valfritt) Redigera alla arbetsflödesvärden för projektet, enligt beskrivningen i [Redigera arbetsflödesvärden i ett projekt](#edit-workflow-values-in-a-project).

   Endast arbetsflöden som har aktiverats under Experience Manager finns tillgängliga i mallar eller projekt.



### Redigera värden i ett projekt

Du kan redigera arbetsflödesvärden på projektnivå. Arbetsflödesvärden på projektnivå åsidosätter värden som angetts i projektmallen, som åsidosätter standardvärdena som angetts i Adobe Experience Manager Assets-integreringen.

Alla arbetsflödesvärden finns i:

* Avsnittet Arbetsflöden eller länkade mappar i fönstret Skapa projekt eller Redigera projekt.
* The Adobe Experience Manager section of the left navigation.


  >[!NOTE]
  >
  >Om dessa områden inte visas har Workfront-administratören inte aktiverat arbetsflöden för din organisation.



#### Länkade mappar

>[!NOTE]
>
>Eftersom länkade mappar skapas när projektet skapas är det ineffektivt att redigera arbetsflödet för länkade mappar i ett befintligt projekt. Redigera dessa värden när du skapar en projektfunktion som förväntat.

Redigera arbetsflödet för länkade mappar:

1. Aktivera eller inaktivera **[!UICONTROL Create Linked folder]** efter behov. Om du aktiverar det kan du sedan redigera konfigurationen för den länkade mappen.

   Mer information om konfigurationen av den länkade mappen finns i [Skapa länkade Adobe Experience Manager-mappar](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) i artikeln [Konfigurera [!UICONTROL Experience Manager Assets as a Cloud Service]-integreringen](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (Valfritt) Om du vill att mappträdet bara ska byggas om det finns vissa värden i ett anpassat formulär som är kopplat till projektet klickar du på **Använd filter** för det mappträdet och väljer sedan det anpassade formulär som innehåller fältet, fältet och fältvärdet. Om fältet i det anpassade formuläret som är kopplat till det nya projektet innehåller det valda värdet skapas mappträdet.
1. (Valfritt) När du konfigurerar mappnamn kan du välja bland följande alternativ:

   * **Namn**: Ange ett namn för mappen.

   * **Objektdata**: Välj källa för mappnamnet, till exempel Projektnamn.

   * **Anpassade formulärdata**: Välj anpassade formulärdata som ska användas som mappnamn.

     Anpassade formulärdata för mappnamn är bara tillgängliga på mallnivå och kan inte konfigureras på integreringsnivå.

     Om ett mappnamn är inställt på anpassade data som inte finns på det anpassade för att kopplas till projektet, tilldelas ett slumpmässigt ID som mappnamn.

1. Om du vill visa mappträdet klickar du på ikonen **Förhandsgranska** ![Förhandsgranska](assets/preview-icon.png) .
1. Klicka på **[!UICONTROL Save]**.

#### Publicera resurser

Så här redigerar du arbetsflödet för publicering av resurser:

1. Aktivera eller inaktivera **Publicera resurser automatiskt** efter behov.
1. (Villkorligt) Om du aktiverar publicering väljer du om du vill publicera till publiceringstjänsten, varumärkesportalen eller båda.
1. Klicka på **[!UICONTROL Save]**.
