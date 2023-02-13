---
product-area: projects
navigation-topic: financials
title: Åsidosätt faktureringshastigheter för jobbroller på projektnivå
description: Som projektledare kan du ange faktureringssatsen för en jobbroll i ett visst projekt. Den här faktureringsnivån på projektnivå åsidosätter faktureringsnivån på systemnivån för den här jobbrollen. Workfront använder faktureringssatsen på projektnivå för jobbrollen för att beräkna intäkten, i stället för att använda faktureringssatsen på systemnivå.
author: Alina
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# Åsidosätt faktureringshastigheter för jobbroller på projektnivå

Som projektledare kan du ange faktureringssatsen för en jobbroll i ett visst projekt. Den här faktureringsnivån på projektnivå åsidosätter faktureringsnivån på systemnivån för den här jobbrollen. Workfront använder faktureringssatsen på projektnivå för jobbrollen för att beräkna intäkten, i stället för att använda faktureringssatsen på systemnivå.

I den här artikeln beskrivs hur du kan åsidosätta faktureringstaxorna för systemjobbroller för ett projekt.

Allmän information om hur du åsidosätter faktureringssatser för jobbroller för projekt och beräknar projektintäkter finns i [Översikt över åsidosättande av faktureringstaxor för jobbroller och beräkning av intäkter för ett projekt](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Mer information om vilken jobbroll som används för att beräkna intäkter i projektet finns i avsnittet Förstå intäktsberäkningar för aktiviteter baserade på användar- och rolltilldelningar i artikeln [Översikt över fakturering och intäkt](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>När det gäller Faktisk intäkt bör de faktureringstariffer som tillämpas på timmar som läggs till i en faktureringspost som är markerad som Fakturerad inte påverkas av åsidosättningar av faktureringstaxor som inträffar efter att faktureringsposten har fakturerats.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p> <p>Administrativ åtkomst för jobbroller</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för det projekt som innehåller Redigera ekonomiska data </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Åsidosätt faktureringshastigheter för jobbroller på projektnivå

Du kan åsidosätta faktureringsfrekvensen för en jobbroll i ett projekt på följande sätt:

* En gång genom att välja en ny avgift för jobbrollen.\
   Den nya avgiften används för att beräkna intäkterna under hela projektets löptid.

* Flera gånger genom att välja flera nya priser för specifika datumintervall.\
   Du kan använda olika hastigheter under varje angivet datumintervall.

>[!TIP]
>
>Du kan inte åsidosätta användarfaktureringstariffer för ett projekt.

Så här åsidosätter du en faktureringstaxa för ett projekt:

1. Gå till det projekt som du vill åsidosätta faktureringstariffer för.
1. Klicka **Faktureringstaxor** i den vänstra panelen. Du måste kanske först klicka **Visa fler**.
1. Klicka **Lägg till faktureringsränta** > **Ny faktureringstakt**.

   Rutan Ny faktureringsränta öppnas.

1. I **Jobbroll** väljer du den jobbroll som du vill ändra faktureringssatsen för.

   ![](assets/override-billing-rate-on-project-nwe-350x310.png)

   The **Standardfaktureringshastighet** visas systemnivåfrekvensen för den här jobbrollen.

1. I **Faktureringstariffer 1** anger du åsidosättning av engångsavgiften och klickar sedan på **Spara** för att åsidosätta faktureringstaxan en gång

   eller

   Klicka **Lägg till frekvens** om du vill lägga till fler åsidosättningar av faktureringsfrekvens.

1. (Villkorligt) Om du lägger till fler än en åsidosättning av faktureringsfrekvens anger du följande information:

   * **Faktureringstariffer 1**: Värdet på faktureringstakten från början av projektet till första datumet för den första åsidosättningen. Det här är vanligtvis samma mängd som **Standardhastighet**.
   * **Startdatum**: detta är det datum då standardpriset upphör.
   * **Slutdatum**: det datum då den nya faktureringstakten upphör.

   ![new_billing_rate_with_adjustment_dates.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. Tidszonen för de datum du väljer visas längst ned i rutan Ny faktureringsfrekvens. Detta är den tidszon som är kopplad till din Workfront-instans, vilket visas i området Kundinformation i installationsprogrammet. Mer information finns i [Konfigurera grundläggande information för ditt system](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. Workfront tillämpar rollfrekvensen för åsidosättningsjobb på de timmar som inträffar under de tidsramar som anges vid beräkning av projektets intäkter.
1. Det ska inte finnas några mellanrum mellan tidsbildrutorna för två åsidosättningsfrekvenser. The **Startdatum** för en override-frekvens ska vara dagen omedelbart efter **Slutdatum** av föregående åsidosättningsdatum.

1. Du kan inte ange ett startdatum för den första åsidosättningsfrekvensen eller ett slutdatum för den senaste åsidosättningsfrekvensen.\
   Vi rekommenderar att du använder standardpriset för den första åsidosättningsfrekvensen.\
   Workfront antar att den första åsidosättandefrekvensen används för alla timmar med ett datum som är äldre än slutdatumet för den första åsidosättningen och att den senaste åsidosättandefrekvensen används för alla timmar med ett datum som är senare än startdatumet för den senaste åsidosättningen.\
   Om en timme loggas före projektets planerade startdatum används den första faktureringstakten.\
   Om en timme loggas efter projektets planerade slutförandedatum används den sista faktureringstakten.

1. Klicka **Spara**.
