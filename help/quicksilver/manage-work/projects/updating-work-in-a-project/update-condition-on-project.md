---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uppdatera villkor för ett projekt
description: Villkoret för ett projekt är en flagga som placeras på det för att ange om arbetet som är kopplat till det går smidigt eller om du har stött på några hinder. Detta skiljer sig från projektets status, vilket anger om du arbetar aktivt med det eller inte.
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: b7f59552e5b66a3b2db765a49abdb2f49b1a51ec
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# Uppdatera villkor för ett projekt

Villkoret för ett projekt är en flagga som placeras på det för att ange om arbetet som är kopplat till det går smidigt eller om du har stött på några hinder. Detta skiljer sig från projektets status, vilket anger om du arbetar aktivt med det eller inte.

Du kan ställa in villkoret för ett projekt antingen automatiskt eller manuellt. Om du vill ändra villkoret för ett projekt manuellt måste du vara projektägare eller ha behörighet att hantera det.

Adobe Workfront-administratören kan skapa anpassade villkor för din miljö, vilket beskrivs i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>

För de nya licenserna:
<p>Standard</p>

För aktuella licenser:
<ul><li><p>Plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa eller öka åtkomst till projekt</p> <p>Redigera åtkomst till uppgifter och ärenden </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller öka behörigheter för aktiviteter och ärenden för att visa deras villkor</p>
   <p>Hantera behörigheter för aktiviteter och problem för att uppdatera villkoret</p>
     </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Ange villkoret automatiskt

Inställningen av villkor för ett projekt bestäms automatiskt av projektets villkorstyp. Villkorstypen måste anges till Förloppsstatus för Workfront för att automatiskt ställa in Projektets villkor.

Din Workfront- eller gruppadministratör bestämmer standardvärdet för fältet Villkorstyp för nya projekt i systemet när du anger projektinställningar under Konfigurera. Mer information finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

När du skapar ett projekt ställs villkoret för projektet automatiskt in så att det matchar projektets förloppsstatus vid den tidpunkten. Projektets förloppsstatus baseras på förloppet för aktiviteterna i projektet.

Mer information om projektvillkor och hur de beräknas baserat på förloppsstatus finns i [Översikt över status för projektförlopp](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## Uppdatera villkoret för ett projekt manuellt

Om du ställer in projektets villkorstyp på Manuell i stället för Status kan du uppdatera ett projekts villkor manuellt.

1. Gå till det projekt som du vill uppdatera villkoret för.
1. Klicka på avsnittet **Projektinformation** i den vänstra panelen.

1. Kontrollera att fältet **Villkorstyp** är inställt på **Manuell**.

   ![](assets/project-details-overview-select-condition.png)

1. I fältet **Villkor** väljer du bland följande alternativ det som matchar din förståelse för om arbetet som är kopplat till det går smidigt eller om det finns några förseningar:

   * **På mål**
   * **Vid risk**
   * **I problem**

   Mer information om projektvillkor finns i [Översikt över projektvillkor och villkorstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >Villkoren kan anpassas efter din miljö, så du kan hitta fler än tre alternativ för Villkor i din miljö. Namnen på villkoren kan skilja sig från namnen ovan. Mer information om hur du anpassar villkor i Workfront finns i [Skapa eller redigera ett anpassat villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. Klicka på **Spara ändringar**.
