---
product-area: documents
navigation-topic: approvals
title: Skapa en arbetsflödesmall för godkännande av dokument
description: Du kan skapa godkännandemallar för att effektivisera godkännandeprocessen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Skapa en arbetsflödesmall för godkännande av dokument

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Den är bara tillgänglig i sandlådemiljön för förhandsgranskning.</span>

I Workfront Setup kan användare med en standardlicens skapa återanvändbara godkännandemallar. När du har skapat mallar för godkännande kan du använda dem på resurser i dokumentområdet för ett projekt, en uppgift eller en utgåva.

>[!IMPORTANT]
>
>Innehållet i den här artikeln hänvisar till den uppdaterade funktionen för dokumentgodkännande som bara är tillgänglig för specifika konton. Mer information om standardgodkännandeprocesser finns i artiklarna i [Arbetsgodkännanden](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Standard</p> 
   <p>Plan</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++




## Skapa en godkännandemall i produktionsmiljön

{{step-1-to-setup}}

1. Klicka på **Granska och godkänn** > **Godkännandemallar** i den vänstra panelen.
1. Klicka på **Ny mall** till höger på sidan.
1. Ange följande information:

   | Mallnamn | Börja skriva ett namn för mallen. |
   |----------------------------|---|
   | **(Valfritt) Tidsram** | Ange tidsramen i dagar. Tidsgränsen för godkännande beräknas från det här fältet när mallen tillämpas på en tillgång. |
   | **Lägg till godkännare eller granskare** | Börja skriva namnet på användare eller team och ange dem sedan som granskare eller godkännare. |

1. Klicka på **Spara**.



<div class="preview">

## Skapa en godkännandemall i förhandsvisningsmiljön

{{step-1-to-setup}}

1. Klicka på **Granska och godkänn** > **Godkännandemallar** i den vänstra panelen.
1. Klicka på **Ny mall** till höger på sidan.

1. Fyll i följande uppgifter:

   <table>
     <tr>
   <td><strong>Mallnamn</strong></td>
   <td>Lägg till ett mallnamn. </td>
   </tr>
   <tr>
   <td><strong>Scennamn</strong></td>
   <td>Lägg till ett scennamn. Du kan ändra namnet till något mer beskrivande, till exempel <em>Inledande granskning</em> eller <em>Slutligt godkännande</em>.</td>
   </tr>
   <tr>
   <td><strong>Lägg till namn eller e-post</strong></td>
   <td>Börja skriva ett användar- eller teamnamn som ska läggas till som godkännare eller granskare. Om du bara har granskare meddelas de och har möjlighet att slutföra granskningen, men inget beslut krävs eller fattas.</td>
   </tr>
   <tr>
   <td><strong>Ett beslut krävs (valfritt)</strong></td>
   <td>Den första personen som fattar ett beslut slutför steget.</td>
   </tr>
   <tr>
   <td><strong>Dagar till förfallodatum</strong></td>
   <td>Välj hur många arbetsdagar som ska förflyta innan godkännandet förfaller efter att en fas har aktiverats.</td>
   </tr>
   </table>

1. (Valfritt) Upprepa föregående steg om du vill lägga till ytterligare steg.

   >[!NOTE]
   >
   >Om du lägger till flera faser fortsätter arbetsflödet för godkännande i den ordning som faserna listas. När alla nödvändiga beslut fattas börjar nästa steg och den föregående fasen låses.

   ![Dokumentinformation](assets/new-stage.png)

1. Klicka på **Spara**.

När mallen har skapats kan den tillämpas på dokument i dokumentdelen av ett projekt, en uppgift eller en utgåva för att starta den formella gransknings- och godkännandeprocessen i Workfront.

</div>


<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
