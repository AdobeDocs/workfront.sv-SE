---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Använd arbetsflöden i integreringen med Experience Manager Assets Essentials
description: Använd arbetsflöden i integreringen med Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: 9080dfe7e46a3780d493b59c8f2a3c4efbc011e7
workflow-type: tm+mt
source-wordcount: '756'
ht-degree: 0%

---

# Använda arbetsflöden i Experience Manager Assets-integrering

<span class="preview">Informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i förhandsvisningssandlådemiljön.</span>

Ett arbetsflöde är en uppsättning åtgärder som kopplar Workfront till Adobe Experience Manager as a Cloud Service. En Workfront-administratör kan konfigurera arbetsflöden i Workfront och sedan tilldela dem till Projektmallar. När ett projekt skapas med en projektmall som ett arbetsflöde är tilldelat till, aktiveras de åtgärder som definieras i arbetsflödet.

>[!NOTE]
>
>Arbetsflöden är bara tillgängliga i en Adobe Experience Manager as a Cloud Service-integrering. De är inte tillgängliga i integreringar med Adobe Experience Manager Assets Essentials.


## Åtkomstkrav

Du måste ha följande:

<table>
  <tr>
   <td><strong>Adobe Workfront-plan*</strong>
   </td>
   <td>Alla
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-licenser*</strong>
   </td>
   <td>Begäran eller senare
   </td>
  </tr>
  <tr>
   <td><strong>Produkt</strong>
   </td>
   <td><p>Du måste ha Experience Manager Assets as a Cloud Service eller Assets Essentials, och du måste läggas till som användare i Admin Console.</p><p>Du måste ha skrivåtkomst till databasen i Adobe Experience Manager för att kunna skapa länkade mappar.</p>&gt;
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationer på åtkomstnivå*</strong>
   </td>
   <td>Redigera åtkomst till dokument
<p>
<strong>Obs! </strong>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <strong>Skapa eller ändra anpassade åtkomstnivåer</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Objektbehörigheter</strong>
   </td>
   <td>Hantera åtkomst eller senare i projektet 
<p>
Mer information om hur du begär ytterligare åtkomst finns i <strong>Begär åtkomst till objekt </strong>.
   </td>
  </tr>
</table>

## Förutsättningar

Innan du börjar,

* Din Workfront-administratör måste konfigurera arbetsflöden i en Adobe Experience Manager-integrering. Mer information finns i [Konfigurera Experience Manager Assets as a Cloud Service-integrering](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Lägga till ett arbetsflöde i en mall

Du kan lägga till ett arbetsflöde i en projektmall. Arbetsflödet används för alla projekt som skapas från mallen.

1. <!-- main menu snippet??--> Öppna en mall genom att klicka på **Mallar** på huvudmenyn och sedan väljer du mallen i listan.
1. Klicka **Experience Manager Assets** i den vänstra navigeringspanelen.

   >[!NOTE]
   >
   >Om Experience Manager Assets-avsnittet inte visas i den vänstra navigeringen har Workfront-administratören inte aktiverat arbetsflöden för din organisation. <!--Is this right?-->

1. I **Välj en integrering för fält för automatiserade arbetsflöden** väljer du integrering med de arbetsflöden du vill använda för projekt som skapas från den här mallen.
1. (Valfritt) Redigera alla arbetsflödesvärden som du vill använda för projekt som skapas från den här mallen.

   Om du till exempel vill skapa en länkad mapp på en annan plats än standardvärdet anger du platsen för den länkade mappen.

   Endast arbetsflöden som har aktiverats under Experience Manager i installationsprogrammet är tillgängliga i mallar eller projekt.

1. Ändringarna sparas automatiskt. <!-- do they though??-->

## Lägga till ett arbetsflöde i ett projekt

Du kan lägga till ett arbetsflöde när du skapar ett projekt eller lägga till ett arbetsflöde i ett befintligt projekt. I båda fallen använder du en projektmall för att lägga till arbetsflödet.

### Lägga till ett arbetsflöde när du skapar ett projekt

1. Börja skapa ett projekt.

   Instruktioner finns i [Skapa ett projekt med en mall](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. När du väljer en mall för projektet väljer du den mall som innehåller de arbetsflöden du vill använda för det här projektet.
1. (Valfritt) Redigera alla arbetsflödesvärden för projektet enligt beskrivningen i [Redigera arbetsflödesvärden i ett projekt](#edit-workflow-values-in-a-project).

   Endast arbetsflöden som har aktiverats under Experience Manager i installationsprogrammet är tillgängliga i mallar eller projekt.


### Lägga till ett arbetsflöde i ett befintligt projekt

1. Börja lägga till en mall i projektet.

   Instruktioner finns i [Bifoga en mall till ett projekt](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. När du väljer en mall för projektet väljer du den mall som innehåller de arbetsflöden du vill använda för det här projektet.
1. (Valfritt) Redigera alla arbetsflödesvärden för projektet enligt beskrivningen i [Redigera arbetsflödesvärden i ett projekt](#edit-workflow-values-in-a-project).

### Redigera arbetsflödesvärden i ett projekt

Du kan redigera arbetsflödesvärden på projektnivå. Arbetsflödesvärden på projektnivå åsidosätter värden som angetts i projektmallen, som åsidosätter standardvärdena som angetts i Adobe Experience Manager Assets-integreringen.

Alla arbetsflödesvärden finns i:

* Avsnittet Arbetsflöden i fönstret Skapa projekt eller Redigera projekt.
* The Adobe Experience Manager section of the left navigation.


   >[!NOTE]
   >
   >Om dessa områden inte visas har Workfront-administratören inte aktiverat arbetsflöden för din organisation.

#### Länkade mappar

Så här redigerar du arbetsflödet för länkade mappar:

1. Växla **[!UICONTROL Create Linked folder]** på.
1. Välj en mappsökväg för att ange var du vill att alla länkade mappar som är associerade med den här integreringen ska vara.
1. Klicka på Spara om du använder fönstret Skapa projekt eller Redigera projekt.

   eller

   Om du befinner dig i Adobe Experience Manager sparar ändringarna automatiskt. <!--Do they though?-->

