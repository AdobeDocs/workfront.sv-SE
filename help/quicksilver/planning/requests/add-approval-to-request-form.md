---
title: Lägga till ett godkännande i ett begärandeformulär i Adobe Workfront Planning
description: Du kan lägga till en godkännandeprocess i ett Adobe Workfront Planning-begärandeformulär, för att initiera ett godkännande för varje skickad begäran, innan den skapar en post.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 2ffd06f2f50d14b6d33bc79c92616ebed1d58fed
workflow-type: tm+mt
source-wordcount: '1195'
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
<p>Alla Workfront-paket och alla Planning-paket</p>
eller
<p>Alla arbetsflödespaket och alla planeringsdokument</p>

<p>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront.</p>
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

## Lägga till ett godkännande i ett begärandeformulär i produktionsmiljön

1. Börja skapa ett begärandeformulär för en posttyp enligt beskrivningen i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Klicka på **Konfiguration**.

   Området **Konfiguration** visas.

   ![Fliken Konfiguration](assets/configuration-tab.png)
1. I fältet **Godkännare** börjar du skriva namnet på en användare eller ett team som du vill ange som godkännare och markerar det sedan när det visas i listan.
1. (Valfritt och villkorligt) Om du har angett mer än en godkännare och bara behöver en godkännare för att fatta ett beslut, aktiverar du alternativet **Endast ett beslut krävs**.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Du kan lägga till en eller flera godkännare i ett begärandeformulär.
   >
   >* Om du lägger till mer än en godkännare och alternativet Endast ett beslut krävs inte är aktiverat, måste alla godkännare godkänna begäran innan Workfront Planning skapar en post.
   >
   >* Om minst en godkännare avvisar begäran, avvisas begäran och posten skapas inte. Begäran finns kvar under Begäranden i Workfront.
   >
   >* Om du lägger till mer än en godkännare och alternativet Endast ett beslut krävs inte är aktiverat, måste alla godkännare fatta ett beslut innan en begäran godkänns eller avslås.
   >
   >* Om ett team utses till godkännare krävs endast ett beslut från teamet.


1. (Valfritt) Klicka på **Publicera** om du aldrig har delat begärandeformuläret tidigare.

   eller

   Klicka på **Dela** för att dela formuläret och sedan på **Kopiera länk**.
1. (Valfritt) När en användare har använt länken som du delar och skickar en begäran skickar Workfront Planning ett meddelande om godkännande i appen och ett e-postmeddelande till godkännarna.

   >[!NOTE]
   >
   >   Din organisations instans av Workfront måste vara registrerad på Adobe Unified Experience för att användare ska kunna ta emot e-post och meddelanden i appen.


   Mer information om hur du godkänner begäranden finns i [Godkänn en begäran](/help/quicksilver/planning/requests/approve-request.md).

<div class="preview">

## Lägga till godkännanderegler i ett begärandeformulär

>[!NOTE]
>
>Den här funktionen är bara tillgänglig i förhandsvisningsmiljön.

Godkännanderegler definierar godkännandeprocessen baserat på fältvärden som används i de skickade förfrågningarna.

Om ett begärandeformulär till exempel har fältet&quot;Kampanjtyp&quot; kan en regel skapas som skickar begäran till en person när fältet har värdet&quot;Digital&quot;, och en annan person när det har värdet&quot;Skriv ut&quot;.

Tänk på följande när du lägger till godkännanderegler:

* Du kan lägga till en eller flera godkännare till en godkännanderegel.
* Om minst en godkännare avvisar begäran, avvisas begäran och posten skapas inte. Begäran finns kvar under Begäranden i Workfront.
* Om du lägger till mer än en godkännare och alternativet Endast ett beslut krävs inte är aktiverat, måste alla godkännare fatta ett beslut innan en begäran godkänns eller avslås.
* Om ett team utses till godkännare krävs endast ett beslut från teamet.

Mer information om hur du lägger till godkännanden finns i [Lägga till godkännande i ett begärandeformulär](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

Så här anger du godkännanderegler för ett begärandeformulär:

1. Börja skapa ett begärandeformulär för en posttyp enligt beskrivningen i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Klicka på **Inställningar**.

   Fliken Inställningar visas.

1. Om du vill börja konfigurera godkännanderegler klickar du på ikonen för godkännande ![](assets/approvals-icon-on-form.png) i den vänstra navigeringen.

1. (Valfritt) Om du vill ange en standardprocess för godkännande lägger du till minst en användare eller grupp i fältet **Godkännare** i området Standardregel för godkännande. Klicka sedan på kryssrutan **Endast ett beslut krävs** om du vill att posten ska skapas när någon av standardgodkännarna har godkänt den.

   ![Standardområde för godkännanderegel](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. (Valfritt) Gör följande för varje ytterligare regel för godkännande:

   1. Klicka på **Lägg till godkännanderegel**
   1. Klicka på platshållartiteln &quot;Namnlös godkännanderegel&quot; och ange ett namn för godkännanderegeln.
   1. Klicka på **Markera ett fält** och markera fältet som aktiverar regeln.
   1. Välj operatorn för regeln. Operatorer varierar beroende på fälttyp.
   1. Om den markerade operatorn kräver ett värde klickar du på plusikonen och lägger till ett eller flera värden.
   1. (Valfritt) Lägg till fler villkor med AND eller OR genom att klicka på Lägg till villkor och konfigurera det ytterligare villkoret som i steg C-E.
   1. I området Åtgärder i godkännanderegeln i fältet **Godkännare** lägger du till minst en användare eller grupp som ska anges som godkännare när villkoret är uppfyllt.
   1. 
      1. (Villkorligt) Om du vill att posten ska skapas efter att någon av godkännarna har godkänt den, markerar du kryssrutan **Endast ett beslut krävs**.

1. Klicka på **Spara** för att spara godkännandereglerna.
1. (Valfritt) Klicka på **Publicera** om du aldrig har delat begärandeformuläret tidigare.

</div>
