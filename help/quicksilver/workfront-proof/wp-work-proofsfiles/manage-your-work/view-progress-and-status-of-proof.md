---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Visa status och förlopp för ett korrektur i  [!DNL Workfront Proof]
description: Bevisförloppet visar det arbete som utförts med ett korrektur från den tidpunkt då du skickar beviset till granskarna tills de fattar ett beslut om beviset.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 8fd85595-1403-490e-9d52-2ba5b01457b7
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# Visa status och förlopp för ett korrektur i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

## Förstå korrekturstatus

Bevisförloppet visar det arbete som utförts med ett korrektur från den tidpunkt då du skickar beviset till granskarna tills de fattar ett beslut om beviset.

* [Förloppsikoner](#progress-icons)
* [Status för korrektur](#levels-of-proof-progress)

### Förloppsikoner {#progress-icons}

Förloppsikonerna, S, O, C och D, visas i förloppsindikatorn och visar korrekturförloppet.

![proof_edit_existing_progress.png](assets/proof-edit-existing-progress-350x78.png)

De innehåller följande uppgifter om ett bevis:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Förloppsikon</strong> </p> </td> 
   <td> <p><strong>Beskrivning</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt="proof_progress_sent_icon.png"> </p> </td> 
   <td> <p><strong>Skickat</strong>. Beviset har skickats till granskarna.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-opened-icon.png" alt="proof_progress_opened_icon.png"> </p> <p> </p> </td> 
   <td> <p><strong>Öppnad</strong>. En granskare har öppnat sidan med korrekturinformation eller öppnat själva korrekturet i korrekturläsaren.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-comment-icon.png" alt="proof_progress_comment_icon.png"> </p> </td> 
   <td> <p><strong>Kommentarer</strong>. Granskare (användare som kan kommentera) har kommenterat korrekturet.</p> <p>Ikonen visas inte om ingen granskare har angetts som provtryckare.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt="proof_progress_Decision_icon.png"> </p> </td> 
   <td> <p><strong>Beslut</strong>. En granskare har fattat ett beslut om beviset.</p> <p>Om inga godkännare (beslutsfattare) har angetts för beviset visas inte den här ikonen. </p> </td> 
  </tr> 
 </tbody> 
</table>

De här ikonerna kan visas i följande färger för att visa viss information om korrekturets förlopp:

* **Grön**. Slutförd.
* **Vit**. Inte komplett.
* **Orange**. Inte komplett och tidsgränsen är mindre än 24 timmar.
* **Röd**. Inte komplett och förbi deadline.

### Status för korrektur {#levels-of-proof-progress}

Workfront Proof använder förloppsikonerna för att spåra korrekturets förlopp på följande nivåer:

* För varje granskare, baserat på den personens aktivitet på beviset.
* För varje fas baseras granskarens förlopp på den scen som ligger längst bak i korrekturprocessen. Mer information finns i [Översikt över automatiska arbetsflödessteg](../../../review-and-approve-work/proofing/proofing-overview/stages.md).
* Beviset baseras på förloppet för den scen (grupp av granskare) som ligger längst bak i korrekturprocessen.

Ett exempel på hur [!DNL Workfront Proof] avgör förloppet med den granskare eller scen som ligger längst bak är om tre granskare måste fatta ett beslut i ett korrektur. Om två av dem har fattat sitt beslut men den tredje inte har gjort det, visar inte förloppsindikatorn för beviset D i grönt på grund av det utestående beslutet.

Om inställningen [!UICONTROL Primary Decision Maker] väljs på ett korrektur och den primära beslutsfattaren skickar ett beslut, blir D:et i korrekturets förloppsindikator grönt för alla granskare eftersom inga andra beslut krävs.

Om inställningen [!UICONTROL Only One Decision Required] är markerad på ett korrektur och en granskare skickar ett beslut, blir D i förloppsindikatorn grönt för alla granskare eftersom inga andra beslut krävs.

## Förstå korrekturstatus

Korrekturstatusen visar statusen för de beslut som krävs för beviset.

![proof_edit_existing_status.png](assets/proof-edit-existing-status-350x78.png)\
Standardstatusalternativen är:

* Väntande
* Godkänd
* Godkänd med ändringar
* Ändringar krävs
* Inte relevant

Om anpassade beslut har konfigurerats i ditt konto återspeglar statusalternativen dina anpassade beslutsinställningar.

Bevisets status styrs av deltagaren i det värsta fallet. Anta till exempel att det finns tre beslut för korrekturet: två har statusen **Godkänd** och en har statusen **Avvisad**. Det &quot;värsta fallet&quot;-beslut som avvisats överstyr de andra besluten och korrekturets totala status visas som **Avvisad**.

## Visningsförlopp och status {#viewing-progress-and-status}

Du kan visa förlopp och status för korrektur, faser och granskare på varje fas.

* [Korrektursammanfattning](#proof-summary)
* [Menyn Scenåtgärder](#stage-actions-menu)
* [I avsnittet [!UICONTROL Summary] kan du även komma åt granskarens åtgärdsmenyer, förutsatt att du har redigeringsbehörighet för korrekturet. Mer information finns i Korrekturbehörighetsprofiler i Workfront Proof och Hantera profilroller i Workfront Proof. Menyn [!UICONTROL Reviewer actions] (1) visas när du hovrar över granskarens information och gör att du kan:](#in-the-summary-section-you-can-also-access-the-reviewer-actions-menus-provided-you-have-edit-rights-on-the-proof-for-more-information-see-proof-permissions-profiles-in-workfront-proof-and-manage-proof-roles-in-workfront-proof-the-reviewer-actions-menu-1-appears-when-you-hover-over-the-reviewer-s-details-and-allows-you-to)
* [Korrekturåtgärder-menyn](#proof-actions-menu)

### Korrektursammanfattning {#proof-summary}

Varje korrektur i mappen har en expanderbar sammanfattning som gör att du snabbt kan visa och redigera korrekturinformationen.

Så här visar eller döljer du sammanfattningen:

1. Klicka på pilen till vänster om korrekturet på kontrollpanelen eller i valfri listvy.

![Summary_expandable.png](assets/summary-expandable-350x68.png)

Sammanfattningen innehåller följande:

* Arbetsflöde (2)
* Version (3)
* Mapp (4)
* Delstat (5)\
   ![summary_2.png](assets/summary-2-350x160.png)

I sammanfattningen kan du visa och redigera följande information om ditt korrektur:

* Bevis på framsteg (1)
* Förlopp för varje fas (2)
* Tidsgräns för scenen (3)
* Information om granskare:

   * Antal kommentarer och svar från varje granskare (4)
   * Varje granskares förlopp (5)
   * Beslut (om ett beslut innehåller en elektronisk signatur visas en ikon bredvid beslutet som anger detta.) (6)
   * Bevisets roll (7)
   * Inställningar för e-postavisering (8)

>[!NOTE]
>
>Din möjlighet att redigera korrekturinformationen beror på dina rättigheter för korrekturet (se [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) och [Manage Proof Roles in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![summary_details_3.png](assets/summary-details-3-350x160.png)

### [!UICONTROL Stage Actions]-menyn  {#stage-actions-menu}

Varje steg i arbetsflödet har en separat meny, som gör att du kan utföra gruppåtgärder som är relaterade till granskarna i det steget.

Menyn [!UICONTROL Stage actions] visas när du hovrar över scenavsnittet (1) och gör att du kan

* [!UICONTROL Message all] (2)
* [!UICONTROL Share] (3)
* [!UICONTROL Delete stage] (4)

>[!NOTE]
>
>Vilka alternativ som är tillgängliga beror på dina rättigheter för korrekturet (se [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) och [Manage Proof Roles in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![Stage_actions_menu.png](assets/stage-actions-menu-350x161.png)

I avsnittet Sammanfattning kan du även komma åt granskarnas åtgärdsmenyer, förutsatt att du har redigeringsbehörighet för korrekturet. Mer information finns i [Korrekturbehörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) och [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md). Menyn för granskningsåtgärder (1) visas när du hovrar över informationen i granskaren och gör att du kan:

* Skicka ett meddelande till granskaren (2)
* Redigera information om granskare (3)- gör att du kan redigera visningsnamn, korrekturroll och e-postavisering för den granskaren
* Gör dem till ägare av beviset (4)
* Gör dem till den primära beslutsfattaren (5)
* Ta bort från korrekturet (6)

>[!NOTE]
>
>Hur dessa alternativ visas beror på dina rättigheter för korrekturet (se [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) och [Manage Proof Roles in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![Reviewer_actions_menu.png](assets/reviewer-actions-menu-350x135.png)

### Korrekturåtgärder-menyn {#proof-actions-menu}

Varje korrektur har också en meny (1) som gör att du kan utföra följande åtgärder:

* Du kan öppna sidan Korrekturinformation (2)
* Dela korrekturet med andra (3)
* Skicka ett meddelande till granskarna (4)
* Skapa en ny version av korrekturet (5)
* Kopiera korrekturet (6)
* Hämta originalfilen (7)
* Dela korrekturlänkar (8)
* Skriv ut kommentarer (9)
* Begär en Excel-sammanfattning av korrekturet (10)
* Lås korrektur (11)
* Ta bort korrektur (12)

![Korrektur_actions_menu__1_.png](assets/proof-actions-menu--1--350x158.png)

>[!NOTE]
>
>Vilka alternativ som är tillgängliga beror på dina rättigheter för korrekturet (se [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) och [Manage Proof Roles in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

Mer information om hur du visar korrekturförlopp och status i [!DNL Workfront] finns i [Visa förlopp och status](#viewing-progress-and-status).

Information om visningsförloppet och statusen i Desktop Proofing Viewer finns i [Granska ett arbetsflöde i korrekturläsaren](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-workflow.md).
