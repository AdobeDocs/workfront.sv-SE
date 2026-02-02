---
product-area: projects
navigation-topic: manage-tasks
title: Redigera uppgifter i en lista
description: Du kan redigera uppgiftsinformation i en lista med uppgifter genom att redigera fälten som visas i listan. Du måste definiera planläget i en lista med uppgifter för att ange hur du vill att dina ändringar ska sparas i Workfront. Du kan spara ändringarna manuellt eller automatiskt.
author: Alina
feature: Work Management
exl-id: 2af81907-3657-459e-b780-65983e224ca8
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '3254'
ht-degree: 0%

---

# Redigera uppgifter i en lista {#edit-tasks-in-a-list}

<!-- Audited: 10/2025 -->

<div class="preview">

Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Samma funktioner är också tillgängliga i produktionsmiljön för alla kunder från och med en vecka från förhandsversionen.

Mer information finns i [Översikt över den andra utgåvan av kvartal 2026](/help/quicksilver/product-announcements/product-releases/26-q2-release-activity/26-q2-release-overview.md).
</div>

Du kan redigera uppgiftsinformation i en lista med uppgifter genom att redigera fälten som visas i listan. Mer information om andra sätt att redigera uppgifter finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Standard<p>
   <p>Arbeta eller högre</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter och projekt</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute eller högre behörigheter för aktiviteten och projektet</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard<p>
   <p>Current: Work or higher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions to the task and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Att tänka på när du redigerar uppgifter i en lista {#considerations-about-editing-tasks-in-a-list}

Att redigera uppgifter i en lista är ett snabbt sätt att göra ändringar i flera uppgifter samtidigt med en tydlig bild av hur ändringarna kan påverka projekttidslinjen.

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

* Du kan styra när Workfront ska spara de ändringar du gör i uppgifterna i en lista genom att definiera planeringsläget innan du börjar redigera uppgifterna.

  Du kan välja mellan att Workfront sparar de ändringar du gör på följande sätt:

   * Automatiskt, efter varje ändring
   * Manuellt, först när du har klickat på Spara.

  Mer information om hur du konfigurerar när Workfront sparar ändringar som du gör i uppgifter i en lista finns i avsnittet [Ändra planläge innan du redigerar uppgifter i en lista](#modify-plan-mode-before-editing-tasks-in-a-list) i den här artikeln.

* Andra användare måste uppdatera sina sidor innan de kan visa de uppdateringar du gör för en uppgift.

## Ändra planeringsläge innan du redigerar uppgifter i en lista

Du kan bestämma om de ändringar du gör i en lista ska sparas automatiskt när de inträffar, eller om du vill spara ändringarna manuellt. För att göra detta måste du ändra planeringsläget i en lista med uppgifter innan du redigerar uppgifterna.

>[!IMPORTANT]
>
>Beroende på om du sparar uppgifterna automatiskt eller manuellt kan du skriva över någon annans information medan du redigerar uppgifter i en lista. Mer information finns i [Översikt över att spara samtidiga ändringar i en uppgiftslista](../../../manage-work/tasks/manage-tasks/save-concurrent-changes-in-a-task-list.md).

När du sparar ändringarna i en lista för ett projekt som har antingen Automatiskt eller Automatiskt och Vid ändring valt som uppdateringstyp, uppdaterar Workfront projekttidslinjen tillsammans med alla projektrelaterade och projektövergripande beroenden. Det kan ta lång tid att beräkna tidslinjen om projektet är stort eller om det finns många beroenden. Vissa metoder för att redigera en uppgiftslista kan vara snabbare än andra, beroende på vilken metod du väljer för att spara ändringarna.

Du kan styra när Workfront ska spara de ändringar du gör i uppgifterna i en lista. Följande scenarier finns:

* Du kan låta Workfront spara ändringarna automatiskt efter varje uppdatering.

  Mer information finns i avsnittet [Ange planeringsläge för att automatiskt spara ändringar](#set-the-plan-mode-to-automatically-save-changes) i den här artikeln.

* Du kan ha kontroll över när du ska göra flera ändringar i taget manuellt med knappen Spara.

  Mer information finns i avsnittet [Ange planeringsläge för att manuellt spara ändringar](#set-the-plan-mode-to-manually-save-changes) i den här artikeln.

### Ställ in planeringsläget så att ändringar sparas automatiskt

>[!TIP]
>
>Det kan ta längre tid att spara ändringarna och alla projektberoenden om projektet innehåller fler än 2 000 uppgifter eller om det har många beroenden.

Tänk på följande när du sparar uppgiftslistan automatiskt:

* Du kan använda en anpassad vy för uppgiftslistan och redigera uppgiftsrelaterade fält som du har tillgång till för uppdatering.
* Du kan inte ångra automatiskt sparade ändringar. Det här är standardinställningen.
* När projektets uppdateringstyp är Automatisk eller Automatisk och vid ändring, beräknar Workfront om tidslinjen för projektet och alla beroenden mellan projekt och projekt automatiskt efter varje ändring. Mer information om projektets uppdateringstyp finns i [Välj projekttyp](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Så här redigerar du uppgifter i en lista och sparar ändringar automatiskt:

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.
1. Klicka på avsnittet **Åtgärder** i den vänstra panelen.

1. Klicka på ikonen **Planeringsläge** ![Planeringsläge](assets/plan-mode-icon.png) högst upp i listan och kontrollera att alternativet **Spara automatiskt** är markerat.

   ![Aktivera autosparinställningen](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

1. Redigera fält som du har behörighet att uppdatera manuellt.

1. (Valfritt) Tryck på **Esc** om du vill avbryta ändringarna.
1. Tryck på **Enter** (Windows) eller **Return** (Mac) på tangentbordet om du vill spara ändringarna i aktiviteterna och projekttidslinjen.
1. (Valfritt) Högerklicka på en uppgift som du vill ändra.

   eller

   Klicka på ikonen **Mer** meny ![Mer i uppgiftslistan](assets/more-icon-task-list.png) till höger om aktivitetsnamnet.

1. (Valfritt) Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Öppna på ny flik</td> 
      <td>Öppnar uppgiften på en ny flik i webbläsaren. </td> 
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
      <td role="rowheader">Redigera</td> 
      <td><p>Öppnar rutan Redigera uppgift, där du kan redigera uppgiften.</p><p>Mer information om hur du redigerar en uppgift finns i <a href="#edit-tasks-in-a-list" class="MCXref xref">Redigera uppgifter i en lista</a>.</p></td> 
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
      <td role="rowheader">Duplicera</td> 
      <td><p>Skapar en dubblettversion av aktiviteten i samma projekt. </p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopiera till...</td> 
      <td><p>Kopierar uppgiften till ett annat projekt.</p><p>Mer information om att kopiera och duplicera uppgifter finns i <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Kopiera och duplicera uppgifter</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Flytta till...</td> 
      <td><p>Flyttar aktiviteten till ett annat projekt.</p><p>Mer information om att flytta uppgifter finns i <a href="../../../manage-work/tasks/manage-tasks/move-tasks.md" class="MCXref xref">Flytta uppgifter</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

### Ange planeringsläget för att spara ändringar manuellt {#edit-tasks-in-a-list-and-manually-save-changes}

Du kan spara ändringar du gör i en lista manuellt. När du sparar ändringar på det här sättet kan du ändra tillbaka dem innan du sparar dem.

>[!TIP]
>
>* Du kan inte ångra ändringar som du gör i uppgifter i en lista när du redigerar dem i underaktivitetsavsnittet eller i en uppgiftsrapport.
>* Det finns inga begränsningar för hur många ändringar du kan ångra. Du kan invertera alla uppgifter en i taget tills du uppnår det ursprungliga tillståndet för uppgifterna.
>

Tänk på följande när du sparar ändringar i en uppgiftslista manuellt:

* Om du vill spara ändringar i uppgiftslistan manuellt måste du ha behörighet att hantera både uppgifterna och projektet.
* Du kan inte redigera projektet. Alternativet att redigera projektet är inaktiverat.
* Du kan inte uppdatera information i projektets huvud. Du kan bara göra följande när du sparar ändringarna i uppgiftslistan manuellt:

   * Prenumerera på projektet.
   * Lägg till projektet i din lista över favoriter.
   * Öppna en uppgift genom att klicka på dess namn i listan.

* Redigera flera uppgifter samtidigt. Ikonen Redigera är inaktiverad när du markerar flera uppgifter.
* Workfront utlöser meddelanden om de ändringar du gör i uppgifterna först när du har sparat ändringarna.

Det finns två sätt att spara ändringar av uppgifter manuellt i en lista:

* [Spara ändringar i en uppgiftslista manuellt när du väljer alternativet Spara standard manuellt](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option)
* [Spara ändringar i en uppgiftslista manuellt när du väljer alternativet Spara tidslinjeplanering manuellt](#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option)

#### Spara ändringar i en uppgiftslista manuellt när du väljer alternativet Spara standard manuellt {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-standard-option}

>[!TIP]
>
>Om ditt projekt har fler än 2 000 uppgifter, eller om det har många beroenden, kan det ta en stund att visuellt identifiera de ändringar du gör i dina uppgifter och hur dessa ändringar påverkar alla projektberoenden. I så fall kan det ta längre tid än förväntat att spara ändringarna.

Tänk på följande när du uppdaterar uppgifter i en lista efter att du har valt alternativet Spara standard manuellt:

* Du kan använda en anpassad vy för uppgiftslistan och redigera uppgiftsrelaterade fält som du har behörighet att hantera i den vyn.
* När projektets uppdateringstyp är Automatisk eller Automatisk och vid ändring, beräknar Workfront tidslinjen för projektet och alla beroenden mellan projekt och projekt när du klickar på Spara. Mer information om projektets uppdateringstyp finns i [Välj projekttyp](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Så här redigerar du uppgifter i en lista när du väljer alternativet Spara standard manuellt:

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.

1. Klicka på avsnittet **Åtgärder** i den vänstra panelen.

1. Klicka på ikonen **Planeringsläge** ![Planeringsläge](assets/plan-mode-icon.png) högst upp i listan.

1. I dialogrutan **Planeringsläge** väljer du **Manuell sparning** och klickar sedan på **Standard**.

   ![Aktivera inställningen för manuell sparning](assets/manual-standard-setting-enabled-quicksilver-task-list-350x493.png)

1. Klicka på **Använd**. En inställning i verktygsfältet visas med alternativ för att ångra, göra om och spara ändringarna.

   ![Verktygsfältet Spara manuellt](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Klicka i ett fält som du har behörighet att uppdatera manuellt. Fältet kan redigeras och du kan göra ändringarna.

1. Tryck på **Enter** (Windows) eller **Return** (Mac) på tangentbordet om du vill spara ändringarna tillfälligt.

1. (Valfritt) Klicka på ikonen **Ångra** ![Ångra &#x200B;](assets/undo-icon-on-task-list.png) om du vill ångra en ändring och återställa ett fält till det ursprungliga läget.

1. (Valfritt och villkorligt) Klicka på ikonen **Gör om** ![Gör om &#x200B;](assets/redo-icon-on-task-list.png) för att återställa den ändring du ångrat.

1. (Valfritt) Högerklicka på en uppgift som du vill ändra.

   eller

   Klicka på ikonen **Mer** meny ![Läge i uppgiftslistan](assets/more-icon-task-list.png).

1. (Valfritt) Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Öppna på ny flik</td> 
      <td>Öppnar uppgiften på en ny flik i webbläsaren. </td> 
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
      <td role="rowheader">Duplicera</td> 
      <td> <p>Skapar en dubblettversion av aktiviteten i samma projekt. </p> <p>Mer information om att kopiera och duplicera uppgifter finns i <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Kopiera och duplicera uppgifter</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront uppdaterar alla projektrelaterade och projektövergripande beroenden när du ändrar tidslinjen för uppgifter.
1. Klicka på **Spara** när du vill behålla aktivitetsändringarna permanent och spara tidslinjen för projektet.

#### Spara ändringar i en uppgiftslista manuellt när du väljer alternativet Spara tidslinjeplanering manuellt {#save-changes-in-a-task-list-manually-when-you-select-the-manual-save-timeline-planning-option}

Det går snabbare att spara ändringarna och alla projektberoenden. Detta är inte tillgängligt för projekt med fler än 2 000 uppgifter.

>[!IMPORTANT]
>
>Vi rekommenderar att du använder det här alternativet när du redigerar en stor lista över uppgifter som är mer än ett fåtal hundra som har många beroenden. Med det här alternativet kan du visuellt identifiera dina ändringar mycket snabbare än med alternativet Spara manuellt.

Tänk på följande när du använder alternativet Spara tidslinjeplanering manuellt i en uppgiftslista:

* Du kan inte använda alternativet för att spara tidslinjeplanering manuellt i projekt som har fler än 2 000 uppgifter.
* Du kan inte använda en anpassad vy, filter eller gruppering för uppgiftslistan. Listrutorna Visa, Filtrera och Gruppera, samt ikonen för vyn Agile, är inaktiverade. Vyn som används som standard innehåller ett begränsat antal fält.
* Tidslinjen för projektet och alla projektberoenden beräknas automatiskt efter varje ändring när projektets uppdateringstyp är Automatisk eller Automatisk och vid ändring.
* När projektets uppdateringstyp är Automatisk eller Automatisk och vid ändring beräknas beroendena mellan projekt efter att du klickar på Spara. Mer information om projektets uppdateringstyp finns i [Välj projekttyp](../../../manage-work/projects/manage-projects/select-project-update-type.md).

Så här redigerar du uppgifter i en lista när du använder alternativet Spara tidslinjeplanering manuellt:


{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.

1. Klicka på avsnittet **Åtgärder** i den vänstra panelen.

1. Klicka på ikonen **Planeringsläge** ![Planeringsläge](assets/plan-mode-icon.png) högst upp i listan.

1. I dialogrutan **Planeringsläge** väljer du **Spara manuellt** och klickar sedan på **Planering av tidslinje**.

   ![Använd inställning för tidslinjeplanering](assets/manual-timeline-planning-setting-enabled-quicksilver-task-list-350x490.png)

   >[!TIP]
   >
   >Alternativet **Tidsplanering** är nedtonat för projekt med fler än 2 000 aktiviteter.

1. Klicka på **Använd**.

   Följande ändringar görs i listan:

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

     ![Verktygsfältet Spara manuellt](assets/undo,-redo,-save,-and-cancel-widget-for-task-list-350x65.png)

1. Redigera fält som du har behörighet att uppdatera manuellt.

1. Tryck på **Enter** (Windows) eller **Return** (Mac) på tangentbordet om du vill spara ändringarna tillfälligt.
1. (Valfritt) Klicka på ikonen **Ångra** ![Ångra &#x200B;](assets/undo-icon-on-task-list.png) om du vill ångra en ändring och återställa ett fält till det ursprungliga läget.
1. (Valfritt och villkorligt) Klicka på ikonen **Gör om** ![Gör om &#x200B;](assets/redo-icon-on-task-list.png) för att återskapa den ändring du ångrat.

1. (Valfritt) Högerklicka på en uppgift som du vill ändra.

   eller

   Klicka på ikonen **Mer** ![Mer i listan &#x200B;](assets/more-icon-task-list.png).

1. Välj bland följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Öppna på ny flik</td> 
      <td>Öppnar uppgiften på en ny flik i webbläsaren. </td> 
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
      <td role="rowheader">Duplicera</td> 
      <td> <p>Skapar en dubblettversion av aktiviteten i samma projekt. </p> <p>Mer information om att kopiera och duplicera uppgifter finns i <a href="../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md" class="MCXref xref">Kopiera och duplicera uppgifter</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Workfront uppdaterar alla projektrelaterade och projektövergripande beroenden när du ändrar tidslinjen för en uppgift.
1. Klicka på **Spara** när du vill behålla aktivitetsändringarna permanent och spara tidslinjen för projektet.

## Redigera en uppgift i en lista med hjälp av Sammanfattning

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.

1. Klicka på avsnittet **Åtgärder** i den vänstra panelen. Listan med uppgifter i projektet visas.

1. Markera den uppgift som du vill redigera och klicka sedan på ikonen **Öppna sammanfattning** ![Öppna sammanfattning](assets/task-summary-icon.png) i det övre högra hörnet av listan. Panelen **Åtgärdssammanfattning** öppnas.

1. (Valfritt) Skriv en uppdatering för aktiviteten i området **Uppdateringar**.
1. Klicka på någon av följande ikoner eller områden för att gå till uppgiften och redigera information på aktivitetsnivå:

<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Dokument</td> 
      <td>Lägg till dokument i uppgiften. </td> 
     </tr> 
          <tr> 
      <td role="rowheader">Anpassad Forms</td> 
      <td>Lägg till eller ta bort anpassade formulär eller uppdatera information i formulären.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Timmar</td> 
      <td>Loggtimmar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Godkännanden</td> 
      <td>Lägg till aktivitetsgodkännanden.</td> 
     </tr> 
     <tr> 
    </tbody> 
   </table>

1. Klicka på **X** i panelens övre högra hörn för att stänga den.

## Redigera flera uppgifter samtidigt

Du kan redigera flera åtgärder samtidigt. Se till att du har behörighet att hantera de uppgifter som du har valt gruppvis för att kunna redigera dem.

Redigering av flera uppgifter samtidigt varierar beroende på vilken miljö du väljer.

### Redigera gruppuppgifter i produktionsmiljön

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.
1. Klicka på avsnittet **Åtgärder** i den vänstra panelen.

1. Klicka på ikonen **Planeringsläge** ![Planeringsläge](assets/plan-mode-icon.png) högst upp i listan och kontrollera att alternativet **Spara automatiskt** är markerat.

   ![Aktivera autosparinställningen](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

   >[!IMPORTANT]
   >
   >Du kan inte redigera flera uppgifter samtidigt när du sparar uppgifter manuellt.

1. Markera mer än en uppgift i uppgiftslistan.
1. (Valfritt) Klicka på menyn **Mer** ![Mer](assets/more-icon.png) överst i uppgiftslistan och sedan **Beräkna om uttryck** för att uppdatera all information i beräknade anpassade fält.
1. Klicka på ikonen **Redigera** ![Redigera](assets/qs-edit-icon.png) . Rutan **Redigera uppgifter** öppnas i den nya versionen.

   Att redigera information för alla uppgifter är detsamma som att redigera information för en uppgift.

   Mer information om hur du redigerar en uppgift finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Villkorligt) Gör följande i den nya upplevelsen:

   1. Ange den information som du vill ändra för alla uppgifter som du har markerat i något av följande områden:

      * Översikt
      * Uppdrag
      * Anpassad Forms
      * Ekonomi
      * Inställningar
      * Inställningar
      * Kommentar

      >[!NOTE]
      >
      >* Den information som du ändrar för alla markerade uppgifter åsidosätter den befintliga informationen för enskilda uppgifter, förutom fältet **Uppdrag**. Om du lägger till en ny tilldelad i en gruppredigering läggs den tilldelade personen till i alla markerade uppgifter. Om andra tilldelningar har tilldelats de markerade aktiviteterna, förblir de tilldelade utöver den som lagts till via massredigering.
      >* Om du vill redigera aktivitetens varaktighet måste de markerade aktiviteterna ha samma aktivitetsbegränsning. Annars fylls inte fältet **Varaktighet** i.
      >
      >* Endast aktiva anpassade formulär visas i listan. Om de markerade uppgifterna inte har några vanliga anpassade formulär visas inga formulär i det här avsnittet.
      >* Du kan bara redigera fält i formulären som är kopplade till alla markerade uppgifter och som du har behörighet att redigera.  Mer information om gruppredigering av anpassade formulär finns i [Hantera anpassade formulär som är kopplade till objekt](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).

   1. Klicka på **Spara**.
   1. (Valfritt) Klicka på **Byt tillbaka till den gamla versionen** längst ned i rutan **Redigera uppgifter**.

1. (Villkorligt) Gör följande i den gamla versionen:

   1. Ange den information som du vill ändra för alla uppgifter som du har markerat i något av följande områden:

      * Översikt
      * Inställningar
      * Uppdrag
      * Anpassad Forms
      * Kommentar

   1. (Valfritt) I avsnittet **Anpassade Forms** markerar du alternativet **Beräkna om anpassade uttryck** för att se till att alla beräknade anpassade fält som finns i de anpassade formulär som är kopplade till de valda uppgifterna är aktuella.
   1. Klicka på **Spara ändringar**. Alla ändringar du har gjort visas nu för alla markerade uppgifter.

<div class="preview">

### Redigera flera uppgifter samtidigt i förhandsvisningsmiljön

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.
1. Klicka på avsnittet **Åtgärder** i den vänstra panelen.

1. Klicka på ikonen **Planeringsläge** ![Planeringsläge](assets/plan-mode-icon.png) högst upp i listan och kontrollera att alternativet **Spara automatiskt** är markerat.

   ![Aktivera autosparinställningen](assets/autosave-setting-enabled-quicksilver-task-list-350x308.png)

   >[!IMPORTANT]
   >
   >Du kan inte redigera flera uppgifter samtidigt när du sparar uppgifter manuellt.

1. Markera mer än en uppgift i uppgiftslistan.
1. (Valfritt) Klicka på menyn **Mer** ![Mer](assets/more-icon.png) överst i uppgiftslistan och sedan **Beräkna om uttryck** för att uppdatera all information i beräknade anpassade fält.
1. Klicka på ikonen **Redigera** ![Redigera](assets/qs-edit-icon.png) . Rutan **Redigera uppgifter** öppnas.

   Att redigera information för alla uppgifter är detsamma som att redigera information för en uppgift.

   Mer information om hur du redigerar en uppgift finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. Ange den information som du vill ändra för alla uppgifter som du har markerat i något av följande områden:

   * Översikt
   * Uppdrag
   * Anpassad Forms
   * Ekonomi
   * Inställningar
   * Inställningar
   * Kommentar

   >[!NOTE]
   >
   >* Den information som du ändrar för alla markerade uppgifter åsidosätter den befintliga informationen för enskilda uppgifter, förutom fältet **Uppdrag**. Om du lägger till en ny tilldelad i en gruppredigering läggs den tilldelade personen till i alla markerade uppgifter. Om andra tilldelningar har tilldelats de markerade aktiviteterna, förblir de tilldelade utöver den som lagts till via massredigering.
   >* Om du vill redigera aktivitetens varaktighet måste de markerade aktiviteterna ha samma aktivitetsbegränsning. Annars fylls inte fältet **Varaktighet** i.
   >
   >* Endast aktiva anpassade formulär visas i listan. Om de markerade uppgifterna inte har några vanliga anpassade formulär visas inga formulär i det här avsnittet.
   >* Du kan bara redigera fält i formulären som är kopplade till alla markerade uppgifter och som du har behörighet att redigera.  Mer information om gruppredigering av anpassade formulär finns i [Hantera anpassade formulär som är kopplade till objekt](../../../workfront-basics/work-with-custom-forms/manage-custom-forms-attached-to-objects.md).

1. Klicka på **Spara**.

</div>

