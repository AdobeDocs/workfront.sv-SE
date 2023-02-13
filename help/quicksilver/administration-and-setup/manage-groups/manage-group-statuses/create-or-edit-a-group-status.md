---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Skapa eller redigera en gruppstatus
description: Som gruppadministratör kan du skapa anpassade statusvärden för en grupp som du hanterar. Detta eliminerar behovet av dussintals företagsövergripande anpassade statusar och ger större självständighet i grupphierarkierna.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: 027d636e8256c6a12d552af736884f6f27886114
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 0%

---

# Skapa eller redigera en gruppstatus

Som gruppadministratör kan du skapa anpassade statusvärden för en grupp som du hanterar. Detta eliminerar behovet av dussintals företagsövergripande anpassade statusar och ger större självständighet i grupphierarkierna.

Du kan också redigera en systemnivåstatus för en grupp som du hanterar om en Workfront-administratör har låst upp statusen. Mer information finns i [Låsta och olåsta statusvärden på systemnivå](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

Om det finns grupper ovanför gruppen kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

>[!NOTE]
>
>Det går inte att visa anpassade gruppstatusar i ett projekt när du visar projektet i en flexibel vy. Endast standardstatus och anpassade låsta statuslägen visas när du visar ett projekt i en flexibel vy. Mer information om hur du anpassar en flexibel vy för ett projekt finns i avsnittet [Skapa eller anpassa en Agile-vy](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) i artikeln [Översikt över vyer i Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Allmän information om status finns i [Översikt över status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

## Skapa eller redigera en status för en grupp

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Grupper** ![](assets/groups-icon.png).

1. Klicka på namnet på gruppen där du vill skapa eller anpassa statusvärden.
1. Klicka på i den vänstra panelen **Status**.

   Om gruppen du visar är en grupp på den översta nivån visas följande i listan:

   * Låsta statusvärden på systemnivå.
   * Anpassade statusvärden har redan skapats för gruppen.

   Om gruppen du visar är en undergrupp innehåller listan dessutom:

   * Låsta statusvärden som tillhör grupperna ovanför undergruppen.
   * Olåsta statusvärden som tillhör grupperna ovanför undergruppen när den skapades.

      När en undergrupp har skapats inkluderas inte olåsta statusar som har skapats i grupperna ovan i undergruppens statuslista. Om någon låser en av dem senare inkluderas den däremot i undergruppens statuslista. Mer information finns i [Hur grupper ärver statusvärden](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).


1. Markera fliken för objekttypen (**Projekt**, **Uppgifter**, eller **Problem**) som du vill associera med statusen.

1. (Villkorligt) Om statusen är ett problem kontrollerar du att **Överordnad lista** är markerat.

   ![](assets/master-list.png)

   Mer information om hur du anpassar de andra problemtyperna (felrapport, Ändra ordning, Problem, Begäran) finns i [Anpassa standardproblemtyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. (Villkorligt) Om du vill skapa en ny status klickar du på **Lägg till en ny status**.

   eller

   Om du vill redigera en befintlig status för du musen över den status du vill redigera och klickar sedan på knappen **Redigera** som visas längst till höger.

   ![](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >Du kan bara redigera en status för din grupp om:
   >      
   >* Du hanterar gruppen som statusen skapades för
   >* En Workfront-administratör låste upp statusen på systemnivå
   >* En gruppadministratör för en grupp ovanför gruppen låste upp statusen

   >      
   >      
   >När du redigerar en befintlig status kan du bara ändra dess namn, beskrivning och färg.
   >
   >När du redigerar en låst status påverkar dina ändringar alla undergrupper som ärver statusen från din grupp.
   >   
   >Omvänt påverkar redigering av olåst status inte de undergrupper som ärvde statusen från din grupp.

1. Ange följande information.

   Om du redigerar en status kan du bara ändra de tre första inställningarna.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Statusnamn</td> 
      <td> <p>Ange ett namn för statusen. Detta är ett obligatoriskt fält.</p> <p>När du skapar ett statusnamn bör du tänka på att andra i systemet kan skapa en status med samma namn. Vi rekommenderar att du använder ett unikt namn för att undvika förvirring när du väljer status i Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>(Valfritt) Skriv en beskrivning av statusen. Detta förmedlar sitt syfte till dem som använder det.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Färg</td> 
      <td> <p>Anpassa statusens färg genom att klicka på färgfältet och välja en färg på panelen Färgruta. Du kan också ange ett hexadecimalt tal i fältet.</p> <p>Statusfärgen visas i det övre högra hörnet av Workfront när en användare tittar på objektet.</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Liknar med</td> 
      <td> <p>Välj ett av alternativen i listan som bäst beskriver statusens funktion. Om statusnamnet till exempel är Klar ska det alternativ som det motsvarar vara Fullständigt.</p> <p>Alla statusvärden måste motsvara ett av dessa alternativ eftersom detta avgör hur statusfunktionen fungerar.</p> <p>Det här alternativet kan inte ändras efter att statusen har skapats.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nyckel</td> 
      <td> <p>Om du skapar en ny status skriver du en kod eller förkortning för statusen eller använder den som har genererats åt dig. Nyckeln måste vara unik i Workfront eftersom den kan användas för rapportering. Om du försöker ange en nyckel som redan används i systemet blir fältet rött.</p> <p>Det kan vara användbart att använda en förkortning som är identifierbar för dem som kommer att använda den.</p> <p>Det här alternativet kan inte ändras efter att statusen har skapats.</p> <p>Du kan inte ändra tangentkoden för statusarna Planning, Current och Complete. Detta är viktigt om du skapar en rapport i textläge.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dölj status</td> 
      <td> <p>(Endast projekt- och aktivitetsstatus)</p> <p>Aktivera det här alternativet om du vill att statusen ska vara dold för användarna. När den är inaktiverad (standardinställningen) kan statusen användas för alla undergrupper under gruppen.</p> <p>Tips: Du kan dölja statusen Problem genom att inaktivera alla fyra problemtyperna (Felrapport, Ändra ordning, Problem, Begäran).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lås för alla grupper</td> 
      <td> 
       <p>Om du låter det här alternativet vara aktiverat kan användarna i din grupp och dess undergrupper se och använda status, och gruppadministratörer kan inte anpassa det för lägre undergrupper.</p> 
       <p>När det här alternativet är inaktiverat kan gruppadministratörer anpassa statusen för undergrupper.</p> 
       <p><b>ANMÄRKNING</b>: Du kan använda både låsta och olåsta lägen i en gruppgodkännandeprocess. Om du skapar en process för gruppgodkännande med olåst gruppstatus kan användarna bifoga godkännandeprocessen till alla projekt, aktiviteter eller utgåvor som är kopplade till gruppen.</p> 
       <p>Mer information om att låsa status finns i <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Låsta och olåsta gruppstatusar</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Klicka **Spara**.

   Statusen är nu tillgänglig för alla projekt som är kopplade till din grupp eller undergrupp. Om du har låst den kan den användas av alla undergrupper.

   Du kan konfigurera statusen till standardstatus för gruppen. Mer information finns i [Använd en anpassad status som standardstatus för en grupp](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Skapa en anpassad status för flera grupper

Om du är Workfront-administratör kan du skapa en anpassad status för flera grupper genom att skapa en systemomfattande status och sedan dölja den statusen för de grupper som inte behöver den.

Om du är gruppadministratör (eller Workfront-administratör) kan du skapa en anpassad status för flera undergrupper i en grupphierarki som du hanterar genom att skapa en status för en grupp på högre nivå och sedan dölja den statusen för alla undergrupper som inte behöver den.

1. Om du är Workfront-administratör skapar du en olåst status för hela systemet enligt beskrivningen i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. I rutan i det övre högra hörnet tar du bort **Systemstatus** börjar du skriva namnet på en grupp där du vill dölja statusen och klickar sedan på namnet när det visas.
1. Håll muspekaren över den status som du vill dölja för gruppen och klicka sedan på **Redigera** när den visas.

   ![](assets/hover-click-edit.jpg)

1. Aktivera **Dölj status** som visas.

   ![](assets/hide-group-status.png)

1. Klicka **Spara**.

   Statusen är nedtonad och inte längre synlig för alla användare i gruppen.

1. Upprepa steg 3 till 5 för att dölja den anpassade statusen för andra grupper som inte behöver den.
