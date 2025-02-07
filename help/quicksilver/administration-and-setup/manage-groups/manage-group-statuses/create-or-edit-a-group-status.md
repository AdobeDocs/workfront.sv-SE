---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Skapa eller redigera en gruppstatus
description: Som gruppadministratör kan du skapa anpassade statusvärden för en grupp som du hanterar. Detta eliminerar behovet av dussintals företagsövergripande anpassade statusar och ger större självständighet i grupphierarkierna.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1344'
ht-degree: 0%

---

# Skapa eller redigera en gruppstatus

Som gruppadministratör kan du skapa anpassade statusvärden för en grupp som du hanterar. Detta eliminerar behovet av dussintals företagsövergripande anpassade statusar och ger större självständighet i grupphierarkierna.

Du kan också redigera en systemnivåstatus för en grupp som du hanterar om en Workfront-administratör har låst upp statusen. Mer information finns i [Låsta och olåsta statusvärden på systemnivå](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

Om det finns grupper ovanför gruppen kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

>[!NOTE]
>
>Det går inte att visa anpassade gruppstatusar i ett projekt när du visar projektet i en flexibel vy. Endast standardstatus och anpassade låsta statuslägen visas när du visar ett projekt i en flexibel vy. Mer information om hur du anpassar en flexibel vy för ett projekt finns i avsnittet [Skapa eller anpassa en Agile-vy](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) i artikeln [Skapa eller redigera vyer i Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

Allmän information om status finns i [Statusöversikt](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Du måste vara gruppadministratör för gruppen eller systemadministratör.</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa eller redigera en status för en grupp

{{step-1-to-setup}}

1. Klicka på **Grupper** ![Grupper](assets/groups-icon.png) i den vänstra panelen.

1. Klicka på namnet på gruppen där du vill skapa eller anpassa statusvärden.
1. Klicka på **Status** i den vänstra panelen.

   Om gruppen du visar är en grupp på den översta nivån visas följande i listan:

   * Låsta statusvärden på systemnivå.
   * Anpassade statusvärden har redan skapats för gruppen.

   Om gruppen du visar är en undergrupp innehåller listan dessutom:

   * Låsta statusvärden som tillhör grupperna ovanför undergruppen.
   * Olåsta statusvärden som tillhör grupperna ovanför undergruppen när den skapades.

     När en undergrupp har skapats inkluderas inte olåsta statusar som har skapats i grupperna ovan i undergruppens statuslista. Om någon låser en av dem senare inkluderas den däremot i undergruppens statuslista. Mer information finns i [Hur grupper ärver statusvärden](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

1. Välj fliken för den objekttyp (**Projekt**, **Åtgärder** eller **Problem**) som du vill associera med statusen.

1. (Villkorligt) Om statusen är ett problem kontrollerar du att **Huvudlista** är markerad.

   ![Huvudlista](assets/master-list.png)

   Mer information om hur du anpassar de andra problemtyperna (felrapport, Ändra ordning, Problem, Begäran) finns i [Anpassa standardproblemtyper](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. (Villkorligt) Om du vill skapa en ny status klickar du på **Lägg till en ny status**.

   eller

   Om du vill redigera en befintlig status för du musen över den status du vill redigera och klickar sedan på alternativet **Redigera** som visas längst till höger.

   ![Gruppstatus](assets/group-statuses-edit.jpg)

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
      <td> <p>Ange ett namn för statusen. Detta är ett obligatoriskt fält.</p> <p>När du skapar ett statusnamn bör du tänka på att andra i systemet kan skapa en status med samma namn. Vi rekommenderar att du använder ett unikt namn för att undvika förvirring när du väljer status i Workfront.</p><p>Om det finns dubblettstatusar bör gruppadministratören uppdatera namnen för att skilja dem åt. Den enda unika indikatorn i systemet är statusnyckeln.</p> </td> 
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
      <td> <p>(Endast projekt- och aktivitetsstatus)</p> <p>Aktivera det här alternativet om du vill att statusen ska vara dold för användarna. När den är inaktiverad (standardinställningen) kan statusen användas för alla undergrupper under gruppen.</p> <p>Tips! Du kan dölja statusen Problem genom att inaktivera alla fyra problemtyperna (Felrapport, Ändra ordning, Problem, Begäran).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lås för alla grupper</td> 
      <td> 
       <p>Om du låter det här alternativet vara aktiverat kan användarna i din grupp och dess undergrupper se och använda status, och gruppadministratörer kan inte anpassa det för lägre undergrupper.</p> 
       <p>När det här alternativet är inaktiverat kan gruppadministratörer anpassa statusen för undergrupper.</p> 
       <p><b>Obs!</b> Du kan använda både låsta och olåsta statusvärden i en gruppgodkännandeprocess. Om du skapar en process för gruppgodkännande med olåst gruppstatus kan användarna bifoga godkännandeprocessen till alla projekt, aktiviteter eller utgåvor som är kopplade till gruppen.</p> 
       <p>Mer information om att låsa status finns i <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Låsta och olåsta gruppstatusar</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Klicka på **Spara**.

   Statusen är nu tillgänglig för alla projekt som är kopplade till din grupp eller undergrupp. Om du har låst den kan den användas av alla undergrupper.

   Du kan konfigurera statusen till standardstatus för gruppen. Mer information finns i [Använd en anpassad status som standardstatus för en grupp](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Skapa en anpassad status för flera grupper

Om du är Workfront-administratör kan du skapa en anpassad status för flera grupper genom att skapa en systemomfattande status och sedan dölja den statusen för de grupper som inte behöver den.

Om du är gruppadministratör (eller Workfront-administratör) kan du skapa en anpassad status för flera undergrupper i en grupphierarki som du hanterar genom att skapa en status för en grupp på en högre nivå och sedan dölja den statusen för undergrupper som inte behöver den.

1. Om du är Workfront-administratör skapar du en olåst status i hela systemet enligt beskrivningen i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. I rutan i det övre högra hörnet tar du bort **Systemstatus**, börjar skriva namnet på en grupp där du vill dölja statusen och klickar sedan på namnet när det visas.
1. Håll markören över den status som du vill dölja för gruppen och klicka sedan på **Redigera** när den visas.

   ![Redigera status](assets/hover-click-edit.jpg)

1. Aktivera alternativet **Dölj status** som visas.

   ![Dölj status](assets/hide-group-status.png)

1. Klicka på **Spara**.

   Statusen är nedtonad och inte längre synlig för alla användare i gruppen.

1. Upprepa steg 3 till 5 för att dölja den anpassade statusen för andra grupper som inte behöver den.

