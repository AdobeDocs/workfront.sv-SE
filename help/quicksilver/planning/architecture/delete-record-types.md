---
title: Ta bort posttyper
description: Du kan ta bort posttyper när de inte längre är relevanta. När du tar bort posttyper tas även all information som är kopplad till posttyperna bort, som poster, fält och vyer.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 5bccad02f90fd99135b50c5a929913b16cc5b809
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 0%

---


<!--keep the global record type reference in yellow till January 2026-->

# Ta bort posttyper

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Du kan ta bort posttyper när de inte längre är relevanta.

Om du tar bort posttyper tas även all information som är kopplad till posttyperna bort. Mer information finns i avsnittet [Att tänka på när du tar bort posttyper](#considerations-when-deleting-record-types) i den här artikeln.

Mer information om posttyper finns i [Översikt över posttyper](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul> 
<li><p>Alla Workfront- och Planning-paket</p></li>
eller
<li><p>Alla arbetsflöden och alla planeringsdokument</p></li></ul>

<p>Så här tar du bort globala posttyper:</p>
<ul><li><p>Alla Workfront-paket och ett Planning Plus-paket</p></li>
eller
<li><p>Alla arbetsflöden och ett Planning Prime- eller Ultimate-paket</p></li></ul>

<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta</p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 
-->


## Att tänka på när du tar bort posttyper

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Du kan bara ta bort posttyper från arbetsytor som du har behörigheten Hantera.
* När du tar bort posttyper tas följande information bort som är kopplad till dem:

   * Alla poster av den typen.
   * Alla fält som är associerade med posttypen.
   * Alla vyer (inklusive filter, grupperingar och sorteringsvillkor) av posttypen.
* Posttypen tas bort från alla användare som använder arbetsytan.
* Du kan inte återställa borttagna posttyper eller deras information.
* Vi rekommenderar att du återskapar de fält och poster som är kopplade till den posttyp som du vill ta bort på en annan posttyp innan du tar bort dem.

* Du kan inte ta bort en global posttyp som har lagts till i andra arbetsytor.

  Mer information finns i avsnittet [Ta bort globala posttyper](#delete-global-record-types) i den här artikeln.

## Ta bort posttyper

{{step1-to-planning}}

1. Klicka på arbetsytan vars posttyper du vill ta bort,

   eller

   Utöka den nedåtriktade pilen till höger om namnet på en befintlig arbetsyta i en arbetsyta, sök efter en arbetsyta och markera den när den visas i listan.

   Arbetsytan öppnas och posttyperna visas.
1. Gör något av följande:

   * Håll markören över posttypkortet, klicka på menyn **Mer** och sedan på **Ta bort**.
   * Klicka på kortet för den posttyp som du vill ta bort och klicka på menyn **Mer** ![Mer](assets/more-menu.png) till höger om posttypens namn på posttypssidan och klicka sedan på **Ta bort**.

     >[!TIP]
     >
     >Du kan inte ta bort en global posttyp från den sekundära arbetsytan där den lades till från posttypssidan. Du kan bara ta bort den från posttypskortet på arbetsytan.

     ![Ta bort posttypsbekräftelse permanent](assets/permanently-delete-record-type-confirmation.png)


1. Skriv **delete** i bekräftelserutan och klicka sedan på **Ta bort permanent**. Detta är inte skiftlägeskänsligt.

   Den valda posttypen, tillsammans med deras fält, associerade poster och vyer, tas bort och kan inte återställas.

## Ta bort globala posttyper

Följande scenarier gäller när globala posttyper tas bort:

* Om en posttyp som konfigurerats som global ännu inte har lagts till på en annan arbetsyta kan du ta bort den från den ursprungliga arbetsytan.

* Om en posttyp som konfigurerats som en global posttyp har lagts till i minst en annan arbetsyta, kan du inte ta bort den från den ursprungliga arbetsytan. Du måste först ta bort (genom att ta bort) den globala posttypen från de sekundära arbetsytorna där de lades till och sedan ta bort den globala posttypen permanent från den ursprungliga arbetsytan.

### Ta bort en global posttyp från den ursprungliga arbetsytan

Du kan ta bort en posttyp från den ursprungliga arbetsytan om den inte längre är relevant.

Alla poster och fält tas också bort och kan inte återställas.

1. Gå till den globala posttypen på den ursprungliga arbetsytan.

1. (Villkorligt) Gör något av följande, beroende på om den globala posttypen har lagts till i sekundära arbetsytor:

   * Om posttypen inte har lagts till på en sekundär arbetsyta klickar du på menyn **Mer** ![Mer](assets/more-menu.png) på posttypens kort, eller till höger om posttypens namn på sidan, och klickar sedan på **Ta bort**.
   * Om posttypen lades till i minst en annan sekundär arbetsyta går du först till den sekundära arbetsytan och tar bort den globala posten från den arbetsytan.

     Mer information finns i avsnittet [Ta bort en global posttyp från en sekundär arbetsyta](#delete-a-global-record-type-from-a-secondary-workspace) i den här artikeln.

1. (Villkorligt) Fortsätt ta bort posttypen enligt beskrivningen i avsnittet [Ta bort posttyper](#delete-record-types-1) i den här artikeln.

   Följande saker händer:

   * Den globala posttypen tas bort från den ursprungliga arbetsytan och posttypen, dess poster och fält kan inte återställas.
   * Alla globala poster från de sekundära arbetsytorna och deras poster tas också bort från den här arbetsytan.

### Ta bort en global posttyp från en sekundär arbetsyta

Du kan ta bort en posttyp som du har lagt till från en annan arbetsyta om den inte längre behövs.

Tänk på följande:

* När du tar bort en global posttyp från en sekundär arbetsyta finns posttypen kvar på den ursprungliga arbetsytan.

* När du tar bort en global posttyp från en sekundär arbetsyta tas även följande bort:

   * Posterna som läggs till från den sekundära arbetsytan tas bort från den sekundära arbetsytan och från den ursprungliga arbetsytan, och kan inte återskapas.

  <!--Coming later: * The fields added from the secondary workspace.-->

* Det går inte att återställa globala posttyper som har tagits bort från deras sekundära arbetsytor.

* Den ursprungliga posttypen finns kvar på den ursprungliga arbetsytan och på andra arbetsytor där den har lagts till.

* Vyer som har lagts till i posttypen på den sekundära arbetsytan bevaras och visas i andra arbetsytor, om de delas med dig.

Ta bort en global posttyp från en sekundär arbetsyta:

1. Gå till den globala posttypen på den sekundära arbetsytan.

1. (Valfritt) Klicka på menyn **Mer** ![Mer &#x200B;](assets/more-menu.png) på posttypens kort och klicka sedan på **Ta bort**.
1. (Villkorligt) Skriv **delete** i det angivna fältet och klicka sedan på **Ta bort permanent**.

   ![Ta bort bekräftelseruta för den sekundära globala posttypen](assets/delete-secondary-global-record-type.png)

   Följande saker händer:

   * Posttypen som skapas från en global posttyp tas bort från den valda sekundära arbetsytan.
   * Den ursprungliga posttypen med dess fält finns kvar på den ursprungliga arbetsytan.
   * Posttypen finns kvar på alla andra arbetsytor där den har lagts till.
   * Posterna <!--and fields--> som lagts till i posttypen från den sekundära arbetsytan tas bort. Alla andra poster som läggs till från ytterligare arbetsytor där den globala posttypen lades till bevaras på deras respektive arbetsytor och på den ursprungliga arbetsytan. &lt;!—Fält bevaras i de arbetsytor där de lades till.


