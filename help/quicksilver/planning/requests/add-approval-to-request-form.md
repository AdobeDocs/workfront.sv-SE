---
title: Lägga till ett godkännande i ett begärandeformulär i Adobe Workfront Planning
description: Du kan lägga till en godkännandeprocess i ett Adobe Workfront Planning-begärandeformulär, för att initiera ett godkännande för varje skickad begäran, innan den skapar en post.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Lägga till ett godkännande i ett begärandeformulär i Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

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

* Du kan lägga till en eller flera godkännare i ett begärandeformulär. Du kan lägga till användare och team som godkännare.
* Du kan visa godkännandeinformation för en post som skapats genom att skicka ett begärandeformulär i fälten Godkänd av och Godkänd. Mer information finns i [Skapa fält](/help/quicksilver/planning/fields/create-fields.md).
* När du lägger till flera godkännare i ett begärandeformulär måste alla godkännare acceptera begäran innan en post skapas i Workfront Planning.
* Om alla godkännare godkänner begäran skapas en post för den posttyp som är associerad med förfrågningsformuläret.
* Om minst en godkännare avvisar begäran och alla andra godkänner den, skapas en begäran för området Förfrågningar i Workfront, men ingen post skapas för den posttyp som är associerad med förfrågningsformuläret.
* Det är valfritt att lägga till godkännanden i ett begärandeformulär. Workfront Planning skapar omedelbart en post när en begäran skickas, om begärandeformuläret inte är kopplat till ett godkännande.

<!--

## Add an approval to a request form in the Production environment

1. Start creating a request form for a record type, as described in [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Click **Configuration**.

    The **Configuration** area displays.

    ![Configuration tab](assets/configuration-tab.png)
1. In the **Approvers** field, start typing the name of a user or team that you want to set as an approver, then select it when it displays in the list. 
1. (Optional and conditional) If you have set more than one approver, and only need one approver to make a decision, enable the **Only one decision is required** option.

    (****most of the Note below is duplicated in the Create a request form article***)

      >[!NOTE]
      >
      >
      >* You can add one or several approvers to a request form.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must approve the request before Workfront Planning creates a record.
      >
      >* If at least one approver rejects the request, the request is rejected and the record is not created. The request remains in the Requests area of Workfront.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must make a decision before a request is either approved or rejected.
      >
      >* If a team is set as an approver, only one decision is required from the team.


1. (Optional) Click **Publish** if you have never shared the request form before.

    Or

    Click **Share** to share the form, then **Copy link**. 
1. (Optional) After a user uses the link you share and submits a request, Workfront Planning sends an approval in-app notification and an email to the approvers.

   For information about approving requests, see [Approve a request](/help/quicksilver/planning/requests/approve-request.md).

-->

## Lägga till godkännanderegler i ett begärandeformulär

Godkännanderegler definierar godkännandeprocessen baserat på fältvärden i de skickade begäranden.

Om ett begärandeformulär till exempel har fältet&quot;Kampanjtyp&quot; kan en regel skapas som skickar begäran till en person när fältet har värdet&quot;Digital&quot;, och en annan person när det har värdet&quot;Skriv ut&quot;.

Tänk på följande när du lägger till godkännanderegler:

* Du kan lägga till en eller flera godkännare till en godkännanderegel.
* Om minst en godkännare avvisar begäran, avvisas begäran och posten skapas inte. Begäran finns kvar under Begäranden i Workfront.
* Om du lägger till mer än en godkännare och alternativet Endast ett beslut krävs inte är aktiverat, måste alla godkännare fatta ett beslut innan en begäran godkänns eller avslås.
* Om ett team utses till godkännare krävs endast ett beslut från en medlem i teamet.

Så här anger du godkännanderegler för ett begärandeformulär:

1. Börja skapa ett begärandeformulär för en posttyp, vilket beskrivs i artikeln [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. När formuläret öppnas klickar du på **Inställningar**.

   Fliken **Inställningar** öppnas.

1. Om du vill börja konfigurera godkännanderegler klickar du på ikonen **Godkännanden** ![Godkännanden](assets/approvals-icon-on-form.png) på den vänstra panelen.

1. (Valfritt) Om du vill ange en standardprocess för godkännande lägger du till minst en användare eller grupp i fältet **Godkännare** i området **Standardregel för godkännande** och klickar sedan på kryssrutan **Endast ett beslut krävs** om du vill att posten ska skapas när någon av standardgodkännarna har godkänt den.

   ![Standardområde för godkännanderegel](assets/default-approvers.png)

1. (Valfritt) Börja lägga till godkännanderegler. Gör följande för varje anpassad regel för godkännande:

   1. Klicka på **Lägg till godkännanderegel**
   1. Klicka på platshållartiteln **Namnlös godkännanderegel** och ange ett namn för godkännanderegeln.
   1. Klicka på **Markera ett fält** och markera fältet som aktiverar regeln.
   1. Välj operatorn för regeln. Operatorer varierar beroende på fälttyp.
   1. Om den markerade operatorn kräver ett värde klickar du på plusikonen och lägger till ett eller flera värden.
   1. (Valfritt) Klicka på **Lägg till villkor** om du vill lägga till fler villkor och koppla dem med programsatserna **And** eller **Or** genom att konfigurera ytterligare villkor som i steg C-E.
   1. I området **Åtgärder** i godkännanderegeln lägger du till minst en användare eller grupp som ska anges som godkännare i fältet **Godkännare** när villkoret är uppfyllt.
   1. (Villkorligt och valfritt) Om du vill att posten ska skapas efter att någon av godkännarna har godkänt den, markerar du kryssrutan **Endast ett beslut krävs**. Annars måste alla godkännare fatta beslut om godkännandet innan begäran godkänns eller avslås.

   >[!NOTE]
   >
   >   Tänk på följande när du lägger till godkännanderegler:
   >
   >   * Om bara en standardregel har konfigurerats gäller den för alla skickade begäranden.
   >   * Om en anpassad regel uppfylls används inte standardinställningen i arbetsflödet för godkännande av begäran. Endast matchade anpassade regler gäller för godkännanden och standardregeln ignoreras.
   >   * Om flera anpassade regler uppfylls gäller den första i ordningen. I det här fallet gäller inte standardgodkännandet, om det finns ett.

1. Klicka på **Spara** för att spara godkännandereglerna.
1. (Valfritt) Klicka på **Publicera** om du aldrig har delat begärandeformuläret tidigare.
