---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Hantera timtyper
description: Du kan associera timtyper med timposterna. Timtyper är etiketter som du använder för att definiera timposterna. Timtyper kan vara för allmän tid eller för projektspecifik tid.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: e8c89b68a022ae1c0cf5da20257cd8bc36e94d4c
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 0%

---

# Hantera timtyper

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>-->

Timtyper är etiketter som du använder för att definiera timposterna. Du kan associera timtyper med timposterna.

Det finns två typer av timmar:

* **Projektspecifika timtyper**: Det här är tidsloggade projekt, uppgifter och problem. Projektspecifika timtyper kan associeras med timposter var som helst i [!DNL Adobe Workfront] där du kan logga tid för projekt, aktiviteter och ärenden.

  När du loggar in i [!DNL Workfront] beror de projektspecifika timtyperna som är tillgängliga på konfigurationsalternativen som ställs in på system-, projekt- och användarnivå.

  Följande standardtyper av projektspecifika timmar är alltid tillgängliga:

   * Projekttid
   * Aktivitetstid
   * Utgivningstid

  Administratören [!DNL Workfront] avgör vilka projektspecifika timtyper som är tillgängliga, vilket beskrivs i [Definiera timtyper och tillgänglighet](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Om du aktiverar några projektspecifika timtyper i ditt [!DNL Workfront]-system måste minst en projektspecifik timtyp aktiveras för varje projekt i systemet. Du kan inte aktivera en projektspecifik timtyp på systemnivå och har inga projektspecifika timtyper tillgängliga på projektnivå.

* **Allmänna timtyper**: Allmänna timmar kan inte associeras med ett projekt, en aktivitet eller ett problem, och de loggas direkt i en tidrapport.

Mer information om hur du loggar timmar och associerar dem med timtyper finns i [Loggtid](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inbyggda timtyper

Workfront levereras med en uppsättning inbyggda timtyper. Det går inte att redigera eller dölja de här timtyperna.

Timtyperna som medföljer [!DNL Workfront] är:

* **[!UICONTROL Sick Time]**: En allmän timtyp som inte kan associeras med timposter i ett projekt, en aktivitet eller en utgåva. Sjukdomstid kan inte räknas som intäkt.
* **[!UICONTROL Vacation Time]**: En allmän timtyp som inte kan associeras med timposter i ett projekt, en aktivitet eller en utgåva. Ledig tid kan inte räknas som intäkt.
* **[!UICONTROL General Overhead]**: En allmän timtyp som inte kan associeras med timposter i ett projekt, en aktivitet eller en utgåva. Det kan räknas som intäkter i projektplaneringsprocessen.
* **[!UICONTROL Project Time]**: En allmän timtyp som bara kan associeras med timposter i ett projekt.
* **[!UICONTROL Task Time]**: En allmän timtyp som bara kan associeras med timposter för en aktivitet.
* **[!UICONTROL Issue Time]**: En allmän timtyp som bara kan associeras med timposter i en utgåva.

## Skapa timtyper

Som [!DNL Workfront]-administratör kan du skapa timtyper för din organisation på system- och projektnivå.

När du har definierat timtyper på systemnivå kan användarna definiera vilka timtyper som är tillgängliga för specifika projekt eller för specifika användare.

Mer information finns i [Definiera timtyper och tillgänglighet](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Skapa timtyper:

{{step-1-to-setup}}

1. Klicka på **Tidrapport och timmar** i den vänstra panelen och klicka sedan på **Timtyper**.

1. Klicka på **Ny timtyp** i avsnittet **Timtyper**.
1. Ange följande information i dialogrutan **Nya timtyper**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Ange ett timtypnamn som är lätt att känna igen i systemet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Lägg till en beskrivning av timtypen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Välj om timtypen är en allmän eller projektspecifik timtyp i listrutan <strong>Omfång</strong>.</p> <p>Allmänna timtyper visas bara i tidrapporter och kan inte associeras med projekt, uppgifter eller problem.</p> <p><b>VIKTIGT</b></p><p> Om du har en anpassad timtyp som är [!UICONTROL Project Specific] och du ändrar den till [!UICONTROL General], ställs alla befintliga aktivitets-, ärenden- och projekttimmar in på respektive systemstandardtyper.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count as Revenue]</td> 
      <td><p>Välj det här alternativet om du vill att timtransaktionen som är kopplad till den här timtypen ska påverka dina intäktsberäkningar.</p>
      <p>Sjukdomstid och semestertid kan inte räknas som intäkt.</p>
      <p><b>ANMÄRKNING</b></p>
      <p>När allmänna timtyper räknas som intäkt, är kostnadssatsen som är associerad med profilen för användaren som loggar tiden associerad med timkostnaden.  
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara**.

   Timtypen läggs till i ditt Workfront-system och aktiveras som standard.

## Redigera timtyper

Som [!DNL Workfront]-administratör kan du redigera timtyper för din organisation på system- och projektnivå.

>[!NOTE]
>
>* Du kan inte redigera inbyggda timtyper.
>* Du kan inte redigera timtyper i bulk.

{{step-1-to-setup}}

1. Klicka på **Tidrapport och timmar** i den vänstra panelen och klicka sedan på **Timtyper**.

1. Klicka på ett timtypsnamn eller välj timtyp och klicka sedan på ikonen **Redigera** ![Redigera ](assets/edit-icon.png) längst upp i listan.
1. Ange följande information i dialogrutan **Redigera timtyper**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Ange ett timtypnamn som är lätt att känna igen i systemet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Lägg till en beskrivning av timtypen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Välj om timtypen är en allmän eller projektspecifik timtyp i listrutan <strong>Omfång</strong>.</p> <p>Allmänna timtyper visas bara i tidrapporter och kan inte associeras med projekt, uppgifter eller problem.</p> <p><b>VIKTIGT</b></p> <p>Om du har en anpassad timtyp som är [!UICONTROL Project Specific] och du ändrar den till [!UICONTROL General], ställs alla befintliga aktivitets-, ärenden- och projekttimmar in på respektive systemstandardtyper.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Count as Revenue]</td> 
      <td><p>Välj det här alternativet om du vill att timtransaktionen som är kopplad till den här timtypen ska påverka dina intäktsberäkningar.</p>
      <p>Sjukdomstid och semestertid kan inte räknas som intäkt.</p>
      <p><b>ANMÄRKNING</b></p>
      <p>När allmänna timtyper räknas som intäkt, är kostnadssatsen som är associerad med profilen för användaren som loggar tiden associerad med timkostnaden.  
      </td> 
     </tr> 
    </tbody> 
   </table>


1. Klicka på **Spara**.

   Ändringarna sparas och timtypen redigeras.

## Inaktivera timtyper

Du kan inaktivera timtyper om du inte längre vill att användarna ska associera sina timmar med dem. Om du inaktiverar timtyper döljs de var som helst i [!DNL Workfront] där timtyper visas.

>[!NOTE]
>
>* Du kan inte inaktivera inbyggda timtyper.
>* Du kan inaktivera timtyper gruppvis.
>* När du inaktiverar en projektspecifik timtyp används automatiskt en inbyggd projektspecifik timtyp för all tid som loggas för den typen. Den tid som loggas för ett projekt är till exempel som standard timtypen Projekttid. Den tid som loggas för en uppgift är som standard timtypen Aktivitetstid.
>* När du inaktiverar en allmän timtyp finns den loggade tiden kvar på tidrapporten, men användare kan inte längre logga tid för den timtypen i framtiden.



Så här inaktiverar du en timtyp:

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Timesheet & Hours]** i den vänstra panelen och sedan på **[!UICONTROL Hour Types]**.

1. Välj den timtyp som du vill inaktivera. Du kan välja flera timtyper.

1. Klicka på **Mer** och sedan på **Inaktivera**.

   ![Aktivera och inaktivera timtyplänkar](assets/activate-and-deactivate-hour-type-links.png)

   Timtypen är inaktiverad och användaren kan inte längre hitta den vid loggning av timmar.

1. (Valfritt) Om du vill återaktivera en timtyp markerar du den i listan **Timtyper** och klickar sedan på **Mer** > **Aktivera**.

