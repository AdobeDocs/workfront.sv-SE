---
product-area: projects
navigation-topic: financials
title: Åsidosätt faktureringshastigheter för jobbroller på projektnivå
description: Som projektledare kan du ange faktureringssatsen för en jobbroll i ett visst projekt. Den här faktureringsnivån på projektnivå åsidosätter faktureringsnivån på systemnivån för den här jobbrollen. Workfront använder faktureringssatsen på projektnivå för jobbrollen för att beräkna intäkten, i stället för att använda faktureringssatsen på systemnivå.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: 5e2c2a29c822150377882006bd6bc15068ff8702
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---

# Åsidosätt faktureringshastigheter för jobbroller på projektnivå

{{highlighted-preview}}

Som projektledare kan du ange faktureringssatsen för en jobbroll i ett visst projekt. Den här faktureringsnivån på projektnivå åsidosätter faktureringsnivån på systemnivån för den här jobbrollen. Workfront använder faktureringssatsen på projektnivå för jobbrollen för att beräkna intäkten, i stället för att använda faktureringssatsen på systemnivå.

I den här artikeln beskrivs hur du kan åsidosätta faktureringstaxorna för systemjobbroller för ett projekt.

Allmän information om hur du åsidosätter faktureringssatser för jobbroller för projekt och beräknar projektintäkter finns i [Översikt över åsidosättande av faktureringssatser för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Mer information om vilken jobbroll som används för att beräkna intäkter för projektet finns i avsnittet Förstå intäktsberäkningar för aktiviteter baserade på användar- och rolltilldelningar i artikeln [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>När det gäller Faktisk intäkt bör de faktureringstariffer som tillämpas på timmar som läggs till i en faktureringspost som är markerad som Fakturerad inte påverkas av åsidosättningar av faktureringstaxor som inträffar efter att faktureringsposten har fakturerats.

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p> <p>Administrativ åtkomst för jobbroller</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Hantera behörigheter för det projekt som innehåller Redigera ekonomiska data </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Åsidosätt faktureringshastigheter för jobbroller på projektnivå

Du kan åsidosätta faktureringsfrekvensen för en jobbroll i ett projekt på följande sätt:

* En gång genom att välja en ny avgift för jobbrollen.\
  Den nya avgiften används för att beräkna intäkterna under hela projektets löptid.

* Flera gånger genom att välja flera nya priser för specifika datumintervall.\
  Du kan använda olika hastigheter under varje angivet datumintervall.

* Du kan lägga till nya faktureringstariffer i en projektmall och dessa blir projektfaktureringstariffer när du skapar projektet från den mallen. Mer information om hur du redigerar mallar finns i [Redigera projektmallar](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!TIP]
>
>Du kan inte åsidosätta användarfaktureringstariffer för ett projekt.

Så här åsidosätter du en faktureringstaxa för ett projekt:

1. Gå till det projekt som du vill åsidosätta faktureringstariffer för.
1. Klicka på **Faktureringstariffer** i den vänstra panelen.
1. Klicka på **Lägg till faktureringsränta** > **Ny faktureringsränta**.

   Rutan Ny faktureringsränta öppnas.

1. I fältet **Jobbroll** väljer du den jobbroll du vill ändra faktureringsfrekvensen för.

   Fältet **Standardfaktureringsfrekvens** visar systemnivåfrekvensen för den här jobbrollen.

1. I fältet **Faktureringstariffer 1** anger du åsidosättning av engångsavgift och klickar sedan på **Spara** för att åsidosätta faktureringstaxan en gång

   eller

   Klicka på **Lägg till ränta** om du vill lägga till fler åsidosättningar av faktureringsfrekvens.

1. (Villkorligt) Om du lägger till fler än en åsidosättning av faktureringsfrekvens anger du följande information:

   * **Faktureringstariffer 1**: värdet på faktureringstakten från början av projektet till första datumet för den första åsidosättningen. Detta är vanligtvis samma belopp som **standardfrekvensen**.
   * **Startdatum**: Detta är det datum då standardhastigheten slutar.
   * **Slutdatum**: det datum då den nya faktureringstariffen upphör.

   <span class="preview">Exempelbild i förhandsvisningsmiljön:</span>
   ![Faktureringstariffer med åsidosättningsdatum](assets/billing-rates-093025.png)

   Exempelbild i produktionsmiljön:
   ![Faktureringstariffer med åsidosättningsdatum](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. Tidszonen för de datum du väljer visas längst ned i rutan Ny faktureringsfrekvens. Detta är den tidszon som är kopplad till din Workfront-instans, vilket visas i området Kundinformation i installationsprogrammet. Mer information finns i [Konfigurera grundläggande information för systemet](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. Workfront tillämpar rollfrekvensen för åsidosättningsjobb på de timmar som inträffar under de tidsramar som anges vid beräkning av projektets intäkter.
1. Det ska inte finnas några mellanrum mellan tidsbildrutorna för två åsidosättningsfrekvenser. **Startdatum** för en åsidosättningsfrekvens ska vara dagen omedelbart efter **Slutdatum** för föregående åsidosättningsdatum.

1. Du kan inte ange ett startdatum för den första åsidosättningsfrekvensen eller ett slutdatum för den senaste åsidosättningsfrekvensen.\
   Vi rekommenderar att du använder standardpriset för den första åsidosättningsfrekvensen.\
   Workfront antar att den första åsidosättandefrekvensen används för alla timmar med ett datum som är äldre än slutdatumet för den första åsidosättningen och att den senaste åsidosättandefrekvensen används för alla timmar med ett datum som är senare än startdatumet för den senaste åsidosättningen.\
   Om en timme loggas före projektets planerade startdatum används den första faktureringstakten.\
   Om en timme loggas efter projektets planerade slutförandedatum används den sista faktureringstakten.

1. Klicka på **Spara**.
