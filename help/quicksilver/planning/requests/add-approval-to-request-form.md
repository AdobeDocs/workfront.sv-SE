---
title: Lägga till ett godkännande i ett begärandeformulär i Adobe Workfront Planning
description: Du kan lägga till en godkännandeprocess i ett Adobe Workfront Planning-begärandeformulär, för att initiera ett godkännande för varje skickad begäran, innan den skapar en post.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: c06baa45e52d77463f9f886b6f6eae4ff68e4ccd
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

---

# Lägga till ett godkännande i ett begärandeformulär i Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Du kan lägga till en godkännandeprocess i ett Adobe Workfront Planning-begärandeformulär, för att initiera ett godkännande för varje skickad begäran, innan den skapar en post.

I den här artikeln beskrivs hur en arbetsytehanterare kan lägga till ett godkännande i ett begärandeformulär som är kopplat till en posttyp.

Mer information om hur du skapar ett begärandeformulär i Workfront Planning finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Mer information om hur du skickar en begäran till en posttyp för att skapa en post finns i [Skicka Adobe Workfront Planning-begäranden för att skapa poster](/help/quicksilver/planning/requests/submit-requests.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront</p></td> 
   <td> 
<ul><li><p>Alla Workfront-paket</p></li>
Och
<li><p>Planeringspaket</p></li></ul>
eller
<ul><li><p>Alla arbetsflödespaket</p></li>
Och
<li><p>Planeringspaket</p></li></ul>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektbehörigheter</p></td> 
   <td>   <p>Hantera behörigheter till en arbetsyta och posttyp </a> </p>  
   <p>Systemadministratörer har behörighet till alla arbetsytor, inklusive de som de inte skapade</p>  </td> 
  </tr>  
</tbody> 
</table>

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Att tänka på när du lägger till godkännanden i ett begärandeformulär

* Du kan lägga till en eller flera godkännare i ett begärandeformulär. Du kan bara lägga till användare som godkännare.
* Du kan visa godkännandeinformation för en post som skapats genom att skicka ett begärandeformulär i fälten Godkänd av och Godkänd. Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).
* När du lägger till flera godkännare i ett begärandeformulär måste alla godkännare acceptera begäran innan en post skapas i Workfront Planning.
* Om alla godkännare godkänner begäran skapas en post för den posttyp som är associerad med förfrågningsformuläret.
* Om minst en godkännare avvisar begäran och alla andra godkänner den, skapas en begäran för området Förfrågningar i Workfront, men ingen post skapas för den posttyp som är associerad med förfrågningsformuläret.
* Det är valfritt att lägga till godkännanden i ett begärandeformulär. Workfront Planning skapar omedelbart en post när en begäran skickas, om begärandeformuläret inte är kopplat till ett godkännande.

## Lägga till ett godkännande i ett begärandeformulär

1. Börja skapa ett begärandeformulär för en posttyp enligt beskrivningen i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Klicka på **Konfiguration**.

   Området **Konfiguration** visas.

   ![Fliken Konfiguration](assets/configuration-tab.png)
1. Klicka på listruteikonen i fältet **Godkännare** och välj en eller flera användare eller team i listan

   eller

   Börja skriva namnet på en användare eller ett team som du vill ange som godkännare och markera det sedan när det visas i listan.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Du kan lägga till en eller flera godkännare i ett begärandeformulär.
   >
   >* Om du lägger till fler än en godkännare måste alla godkännare godkänna begäran innan Workfront Planning skapar en post.
   >
   >* Om minst en godkännare avvisar begäran, avvisas begäran och posten skapas inte. Begäran finns kvar på fliken Planering i avsnittet Skickat i området Begäranden i Workfront.
   >
   >* Alla godkännare måste fatta ett beslut innan en begäran godkänns eller avslås.
   >
   >* Om ett team utses till godkännare krävs endast ett beslut från teamet.


1. (Valfritt) Klicka på **Publicera** om du aldrig har delat begärandeformuläret tidigare

   eller

   Klicka på **Dela** för att dela formuläret och sedan på **Kopiera länk**.
1. (Valfritt) När en användare har använt länken som du delar och skickar en begäran skickar Workfront Planning ett meddelande om godkännande i appen och ett e-postmeddelande till godkännarna.

   >[!NOTE]
   >
   >   Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att användare ska kunna ta emot e-post och meddelanden i appen.


   Mer information om hur du godkänner begäranden finns i [Godkänn en begäran](/help/quicksilver/planning/requests/approve-request.md).
