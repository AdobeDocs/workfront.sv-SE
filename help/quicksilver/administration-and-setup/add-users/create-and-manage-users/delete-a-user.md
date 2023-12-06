---
title: Ta bort användare
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: När en användare lämnar din organisation kan ta bort den användaren från Workfront, men vi rekommenderar att du inaktiverar användare i stället för att ta bort dem.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Ta bort användare

När en användare lämnar organisationen kan du ta bort den användaren från Adobe Workfront.

>[!IMPORTANT]
>
>* Om du tar bort en användare från systemet tas även information som är kopplad till användaren bort. Vi rekommenderar att du inaktiverar användare i stället för att ta bort dem. Mer information finns i [Inaktivera eller återaktivera en användare](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* Det förfarande som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Admin Console. Om du har anslutit dig till Adobe Admin Console måste du utföra den här åtgärden via Adobe Admin Console.
>
>Ta bort en användare från [!DNL Adobe Admin Console] inaktiverar användaren i [!DNL Workfront], men tar inte bort dem från [!DNL Workfront].
>
>  Instruktioner om hur du tar bort en användare i Adobe Admin Console finns i avsnittet&quot;Ta bort användare permanent&quot; i artikeln [Hantera användare individuellt](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) eller kontakta Adobe Admin Console Administrator.
>
>  En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns på [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

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
   <td> <p>Du måste ha något av följande:</p> 
    <ul> 
     <li> <p>Åtkomstnivån Systemadministratör. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>. </p> </li> 
     <li> <p><b>Användare</b> ange din åtkomstnivå som <b>Redigera</b> åtkomst, med <b>Skapa</b> och minst en av de två <b>Användaradministratör</b> alternativ aktiverade under <b>Finjustera inställningarna</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>av dessa två alternativ, om användaren <b>Administratör (gruppanvändare)</b> är aktiverat måste du vara gruppadministratör för en grupp där användaren är medlem.</p> <p>Mer information om <b>Användare</b> ange en åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst för användare</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Ta bort kontra inaktivera en användare

När du inaktiverar en användare händer följande:

* Tar bort användarens licenser till både Workfront och Workfront Proof om Workfront-komponenten är kopplad till ditt Workfront-konto. Mer information om Workfront Proof finns i [Workfront-korrektur: artikelindex](../../../workfront-proof/workfront-proof.md).
* Användaren kan inte längre tilldelas arbete.
* Användaren kan inte längre läggas till i uppdateringar.
* Användaren kan inte längre läggas till i team eller grupper.
* Objekt kan inte längre delas med användaren.
* Deras koppling till följande objekt förblir intakt:

   * Uppgifter, ärenden, projekt, portfolior
   * Kontrollpaneler

     >[!NOTE]
     >
     >Om du inaktiverar en användare och inte längre kan visa rapporter eller kontrollpaneler som är kopplade till en användare, kan du behöva uppdatera **Kör den här rapporten med åtkomsträttigheterna för:** fält.\
     >Mer information finns i [Varför kan jag inte komma åt en rapport som ägs av en inaktiverad användare?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) i [Vanliga frågor och svar om rapporter](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) artikel.

   * Dokument
   * Uppdateringar
   * Timmar

* Om användaren har checkat ut dokument förblir dokumenten utcheckade när du inaktiverar dem. Endast en Workfront-administratör kan checka in dem igen. Mer information om utcheckning av dokument finns i [Checka ut dokument](../../../documents/managing-documents/check-out-documents.md).

Om du tar bort en användare händer följande:

* Tar bort användarens licenser till både Workfront och Workfront Proof om Workfront-komponenten är kopplad till ditt Workfront-konto. Mer information om Workfront Proof finns i [Workfront-korrektur: artikelindex](../../../workfront-proof/workfront-proof.md).
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
     >Mer information finns i [Hur får jag åtkomst till en instrumentpanel som innehåller en rapport som ägs av en borttagen användare?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) i [Vanliga frågor och svar om rapporter](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) artikel.

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

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn.

1. Klicka **Användare**.
1. Markera minst en användare som du vill ta bort och klicka på menyn Mer ![](assets/more-icon.png)och sedan klicka **Ta bort**.
1. Klicka i rutan som visas **Ta bort** för att bekräfta borttagningen.

   Processen att ta bort användare körs som en bakgrundsprocess, så du kan fortsätta använda Workfront när användaren eller användarna tas bort.

   Beroende på hur många användare du tar bort kan det ta flera minuter eller t.o.m. några timmar.

   När du har fått en bekräftelse i Workfront om att användarna har tagits bort, kan du fortsätta att se dem i systemet tills borttagningen är klar i bakgrunden.

   Om du upptäcker att en eller flera användare inte kunde tas bort vid ett senare tillfälle kan du försöka ta bort dem en åt gången.
