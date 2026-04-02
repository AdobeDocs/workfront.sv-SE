---
content-type: overview
product-area: projects
navigation-topic: financials
title: Åsidosätt användarkostnadstariffer på projektnivå
description: I den här artikeln beskrivs hur du kan åsidosätta systemets användarkostnader för ett projekt.
author: Lisa
feature: Work Management
source-git-commit: cb21414992587c62c37580f156100f2b5b755e9b
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 0%

---

# Åsidosätt användarkostnadstariffer på projektnivå

{{highlighted-preview-article-level}}

Du kan ange kostnadsnivån för en användare i ett visst projekt. Kostnadsnivån på projektnivå åsidosätter kostnadsnivån på systemnivån för den här användaren. Workfront använder kostnadstariffen på projektnivå för jobbrollen för att beräkna kostnaden, i stället för att använda kostnadstariffen på systemnivå.

I den här artikeln beskrivs hur du kan åsidosätta systemets användarkostnader för ett projekt.

Mer information om hur du beräknar kostnader för projektet finns i [Översikt över intäkt- och kostnadshierarkin](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) och [Spåra kostnader](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Arbetsflöde Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till projekt och finansiella data</p>
       <p><p>Du måste också ha något av följande:</p> 
        <ul> 
          <li> <p>Åtkomstnivån Systemadministratör. </li> 
          <li> <p><b>Användare</b> i din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av de två <b>användaradministratörsalternativen</b> som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om <b>Användaradministratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Hantera behörigheter för det projekt som innehåller Redigera ekonomiska data </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Användaren måste ha fältet **Åsidosätt kostnadstariff** aktiverat för sin användarprofil. När en användare inte har fältet för kostnadsåsidosättning aktiverat tillåts inte kostnadsåsidosättningar för den användaren i något projekt, och systemet använder priset för användarprofilen för att beräkna kostnaden.

Mer information finns i [Redigera en användares profil](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Åsidosätt användarkostnadstariffer på projektnivå

1. Gå till det projekt som du vill åsidosätta kostnadstariffer för.
1. Klicka på **Kurser** i den vänstra panelen. Du måste kanske först klicka på **Visa mer**.
1. Klicka på fliken **Kostnad** om den inte redan är markerad.
1. Klicka på **Lägg till kostnadstariff** > **Ny kostnadstariff**.

   Rutan Ny kostnadstariff för användare öppnas.

1. I fältet **Användare** väljer du den användare som du vill ändra kostnadstariffen för.
1. Välj **Valuta** för åsidosättning av kostnadstariff.
1. I fältet **Kostnadstariff** anger du den första kostnadstariff-åsidosättningen.
1. (Valfritt) Klicka på **Lägg till giltighetsdatum** om du vill lägga till fler åsidosättningar av kostnadstariffer.

   >[!NOTE]
   >
   >Om du anger en åsidosättning med en enda avgift gäller den hela projektets livslängd.
   >Om du vill ha olika priser över tiden kan du lägga till flera datumeffektiva åsidosättningar.

1. (Villkorligt) Om du lägger till åsidosättningar av kostnadstariffer anger du följande information för varje rad:

   * **Kostnadsnivå**: Kostnadsnivån under den angivna tidsperioden.
   * **Startdatum**: det datum då åsidosättningen av kostnadstariff börjar.
   * **Slutdatum**: det datum då kostnadstariff-åsidosättningen upphör.

   ![Rutan Ny användarkostnadstariff som visar giltighetsdatum](assets/new-user-cost-rate-box.png)

   Workfront tillämpar rollfrekvensen för åsidosättningsjobb på de timmar som inträffar under dessa tidsramar när kostnaden för projektet beräknas.

   Det ska inte finnas några mellanrum mellan tidsbildrutorna för två åsidosättningsfrekvenser. **Startdatum** för en åsidosättningsfrekvens ska vara dagen omedelbart efter **Slutdatum** för föregående åsidosättningsdatum.

   Du behöver inte ange ett startdatum för den första åsidosättningsfrekvensen eller ett slutdatum för den senaste åsidosättningsfrekvensen.

   Vi rekommenderar att du använder standardpriset för den första åsidosättningsfrekvensen.

   Workfront antar att den första åsidosättandefrekvensen används för alla timmar med ett datum som är äldre än slutdatumet för den första åsidosättningen och att den senaste åsidosättandefrekvensen används för alla timmar med ett datum som är senare än startdatumet för den senaste åsidosättningen.

   Om en timme loggas före projektets planerade startdatum används den första självkostnaden.

   Om en timme loggas efter projektets planerade slutförandedatum används den sista kostnadstariffen.

1. Klicka på **Spara**.


