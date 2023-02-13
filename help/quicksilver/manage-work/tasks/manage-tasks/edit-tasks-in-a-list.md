---
product-area: projects
navigation-topic: manage-tasks
title: Redigera uppgifter i en lista
description: Du kan redigera uppgiftsinformation i en lista med uppgifter genom att redigera fälten som visas i listan. Mer information om andra sätt att redigera uppgifter finns i Redigera uppgifter.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '2828'
ht-degree: 0%

---

# Redigera uppgifter i en lista {#edit-tasks-in-a-list}

Du kan redigera uppgiftsinformation i en lista med uppgifter genom att redigera fälten som visas i listan. Mer information om andra sätt att redigera uppgifter finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute eller högre behörigheter för aktiviteten och projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Att tänka på när du redigerar uppgifter i en lista {#considerations-about-editing-tasks-in-a-list}

Att redigera uppgifter i en lista är ett snabbt sätt att göra ändringar i flera uppgifter samtidigt, med en tydlig bild av hur ändringarna kan påverka projekttidslinjen.

Tänk på följande när du redigerar uppgifter i en lista:

* Till skillnad från när du behöver hantera behörigheter för en uppgift när du redigerar den i redigeringsrutan, kan du bara redigera en uppgift i en lista med Contribute-behörigheter för uppgiften. På så sätt kan du redigera följande begränsade information för uppgiften:

   * Beskrivning
   * Status
   * Procent färdigt
   * Anpassad formulärinformation

      >[!NOTE]
      >
      >Du kan bara redigera ett anpassat aktivitetsfält i en lista om du har behörighet att uppdatera fältet.

   * Loggtimmar
   * Ändra uppdrag
   * Visa ekonomisk information
   * Lägg till utgifter, uppgifter eller ärenden

* Du kan redigera en uppgift i följande listor:

   * Avsnittet Uppgifter i projektet
   * Delaktivitetsavsnittet i projektet
   * En uppgiftsrapport

      >[!NOTE]
      >
      >Som standard sparar Workfront automatiskt ändringar i uppgifter i underaktivitetsavsnittet eller i en uppgiftsrapport.

* Du kan styra när Workfront ska spara de ändringar du gör i uppgifterna i en lista. Ändringarna kan sparas automatiskt eller så kan du spara dem manuellt.

   Information om hur du konfigurerar när Workfront sparar ändringar som du gör i uppgifter i en lista finns i [Välj ett sparningsalternativ när du redigerar uppgifter i en lista](#select-a-save-option-when-editing-tasks-in-a-list) i den här artikeln.

## Välj ett sparningsalternativ när du redigerar uppgifter i en lista {#select-a-save-option-when-editing-tasks-in-a-list}

Du kan bestämma var ändringarna som du gör i en lista ska sparas automatiskt, allt eftersom de inträffar, eller om du vill spara ändringarna manuellt.

>[!IMPORTANT]
>
>Beroende på om du sparar uppgifterna automatiskt eller manuellt kan du skriva över någon annans information medan du redigerar uppgifter i en lista. Mer information om hur Workfront sparar ändringar i uppgifter som du gör samtidigt med andra användare finns i [Översikt över att spara samtidiga ändringar i en uppgiftslista](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

När du sparar ändringarna i en lista för ett projekt som har antingen Automatiskt eller Automatiskt och Vid ändring valt som uppdateringstyp, uppdaterar Workfront projekttidslinjen tillsammans med alla projektrelaterade och projektövergripande beroenden. Det kan ta lång tid att beräkna tidslinjen om projektet är stort eller om det finns många beroenden. Vissa metoder för att redigera en uppgiftslista kan vara snabbare än andra, beroende på vilken metod du väljer för att spara ändringarna.

Du kan styra när Workfront ska spara de ändringar du gör i uppgifterna i en lista. Följande scenarier finns: 

* Du kan låta Workfront spara ändringarna automatiskt efter varje uppdatering.

   Mer information finns i avsnittet [Redigera uppgifter i en lista och spara ändringar automatiskt](#edit-tasks-in-a-list-and-automatically-save-changes) i den här artikeln.

* Du kan ha kontroll över när du ska göra flera ändringar i taget manuellt med knappen Spara.

   Mer information finns i avsnittet [Redigera uppgifter i en lista och spara ändringar manuellt](#edit-tasks-in-a-list-and-manually-save-changes) i den här artikeln.

### Redigera uppgifter i en lista och spara ändringar automatiskt {#edit-tasks-in-a-list-and-automatically-save-changes}

>[!TIP]
>
>Det kan ta längre tid att spara ändringarna och alla projektberoenden om projektet innehåller fler än 2 000 uppgifter eller om det har många beroenden.

Tänk på följande när du sparar uppgiftslistan automatiskt:

* Du kan använda en anpassad vy för uppgiftslistan och redigera uppgiftsrelaterade fält som du har tillgång till för uppdatering.
* Du kan inte ångra automatiskt sparade ändringar. Det här är standardinställningen.
* Workfront beräknar om tidslinjen för projektet och alla beroenden mellan projekt och projekt automatiskt efter varje ändring, när projektets uppdateringstyp är Automatisk eller Automatisk och Vid ändring. Mer information om projektets uppdateringstyp finns i [Välj typ av projektuppdatering](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Så här redigerar du uppgifter i en lista och sparar ändringar automatiskt:

1. Gå till projektet och klicka sedan på **Uppgifter** -avsnitt.
1. Klicka på **Menyn Planeringsläge** ![](assets/qs-list-mode-or-save-mode-icon-small.png) högst upp i listan och se till att **Spara automatiskt** är markerat.

   ![](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Redigera fält som du har behörighet att uppdatera manuellt.

   ![](assets/inline-editing-a-task-350x26.png)

1. (Valfritt) Tryck på **Escape** om du vill avbryta ändringarna.
1. Tryck på Retur för att spara ändringarna i aktiviteterna och på projekttidslinjen.
1. (Valfritt) Högerklicka på en uppgift som du vill ändra.

   eller

   Klicka på **Mer** meny ![](assets/more-icon-task-list.png) till höger om aktivitetsnamnet.

1. (Valfritt) Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Öppna på en ny flik</strong></td> 
      <td>Öppnar uppgiften på en ny flik i webbläsaren. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Redigera</strong></td> 
      <td><p>Öppnar <strong>Redigera uppgift</strong> där du kan redigera uppgiften.</p><p>Mer information om hur du redigerar en uppgift finns i <a href="#edit-tasks-in-a-list" class="MCXref xref">Redigera uppgifter i en lista</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ta bort</td> 
      <td><p>Tar bort aktiviteten.</p><p>Mer information om hur du tar bort uppgifter finns i <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Ta bort uppgifter</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Indrag</td> 
      <td><p>Drar in uppgiften en nivå. </p><p>Det här alternativet visas endast för fristående uppgifter.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Minska indrag</td> 
      <td><p>Minskar indraget för aktiviteten med en nivå. </p><p>Det här alternativet visas endast för underordnade uppgifter. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Infoga aktivitet ovan</td> 
      <td>Infogar en uppgift ovanför den markerade uppgiften.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Infoga aktivitet nedan</td> 
      <td>Infogar en uppgift under den valda uppgiften</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplicera</td> 
      <td><p>Skapar en dubblettversion av aktiviteten i samma projekt. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopiera till</td> 
      <td><p>Kopierar uppgiften till ett annat projekt.</p><p>Mer information om att kopiera och duplicera uppgifter finns i <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Kopiera och duplicera uppgifter</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Flytta till</td> 
      <td><p>Flyttar aktiviteten till ett annat projekt.</p><p>Mer information om hur du flyttar uppgifter finns i <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Flytta uppgifter</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

   Ändringarna sparas automatiskt och du kan inte ångra dem.

### Redigera uppgifter i en lista och spara ändringar manuellt {#edit-tasks-in-a-list-and-manually-save-changes}

Du kan spara ändringar du gör i en lista manuellt. När du sparar ändringar på det här sättet kan du ändra tillbaka dem innan du sparar dem.

>[!TIP]
>
>* Du kan inte ångra ändringar som du gör i uppgifter i en lista när du redigerar dem i underaktivitetsavsnittet eller i en uppgiftsrapport.
>* Det finns inga begränsningar för hur många ändringar du kan ångra. Du kan invertera alla en i taget tills du når det ursprungliga tillståndet för åtgärderna.
>


Tänk på följande när du sparar ändringar i en uppgiftslista manuellt:

* Om du vill spara ändringar i uppgiftslistan manuellt måste du ha behörighet att hantera både uppgifterna och projektet.
* Du kan inte redigera projektet. Alternativet att redigera projektet är inaktiverat.
* Du kan inte uppdatera information i projektets huvud. Du kan bara göra följande när du sparar ändringarna i uppgiftslistan manuellt:

   * Prenumerera på projektet.
   * Lägg till projektet i din lista över favoriter.
   * Öppna en uppgift genom att klicka på dess namn i listan.

* redigera flera uppgifter samtidigt. Ikonen Redigera är inaktiverad när du markerar flera uppgifter.
* Workfront utlöser meddelanden om de ändringar du gör i uppgifterna först när du har sparat ändringarna.

Det finns två sätt att spara ändringar av uppgifter manuellt i en lista. Dessa två sätt beskrivs nedan.

* [Spara ändringar i en uppgiftslista manuellt när du väljer alternativet Spara standard manuellt](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Spara ändringar i en uppgiftslista manuellt när du väljer alternativet Spara tidslinjeplanering manuellt](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Spara ändringar i en uppgiftslista manuellt när du väljer alternativet Spara standard manuellt {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Om ditt projekt har fler än 2 000 uppgifter, eller om det har många beroenden, kan det ta en stund att visuellt identifiera de ändringar du gör i dina uppgifter och hur dessa ändringar påverkar alla projektberoenden. I det här fallet kan det ta längre tid att spara ändringarna om projektet har fler än 2 000 uppgifter eller om det har många beroenden.

Tänk på följande när du uppdaterar uppgifter i en lista efter att du har valt alternativet Spara standard manuellt:

* Du kan använda en anpassad vy för uppgiftslistan och redigera uppgiftsrelaterade fält som du har behörighet att hantera i den vyn.
* Workfront beräknar tidslinjen för projektet och alla projektrelaterade och projektövergripande beroenden när du klickar på Spara, när projektets uppdateringstyp är Automatisk eller Automatisk och vid ändring. Mer information om projektets uppdateringstyp finns i [Välj typ av projektuppdatering](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Så här redigerar du uppgifter i en lista när du väljer alternativet Spara standard manuellt:

1. Gå till ett projekt och klicka sedan på **Uppgifter** avsnitt .
1. Klicka på **Planläge** meny ![](assets/qs-list-mode-or-save-mode-icon-small.png) högst upp i listan och välj **Spara manuellt** och sedan klicka **Standard** > **Använd**.

   ![](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

   En inställning i verktygsfältet visas med alternativ för att ångra, göra om och spara ändringarna.

   ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Klicka i ett fält som du har behörighet att uppdatera manuellt. Fältet kan redigeras och du kan göra ändringarna.

   ![](assets/inline-editing-a-task-350x26.png)

1. Tryck på Retur om du vill spara ändringarna tillfälligt.
1. (Valfritt) Klicka på **Ångra-ikon** ![](assets/undo-icon-on-task-list.png) om du vill återställa en ändring och återställa ett fält till det ursprungliga läget.
1. (Valfritt och villkorligt) Klicka på **Ikonen Gör om** ![](assets/redo-icon-on-task-list.png) för att återställa den ändring som du har ångrat.

1. (Valfritt) Högerklicka på en uppgift som du vill ändra.

   eller

   Klicka på **Mer** meny ![](assets/more-icon-task-list.png).

1. (Valfritt) Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Öppna på en ny flik</strong> </td> 
      <td>Öppnar uppgiften på en ny flik i webbläsaren. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ta bort</td> 
      <td>Mer information om hur du tar bort uppgifter finns i <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Ta bort uppgifter</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Indrag</td> 
      <td> <p>Drar in uppgiften en nivå. </p> <p>Det här alternativet visas endast för fristående uppgifter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Minska indrag</td> 
      <td> <p>Minskar indraget för aktiviteten med en nivå. </p> <p>Det här alternativet visas endast för underordnade uppgifter. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Infoga aktivitet ovan</td> 
      <td>Infogar en uppgift ovanför den markerade uppgiften.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Infoga aktivitet nedan</td> 
      <td>Infogar en uppgift under den valda uppgiften</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplicera</td> 
      <td> <p>Skapar en dubblettversion av aktiviteten i samma projekt. </p> <p>Mer information om att kopiera och duplicera uppgifter finns i <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Kopiera och duplicera uppgifter</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront uppdaterar alla projektrelaterade och projektövergripande beroenden när du ändrar tidslinjen för uppgifter.
1. Klicka **Spara** när du vill behålla ändringarna permanent och spara tidslinjen för projektet.

#### Spara ändringar i en uppgiftslista manuellt när du väljer alternativet Spara tidslinjeplanering manuellt {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Det går snabbare att spara ändringarna och alla projektberoenden. Detta är inte tillgängligt för projekt med fler än 2 000 uppgifter.

>[!IMPORTANT]
>
>Vi rekommenderar att du använder det här alternativet när du redigerar en stor lista över uppgifter som är mer än ett fåtal hundra som har många beroenden. Med det här alternativet kan du visuellt identifiera dina ändringar mycket snabbare än med alternativet Spara manuellt.

Tänk på följande när du använder alternativet Spara tidslinjeplanering manuellt i en uppgiftslista:

* Du kan inte använda alternativet för att spara tidslinjeplanering manuellt i projekt som har fler än 2 000 uppgifter.
* Du kan inte använda en anpassad vy, filter eller gruppering för uppgiftslistan. Listrutorna Visa, Filtrera och Gruppera, samt ikonen för vyn Agile, är inaktiverade. Vyn som används som standard innehåller ett begränsat antal fält.
* Tidslinjen för projektet och alla projektberoenden beräknas automatiskt efter varje ändring när projektets uppdateringstyp är Automatisk eller Automatisk och vid ändring.
* Beroenden mellan projekt beräknas när du klickar på Spara, när projektets uppdateringstyp är Automatisk eller Automatisk och Vid ändring. Mer information om projektets uppdateringstyp finns i [Välj typ av projektuppdatering](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Så här redigerar du uppgifter i en lista när du använder alternativet Spara tidslinjeplanering manuellt:

1. Gå till ett projekt och klicka sedan på **Uppgifter** -avsnitt.
1. Klicka på **Planläge** meny ![](assets/qs-list-mode-or-save-mode-icon-small.png) högst upp i listan och välj **Spara manuellt** och sedan klicka **Planering av tidslinje**> **Använd**.

   Det här alternativet är nedtonat för projekt med fler än 2 000 uppgifter.

   ![](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >När du lämnar den här sidan återaktiveras alternativet Spara automatiskt.

   Observera följande ändringar i listan:

   * De nedrullningsbara menyerna Visa, Gruppera och Filter tas bort och vyn ersätts med följande fält:

      * Aktivitetsnummer
      * Aktivitetsnamn
      * Begränsningstyp
      * Varaktighet
      * Planerat startdatum
      * Planerat slutförandedatum
      * Föregående
      * Uppdrag
      * Status
      * Procent färdigt
   * Ikonen för vyn Agile har tagits bort.
   * En inställning i verktygsfältet visas med alternativ för att ångra, göra om och spara ändringarna.

      ![](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)


1. Redigera fält som du har behörighet att uppdatera manuellt.

   ![](assets/inline-editing-a-task-350x26.png)

1. Tryck på Retur om du vill spara ändringarna tillfälligt.
1. (Valfritt) Klicka på **Ångra-ikon** ![](assets/undo-icon-on-task-list.png) om du vill återställa en ändring och återställa ett fält till det ursprungliga läget.
1. (Valfritt och villkorligt) Klicka på **Ikonen Gör om** ![](assets/redo-icon-on-task-list.png) för att återskapa den ändring du återfört.

1. (Valfritt) Högerklicka på en uppgift som du vill ändra

   eller

   Klicka på **Mer** meny ![](assets/more-icon-task-list.png).

1. Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Öppna på en ny flik</strong> </td> 
      <td>Öppnar uppgiften på en ny flik i webbläsaren. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ta bort</td> 
      <td>Mer information om hur du tar bort uppgifter finns i <a href="../../../manage-work/tasks/manage-tasks/delete-tasks.md" class="MCXref xref">Ta bort uppgifter</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Indrag</td> 
      <td> <p>Drar in uppgiften en nivå. </p> <p>Det här alternativet visas endast för fristående uppgifter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Minska indrag</td> 
      <td> <p>Minskar indraget för aktiviteten med en nivå. </p> <p>Det här alternativet visas endast för underordnade uppgifter. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Infoga aktivitet ovan</td> 
      <td>Infogar en uppgift ovanför den markerade uppgiften.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Infoga aktivitet nedan</td> 
      <td>Infogar en uppgift under den valda uppgiften</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duplicera</td> 
      <td> <p>Skapar en dubblettversion av aktiviteten i samma projekt. </p> <p>Mer information om att kopiera och duplicera uppgifter finns i <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Kopiera och duplicera uppgifter</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront uppdaterar alla projektrelaterade och projektövergripande beroenden när du ändrar tidslinjen för en uppgift.
1. Klicka **Spara** när du vill behålla ändringarna permanent och spara tidslinjen för projektet.

## Redigera en uppgift i en lista med hjälp av Sammanfattning

1. Gå till det projekt som innehåller uppgifter som du vill redigera.
1. Klicka **Uppgifter** i den vänstra panelen.

   Listan med uppgifter i projektet visas.

1. Klicka på Mer-menyn ![](assets/more-icon-task-list.png) efter uppgiftsnamnet klickar du på **Öppna sammanfattning**. Markera den uppgift som du vill redigera och klicka sedan på **Ikonen Öppna sammanfattning** ![](assets/qs-open-summary-icon-in-new-toolbar-small.png) i listans övre högra hörn.

   The **Sammanfattning** öppnas.

   ![](assets/qs-task-right-panel-in-a-task-list-350x328.png)

1. (Valfritt) Klicka på **X-ikon** i det övre högra hörnet av sammanfattningen för att stänga panelen och redigera uppgifterna infogat.

   Följ stegen om hur du redigerar en uppgift i en lista för att infoga redigering av uppgiften.

   Mer information om hur du redigerar en uppgift i en lista finns i [Att tänka på när du redigerar uppgifter i en lista](#considerations-about-editing-tasks-in-a-list) i den här artikeln.

1. (Valfritt) Skriv en uppdatering för uppgiften i **Uppdateringar** område.
1. Klicka på någon av följande ikoner eller områden för att gå till uppgiften och redigera information på aktivitetsnivå:

   | Dokument | Klicka **Klicka här för att lägga till** om du vill lägga till dokument i uppgiften. |
   |---|---|
   | Detaljer | Klicka för att uppdatera information om uppgiften. |
   | Anpassad Forms | Klicka för att lägga till eller ta bort anpassad Forms eller för att uppdatera informationen i formulären. |
   | Timmar | Klicka för att logga timmar. |
   | Godkännanden | Klicka för att lägga till aktivitetsgodkännanden. |

   {style=&quot;table-layout:auto&quot;}

1. Klicka på knappen Bakåt i webbläsaren för att återgå till uppgiftslistan när du har uppdaterat uppgiften.

## Redigera flera uppgifter samtidigt

Du kan redigera flera åtgärder samtidigt. Se till att du har behörighet att hantera uppgifter för att kunna redigera dem.

1. Gå till ett projekt som innehåller uppgifter som du vill redigera gruppvis.
1. Klicka **Uppgifter** i den vänstra panelen.
1. Se till att **Spara automatiskt** är markerat.

   >[!IMPORTANT]
   >
   >Du kan inte redigera flera uppgifter samtidigt när du sparar uppgifter manuellt.

   Mer information om hur du sparar ändringar av uppgifter i en lista finns i avsnittet [Att tänka på när du redigerar uppgifter i en lista](#considerations-about-editing-tasks-in-a-list) i den här artikeln.

1. Markera flera uppgifter i uppgiftslistan.
1. Klicka på **Ikonen Redigera** ![](assets/qs-edit-icon.png).

   The **Redigera uppgifter** öppnas.

1. Ange den information som du vill ändra för alla uppgifter som du har markerat.

   Att redigera information för alla uppgifter är detsamma som att redigera information för en uppgift. Om du vill redigera aktivitetens varaktighet måste de markerade aktiviteterna ha samma aktivitetsbegränsning; i annat fall **Varaktighet** fältet fylls inte i.

   Mer information om hur du redigerar en uppgift finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   >[!NOTE]
   >
   >Informationen som du ändrar för alla markerade uppgifter åsidosätter den befintliga informationen för enskilda uppgifter, förutom för **Uppdrag** fält. Om du lägger till en ny tilldelad i en gruppredigering läggs den tilldelade personen till i alla markerade uppgifter. Om andra tilldelningar har tilldelats de markerade aktiviteterna, förblir de tilldelade utöver den som lagts till via massredigering.

1. Klicka **Anpassad Forms** om du vill redigera anpassade formulär som är kopplade till alla markerade uppgifter. Endast aktiva anpassade formulär visas i listan.

   Om de markerade uppgifterna inte har några vanliga anpassade formulär visas inga formulär i det här avsnittet.

   Du kan bara redigera fält i formulären som är kopplade till alla markerade uppgifter och som du har behörighet att redigera.

1. (Valfritt) I delen Anpassad Forms väljer du **Beräkna om anpassade uttryck** för att säkerställa att alla beräknade anpassade fält som finns i de anpassade formulär som är kopplade till de valda uppgifterna är aktuella.
1. Klicka **Spara ändringar**.

   Alla ändringar du har gjort visas nu för alla markerade uppgifter.

Mer information om massredigering av anpassade formulär finns i avsnittet Redigera flera anpassade Forms när du redigerar objekt gruppvis i [Hantera anpassade formulär som är kopplade till objekt](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).
