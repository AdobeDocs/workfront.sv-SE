---
title: Ta bort användare
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: När en användare lämnar din organisation kan ta bort den användaren från Workfront, men vi rekommenderar att du inaktiverar användare i stället för att ta bort dem.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 0%

---

# Ta bort användare

>[!IMPORTANT]
>
>Den procedur som beskrivs på den här sidan gäller endast organisationer som ännu inte har anslutit sig till Adobe Business Platform. Om du har anslutit dig till Adobe Business Platform måste du ta bort användare i Adobe Admin Console.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Business Platform finns i [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

När en användare lämnar organisationen kan du ta bort den användaren från Adobe Workfront.

>[!IMPORTANT]
>
>Om du tar bort en användare från systemet tas även information som är kopplad till användaren bort. Vi rekommenderar att du inaktiverar användare i stället för att ta bort dem. Mer information finns i [Inaktivera eller återaktivera en användare](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

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
   <td><p>Nytt: Standard</p><p>eller</p><p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. </li> 
     <li> <p><b>Användare</b> i din åtkomstnivå har konfigurerats till <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst ett av de två <b>användaradministratörsalternativen</b> som har aktiverats under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Om <b>Användaradministratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort kontra inaktivera en användare

När du inaktiverar en användare händer följande:

* Tar bort användarens licenser till både Workfront och Workfront Proof om Workfront Proof-komponenten är kopplad till ditt Workfront-konto. Mer information om Workfront Proof finns i [Workfront Proof: artikelindex](../../../workfront-proof/workfront-proof.md).
* Användaren kan inte längre tilldelas arbete.
* Användaren kan inte längre läggas till i uppdateringar.
* Användaren kan inte längre läggas till i team eller grupper.
* Objekt kan inte längre delas med användaren.
* Deras koppling till följande objekt förblir intakt:

   * Uppgifter, ärenden, projekt, portfolior
   * Kontrollpaneler

     >[!NOTE]
     >
     >Om du inaktiverar en användare och inte längre kan visa rapporter eller instrumentpaneler som är kopplade till en användare, kan du behöva uppdatera **Kör den här rapporten med åtkomstbehörigheten**.\
     >Mer information finns i [Varför kan jag inte komma åt en rapport som ägs av en inaktiverad användare?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) i artikeln [Rapporterar vanliga frågor och svar](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

   * Dokument
   * Uppdateringar
   * Timmar

* Om användaren har checkat ut dokument förblir dokumenten utcheckade när du inaktiverar dem. Endast en Workfront-administratör kan checka in dem igen. Mer information om utcheckning av dokument finns i [Checka ut dokument](../../../documents/managing-documents/check-out-documents.md).

Om du tar bort en användare händer följande:

* Tar bort användarens licenser till både Workfront och Workfront Proof, om Workfront Proof-komponenten är kopplad till ditt Workfront-konto. Mer information om Workfront Proof finns i [Workfront Proof: artikelindex](../../../workfront-proof/workfront-proof.md).
* Användaren kan inte längre tilldelas arbete.
* Användaren kan inte längre läggas till i uppdateringar.
* Användaren kan inte längre läggas till i team eller grupper.
* Objekt kan inte längre delas med användaren.
* Tar bort associationen mellan användaren och följande objekt:

   * Uppgifter, ärenden, projekt, portfölj
   * Kontrollpaneler

     >[!NOTE]
     >
     >Du förlorar även åtkomsten till anpassade avsnitt som innehöll kontrollpaneler som är kopplade till den borttagna användaren.\
     >Mer information finns i [Hur kommer jag åt en instrumentpanel som innehåller en rapport som ägs av en borttagen användare?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) i artikeln [Rapporterar vanliga frågor och svar](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

   * Uppdateringar
   * Timmar

     >[!NOTE]
     >
     >Objekten finns kvar i Workfront men objektets ägare är nu tom.

* Om användaren har överfört dokument under dokumentområdet i det globala navigeringsfältet, tas även dokumenten bort.
* Om användaren har checkat ut dokument som han/hon äger och dokumenten har överförts till huvuddokumentområdet (som nås från huvudmenyn), tas dokumenten bort med användaren. Mer information om utcheckning av dokument finns i [Checka ut dokument](../../../documents/managing-documents/check-out-documents.md).

Mer information om hur du inaktiverar användare finns i [Inaktivera eller återaktivera en användare](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

Du kan ta bort användare en åt gången permanent eller ta bort flera användare permanent samtidigt. När du tar bort enskilda användare måste du vänta tills borttagningsprocessen har slutförts innan du går vidare till andra aktiviteter i Workfront. Processen att ta bort flera användare samtidigt körs som en bakgrundsprocess, så du kan fortsätta använda Workfront när användarna tas bort.

## Ta bort en eller flera användare

{{step-1-to-users}}

1. Markera minst en användare som du vill ta bort, klicka på Mer-menyn ![Mer-ikon](assets/more-icon.png) och klicka sedan på **Ta bort**.
1. I rutan som visas klickar du på **Ta bort** för att bekräfta borttagningen.

   Processen att ta bort användare körs som en bakgrundsprocess, så du kan fortsätta använda Workfront när användaren eller användarna tas bort.

   Beroende på hur många användare du tar bort kan det ta flera minuter eller t.o.m. några timmar.

   När du har fått en bekräftelse i Workfront om att användarna har tagits bort, kan du fortsätta att se dem i systemet tills borttagningen är klar i bakgrunden.

   Om du upptäcker att en eller flera användare inte kunde tas bort vid ett senare tillfälle kan du försöka ta bort dem en åt gången.
