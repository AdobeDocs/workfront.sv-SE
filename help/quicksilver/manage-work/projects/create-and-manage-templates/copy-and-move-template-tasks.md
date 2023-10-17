---
product-area: templates
navigation-topic: templates-navigation-topic
title: Kopiera och flytta malluppgifter
description: Du kan kopiera eller flytta en malluppgift till samma mall eller till en annan mall.
author: Alina
feature: Work Management
exl-id: a2e09e63-5c88-460c-9996-3a39fbb82150
source-git-commit: 5db9a4869e1321bd268e80f786d157fbb41c0656
workflow-type: tm+mt
source-wordcount: '2127'
ht-degree: 0%

---

# Kopiera och flytta malluppgifter

Du kan kopiera en malluppgift från en mall till en annan, eller flytta den till en annan mall eller till en annan plats i samma mall.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till mallar</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter till en mall och till malluppgiften </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när du kopierar eller flyttar malluppgifter

Tänk på följande när du kopierar malluppgifter:

* Följande information överförs inte till den kopierade uppgiften:

   * Milstolpar

* Du kan välja att kopiera vissa objekt som är associerade med malluppgiften till den kopierade uppgiften under kopieringsprocessen. Som standard överförs dock inte följande objekt till den kopierade uppgiften:

   * Användarkommentarer

* Anpassade formulär kopieras med malluppgiften när du kopierar en malluppgift. Informationen i de anpassade fälten överförs endast till den nya malluppgiften när du väljer att kopiera anpassade data.

* Följande objekt överförs som standard till den kopierade malluppgiften:

   * Underaktiviteter

Tänk på följande när du flyttar malluppgifter:

* Följande information överförs som standard till den flyttade uppgiften:

   * Anpassade formulär och anpassad fältinformation.
   * Underaktiviteter.
   * Användarkommentarer.

* Följande information överförs inte till den flyttade aktiviteten:

   * Milstolpar.

## Kopiera malluppgifter

Du kan kopiera en enstaka malluppgift eller flera malluppgifter samtidigt.

1. Gå till mallen som innehåller malluppgiften eller malluppgifterna som du vill kopiera.
1. Klicka **Malluppgifter** till vänster.
1. Gör något av följande:
   * Klicka på namnet på en malluppgift för att öppna den.
   * Markera en eller flera malluppgifter i listan.
1. (Villkorligt) Klicka på **Mer** meny ![](assets/more-icon.png) högst upp i uppgiftslistan för mallen eller till höger om uppgiftsnamnet för mallen om du öppnade uppgiften och sedan klickar du på **Kopiera till** eller **Kopiera**, beroende på var du öppnar alternativet Kopiera från.
Rutan Kopiera malluppgift öppnas.
   ![](assets/copy-template-task-box-unshimmed.png)
1. (Valfritt) Byt namn på mallåtgärden i **Malluppgiftsnamn** fält.

   >[!TIP]
   >
   >Det här fältet är nedtonat och går inte att redigera när du väljer att kopiera flera malluppgifter i en lista. Du kan hovra över fältet Malluppgiftsnamn och en lista över alla valda mallåtgärder visas.

1. Börja skriva namnet på **Målmall** där du vill kopiera malluppgiften i **Välj målmall** markerar du det när det visas i listan.

   Det aktuella mallnamnet visas som standard. Om du vill kopiera malluppgiften inom samma mall lämnar du det här fältet oförändrat.

   >[!TIP]
   >
   >Du kan också börja skriva referensnumret eller ange ID:t för mallen. Det kan hjälpa dig att skilja mellan mallar med identiska namn.

1. (Villkorligt) Klicka **begära åtkomst** om du vill begära åtkomst till målmallen, om du inte har åtkomst till den valda mallen.
1. (Villkorligt) Fortsätt att kopiera malluppgiften till den valda målmallen utan att begära åtkomst om du har tillgång till att lägga till malluppgifter i någon av malluppgifterna i målmallen.

1. Klicka **Alternativ** i den vänstra panelen avmarkerar du de malluppgiftsattribut som du inte vill kopiera med malluppgiften. Alla alternativ är markerade som standard.

   >[!TIP]
   >
   >Avmarkera **Markera alla** avmarkerar alla alternativ.

   Avmarkera bland följande alternativ om du inte vill överföra dem till den kopierade malluppgiften. I följande tabell beskrivs vad som händer när alternativen avmarkeras:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Markera alla</td> 
      <td>Avmarkera det här alternativet om du vill ta bort all information från malluppgiften när den kopieras till den nya platsen. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Begränsning</td> 
      <td> <p>Malluppgiftsbegränsningen ställs in på Så snart som möjligt eller Sent som möjligt baserat på mallplaneringsläget.</p> <p> När du väljer det här alternativet överförs den aktuella begränsningen för malluppgiften till den kopierade malluppgiften. </p> 
      <p><b>ANMÄRKNING</b>

   När du kopierar en malluppgift med datumspecifika begränsningar till en annan mall och begränsningsdatumen för mallaktiviteten ligger utanför datumen för den nya mallen, ändras malluppgiftsbegränsningen till Så snart som möjligt eller Så sent som möjligt, eller mallarnas planerade start- eller slutförandedatum justeras.

   Nedan följer exempel på datumspecifika begränsningar:
   <ul>
      <li> Måste börja på</li>
      <li> Måste avslutas</li>
      <li> Starta tidigast</li>
      <li> Starta senast</li>
      </ul>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppdrag</td> 
      <td> <p>Alla tilldelningar tas bort från malluppgiften. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Godkännandeprocess</td> 
      <td>Alla godkännandeprocesser tas bort från malluppgiften.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Alla föregående</td> 
      <td> <p>Det innebär att beroendena inte överförs till de kopierade malluppgifterna. </p> <p>När du väljer det här alternativet bevaras föregående aktiviteter i gruppen med kopierade malluppgifter, andra tas bort.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Anpassade data</td> 
      <td> <p>Värdena för de anpassade fälten rensas och de anpassade formulären överförs till den kopierade malluppgiften. </p> <p>När du väljer det här alternativet överförs både formulären och värdena för de anpassade fälten till den kopierade malluppgiften. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ekonomisk information</td> 
      <td>Den ekonomiska informationen för den kopierade mallaktiviteten tas bort och Workfront uppdaterar malluppgiftens kostnadstyp till Ingen kostnad och malluppgiftens intäktstyp som inte fakturerbar.
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokument</td> 
      <td> <p>De dokument som är kopplade till malluppgiften överförs inte till den kopierade malluppgiften. Detta inkluderar versioner, korrektur och länkade dokument.</p> <p><b>ANMÄRKNING</b></p>

   <p>Detta inkluderar inte dokumentgodkännanden. Dokumentgodkännanden kan aldrig kopieras när en malluppgift kopieras.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Påminnelsemeddelanden</td> 
      <td>Påminnelser om malluppgifter överförs inte till den kopierade malluppgiften. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Utgifter</td> 
      <td>Utgifterna som är inloggade i mallaktiviteten överförs inte till den kopierade malluppgiften. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Valfritt) Klicka på **Markera överordnad** i den vänstra panelen väljer du sedan den mallåtgärd i målmallen som du vill ska vara överordnad den kopierade malluppgiften.

   >[!TIP]
   >
   >När du väljer att kopiera flera malluppgifter i en lista blir alla markerade malluppgifter underordnade den markerade överordnade och läggs till efter de befintliga underordnade uppgifterna.

   Välj en överordnad genom att göra något av följande:

   * Välj en av de överordnade i mallplanen i listan över malluppgifter.
   * Klicka på sökikonen ![Ikonen Sök](assets/search-icon.png) och söka efter en överordnad malluppgift efter namn.

   Malluppgiften ska visas i listan.

1. Markera alternativknappen för den överordnade när du har hittat den.

   Om du inte väljer en överordnad malluppgift kopieras malluppgifterna som huvudmalluppgifter i stället för underuppgifter, och de placeras i slutet av malluppgiftslistan på målmallen.

1. Klicka **Kopiera malluppgift**.

   De kopierade malluppgifterna finns nu i den angivna mallen och är antingen underuppgifter till den valda överordnade malluppgiften eller de senaste malluppgifterna i mallen.


## Flytta malluppgifter

Du kan flytta en malluppgift till en annan malluppgift i samma mall eller till en annan mall. Du kan flytta en malluppgift eller flera malluppgifter åt gången.

1. Gå till mallen som innehåller malluppgiften eller malluppgifterna som du vill flytta.
1. Klicka **Malluppgifter** till vänster.
1. Gör något av följande:
   * Klicka på namnet på en malluppgift för att öppna den.
   * Markera en eller flera malluppgifter i listan.
1. (Villkorligt) Klicka på **Mer** meny ![](assets/more-icon.png) högst upp i uppgiftslistan för mallen eller till höger om uppgiftsnamnet för mallen om du öppnade uppgiften och sedan klickar du på **Flytta till** eller **Flytta**, beroende på var du öppnar alternativet Flytta från.
Rutan Flytta malluppgift öppnas.
   ![](assets/move-template-task-box-unshimmed.png)

1. (Valfritt) Byt namn på mallåtgärden i **Malluppgiftsnamn** fält.

   >[!TIP]
   >
   >Det här fältet är nedtonat och går inte att redigera när du väljer att flytta flera malluppgifter i en lista. Du kan hålla muspekaren över malluppgiftsfältet och en lista över alla valda malluppgifter visas.

1. Börja skriva namnet på **Målmall** där du vill flytta malluppgiften i **Välj målmall** markerar du det när det visas i listan.

   >[!TIP]
   >
   >Du kan också börja skriva referensnumret eller ange ID:t för mallen. Det kan hjälpa dig att skilja mellan mallar med identiska namn.

1. (Villkorligt) Klicka **begära åtkomst** om du vill begära åtkomst till mallen, om du inte har åtkomst till målmallen.
1. (Villkorligt) Fortsätt att flytta malluppgiften till den valda målmallen utan att begära åtkomst om du har tillgång till att lägga till malluppgifter till någon av malluppgifterna i målmallen.

1. Klicka **Alternativ** i den vänstra panelen avmarkerar du de malluppgiftsattribut som du inte vill kopiera med malluppgiften. Alla alternativ är markerade som standard.

   >[!TIP]
   >
   >* Alternativavsnittet är bara tillgängligt när du har valt en målmall.
   >* Avmarkera **Markera alla** avmarkerar alla alternativ.

   Avmarkera följande alternativ om du inte vill överföra informationen till den flyttade malluppgiften. I följande tabell beskrivs vad som händer när alternativen avmarkeras:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Markera alla</td> 
      <td>Avmarkera det här alternativet om du vill ta bort all information från mallaktiviteten när du flyttar den till dess nya plats. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Begränsning</td> 
      <td> <p>Malluppgiftsbegränsningen ställs in på Så snart som möjligt eller Sent som möjligt baserat på mallplaneringsläget.</p> <p> När du väljer det här alternativet överförs den aktuella begränsningen för malluppgiften till den flyttade malluppgiften. </p>

   <p><b>ANMÄRKNING</b>

   När du flyttar en malluppgift med datumspecifika begränsningar till en annan mall och begränsningsdatumen för mallaktiviteten ligger utanför datumen för den nya mallen, ändras malluppgiftsbegränsningen till Så snart som möjligt eller Så sent som möjligt, eller mallarnas planerade start- eller slutförandedatum justeras.

   Nedan följer exempel på datumspecifika begränsningar:
   <ul>
      <li> Starta den</li>
      <li> Måste avslutas</li>
      <li> Starta tidigast</li>
      <li> Starta senast</li>
      </ul>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppdrag</td> 
      <td> <p>Alla tilldelningar tas bort från malluppgiften. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Godkännandeprocess</td> 
      <td>Alla godkännandeprocesser tas bort från malluppgiften.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Alla föregående</td> 
      <td> <p>Det innebär att beroendena inte överförs med de flyttade malluppgifterna. </p> <p>När du väljer det här alternativet bevaras föregående aktiviteter i gruppen med flyttade malluppgifter, andra tas bort.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Anpassade data</td> 
      <td> <p>Värdena för de anpassade fälten rensas och de anpassade formulären överförs med den flyttade mallaktiviteten. </p> <p>När du väljer det här alternativet överförs både formulären och värdena för de anpassade fälten med den flyttade malluppgiften. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ekonomisk information</td> 
      <td>Den ekonomiska informationen för den flyttade mallaktiviteten tas bort och Workfront uppdaterar malluppgiftens kostnadstyp till Ingen kostnad och malluppgiftens intäktstyp som Inte fakturerbar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokument</td> 
      <td> <p>De dokument som är kopplade till malluppgiften överförs inte med den flyttade malluppgiften. Detta inkluderar versioner, korrektur och länkade dokument.</p>

   <p><b>ANMÄRKNING</b></p>

   <ul><li>
      <p>Detta inkluderar inte dokumentgodkännanden. Dokumentgodkännanden kan aldrig flyttas när en malluppgift flyttas.</p> </li>
      <li>Om du inte vill att dokumenten ska flyttas tillsammans med malluppgiften, tas dokumenten bort och placeras i papperskorgen under 30 dagar. En administratör kan återställa dem och de återställs vid den flyttade mallaktiviteten.

   Om mallåtgärden tas bort när den har flyttats placeras de återställda dokumenten i området Dokument på administratörens användarsida, som återställer dem. </li> </ul>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Påminnelsemeddelanden</td> 
      <td>Påminnelser om malluppgifter överförs inte till den flyttade mallaktiviteten. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Utgifter</td> 
      <td>Utgifterna som är inloggade i mallaktiviteten överförs inte med den flyttade mallaktiviteten. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Valfritt) Klicka på **Markera överordnad** i den vänstra panelen väljer du sedan den mallåtgärd i målmallen som du vill ska vara överordnad den flyttade malluppgiften.

   >[!TIP]
   >
   >När du väljer att flytta flera malluppgifter i en lista blir alla markerade malluppgifter underordnade den markerade överordnade och läggs till efter de befintliga underordnade uppgifterna.

   Välj en överordnad genom att göra något av följande:

   * Välj en av de överordnade i mallplanen i listan över malluppgifter.
   * Klicka på sökikonen ![Ikonen Sök](assets/search-icon.png) och söka efter en överordnad malluppgift efter namn.

   Malluppgiften ska visas i listan.

1. Markera alternativknappen för den överordnade när du har hittat den.

   Om du inte väljer en överordnad malluppgift flyttas malluppgifterna som huvudmalluppgifter i stället för underuppgifter, och de placeras i slutet av malluppgiftslistan på målmallen.

1. Klicka **Flytta malluppgift**.

   De flyttade malluppgifterna finns nu i den angivna mallen och är antingen underuppgifter till den valda överordnade malluppgiften eller de senaste malluppgifterna i mallen.
