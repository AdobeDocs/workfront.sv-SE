---
filename: how-to-delegate-work
navigation-topic: delegate-work
title: Delegera uppgifter och ärenden
description: Du kan tillfälligt delegera det arbete du är tilldelad när du inte är på kontoret. I den här artikeln beskrivs hur du delegerar uppgifter och utfärdar tilldelningar.
author: Alina
exl-id: 42b3112f-4f39-4078-aaa0-623559384a12
source-git-commit: 72a2927d33f40c4fe08888712bdf62e9a5db9c40
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 0%

---

# Hantera delegering av uppgifter och utgåvor

<!--
<NOTE: 
<you might need to change the tile to Delegate PTI, etc, when that functionality is added. Named it this so it will not conflict with the TOC article for Delegate section which was also "Delegate work"
I wrote thhis as a "Manage..." article and I did not add three separate articles, to match what we have for delegating approval requests)
-->

Du kan tillfälligt delegera det arbete du är tilldelad när du inte är på kontoret.

Du kan delegera uppgifter och utleveranser eller delegera godkännanden. I den här artikeln beskrivs hur du delegerar uppgifter och utfärdar tilldelningar.

Allmän information om att delegera arbete finns i [Delegera arbetsöversikt](../../manage-work/delegate-work/delegate-work-overview.md).

## Åtkomstkrav

>[!IMPORTANT]
>
>* De användare som du väljer som ombud får samma behörigheter som dina behörigheter för de uppgifter och utgåvor som du delegerar till dem.
>* Behörigheterna måste fungera inom sina åtkomstnivåer och ibland kan deras åtkomstnivåer vara lägre än dina.

   >
   >   
   >   Om en användare till exempel bara har Visa åtkomst till uppgifter på sin åtkomstnivå och du har behörigheten Hantera för de uppgifter som du delegerar till dem, får de behörigheten Hantera för de uppgifter som du delegerar till dem. De kan dock inte utföra samma åtgärder som du för de delegerade uppgifterna. De måste begära Redigera-åtkomst till uppgifter från systemadministratören för att kunna uppdatera uppgifter om du inte är anställd.
   >
   >   
   >   Mer information om hur en användare kan ändra din åtkomstnivå finns i [Skapa eller ändra anpassade åtkomstnivåer](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
>
>* För artiklar som tilldelas efter att delegeringen redan har startats kan det ta upp till en timme efter det att artikeln har tilldelats [!DNL Workfront] för att dela nyligen tilldelade objekt med ombudet.



Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>Granska eller högre</p>

>[!NOTE]
>
>Även om du kan tilldelas att arbeta när du har en Request-licens, kan du inte delegera ditt arbete till andra. [!DNL Workfront] rekommenderar inte att du tilldelar arbete till gransknings- eller begärananvändare.

</tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter och ärenden Om du fortfarande inte har åtkomst frågar du [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter för de uppgifter eller utgåvor som du har tilldelats</p> 
    <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta [!DNL Workfront] administratör.

<!--note from the table for Object permissions:
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Contribute or higher permissions to the projects where you are designated as the Project&nbsp;Owner (NOTE:&nbsp;you cannot delegate projects yet)</p>
    -->

## Förutsättningar

Innan du kan utföra de aktiviteter som beskrivs i den här artikeln måste du se till följande:

* Dina [!DNL Workfront] eller gruppadministratören aktiverade [!UICONTROL Allow users to delete tasks & issues with logged hours] i [!UICONTROL Setup] ditt område [!DNL Workfront] -instans.

   Mer information finns i [Konfigurera inställningar för uppgifter och problem i hela systemet](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Delegera uppgifter och ärenden till en annan användare

Innan du delegerar arbete till andra rekommenderar vi att du kontaktar dem och informerar dem om att de kommer att utses till delegater på dina arbetsuppgifter. Be om deras muntliga godkännande innan du delegerar arbetet för att försäkra dig om att de har den tid som krävs för att slutföra arbetet medan du är utanför kontoret.

Allmän information om delegering av uppgifter och problem finns i [Översikt över uppgifter och problem i delegering](delegate-work.md).

Så här delegerar du dina uppgifter och utgåvor till andra:

1. Gå till [!UICONTROL **Startsida**] området och klicka sedan på [!UICONTROL **Delegera**] högst upp på [!UICONTROL **Arbetslista**].

   ![](assets/delegate-button-in-home.png)

1. I [!UICONTROL **Delegera uppgifter och ärenden**] uppdaterar du följande:

   * [!UICONTROL **Delegera uppgifter och ärenden till**]: Börja skriva namnet på en användare som du vill att dina uppgifter och utgåvor ska delegeras till och markera sedan den när den visas i listan. Du kan bara välja en användare.\

      Användaren som du väljer som ombud får samma behörigheter som dina behörigheter för de uppgifter och utgåvor som du delegerar till dem. Mer information finns i [Översikt över delegeringsuppgifter och utgåvor](delegate-work-overview.md).

   * [!UICONTROL **Startdatum**]: Välj ett datum i kalendern när delegeringen av dina arbetsobjekt ska börja.

      >[!TIP]
      >
      >Startdatumet får inte vara tidigare.

   * [!UICONTROL **Inget slutdatum**]: Välj det här alternativet om du inte vill ange slutdatumet för din delegering.

   * [!UICONTROL **Slutdatum**]: Välj ett datum i kalendern när delegeringen ska stoppas.

      >[!TIP]
      >
      >Om du inte väljer ett slutdatum aktiveras delegeringen bara för den aktuella dagen.

      ![](assets/delegate-box-expanded-in-home.png)

1. Klicka [!UICONTROL **Spara**].

   Följande saker händer:

   * Ditt arbete delegeras till den angivna användaren. Alla ofullständiga uppgifter eller utgåvor som har datum inom den tidsram du valde (inklusive nyligen tilldelade, efter att delegeringen aktiverats) delegeras.
   >[!TIP]
   >
   >   Slutförda arbetsuppgifter som har datum inom delegeringens tidsram delegeras inte.


   * Du får ett meddelande i skärmens övre högra hörn som bekräftar att du har aktiverat delegering av ditt arbete till en annan användare. Namnet på delegatanvändaren visas i bekräftelsemeddelandet.

   * En indikation på att dina uppgifter och utgåvor har delegerats till andra användare visas på de flesta områden där du kan se tilldelningar i [!DNL Workfront]. Mer information om vilka områden som inte innehåller delegaternas namn finns i [Översikt över delegeringsuppgifter och utgåvor](delegate-work-overview.md).

   * The [!UICONTROL **Delegera**] i [!UICONTROL Home] område ändras till [!UICONTROL **Redigera delegering**] ange att det finns en delegering på plats.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: is this shot correct?&nbsp;See UI - this is a mock)
   </MadCap:conditionalText>
   -->

   ![](assets/work-delegated-button-in-home.png)

   * Om dina händelsemeddelanden och dina personliga meddelanden är aktiverade får du också en e-postbekräftelse från din delegering.

   * Användaren som du har valt som ombud får ett e-postmeddelande om delegeringen, om deras händelsemeddelanden är aktiverade.

      Mer information om hur du aktiverar personliga e-postmeddelanden finns i [Aktivera eller inaktivera egna händelsemeddelanden](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).





## Redigera eller stoppa delegering

Du kan låta en delegering förfalla, om du har valt ett slutdatum, eller så kan du stoppa det manuellt. Du kan också ändra tidsramen för delegeringen om datumen för delegeringen ändras.

1. Gå till [!UICONTROL Home] området och klicka sedan på [!UICONTROL Edit delegation] i det övre högra hörnet av arbetslistan.
1. I [!UICONTROL Delegate tasks and issues] gör du något av följande:
   * Ändra [!UICONTROL **Startdatum**] eller [!UICONTROL **Slutdatum**]
   * Klicka [!UICONTROL **Stoppa delegering**]

   >[!TIP]
   >
   >    Du kan bara redigera slutdatumet för en delegering om delegeringen redan har startats.

   ![](assets/stop-delegation-screen-in-home.png)

1. (Villkorligt) klicka [!UICONTROL **Spara**] för att spara nya delegeringsdatum

   eller

   Klicka [!UICONTROL **Stoppa delegering**] i bekräftelserutan för att bekräfta att delegeringen stoppats.

   Delegeringen har antingen uppdaterat datumen eller stoppat och de delegerade användarna har tagits bort från dina uppgifter och problem. Deras behörigheter till uppgifter och problem finns kvar.


## Hitta information om delegerat arbete och delegerande

<!--(if this was released, make sure that viewing delegated approvals has not changed, as documented here: /Content/Review and approve work/Manage Approvals/delegate-approval-requests.html) 
-->

När uppgifter och ärenden delegeras finns det flera områden i [!DNL Workfront] där du kan se det delegerade arbetet eller vilka delegaterna är.

* [Hitta delegater i rutan Uppdrag](#locate-delegates-in-the-assignments-box)
* [Hitta delegerat arbete i [!UICONTROL Home]](#locate-delegated-work-in-home)


### Hitta delegater i [!UICONTROL Assignments] box

När din system- eller gruppadministratör aktiverar delegering av arbete i ditt system [!UICONTROL Assignments] visas följande flikar där du kan komma åt dem:

* [!UICONTROL **Uppdrag**]: Användare som är tilldelade uppgiften eller utgåvan visas här.
* [!UICONTROL **Delegeringar**]: Användare som har utsetts till delegater av de som har tilldelats uppgiften eller problemet visas här.

Du kommer åt [!UICONTROL Assignments] i följande områden:

* Aktivitets- eller utgivningsrubriken

   ![](assets/assignments-and-delegates-panel-in-task-header.png)

   The [!UICONTROL Assignments] fält i uppgifts- eller utgivningsrubriken ändras till [!UICONTROL Assignments and delegations].

* The [!DNL Workload Balancer] när uppgifter eller problem tilldelas manuellt

   ![](assets/assignments-and-delegates-panel-in-workload-balancer.png)

>[!NOTE]
>
> Du kan inte visa delegater i [!UICONTROL Assignments] i en åtgärd eller i rutan Redigera problem.

Om en uppgift eller ett ärende delegeras och [!UICONTROL Delegations] underfliken är tom. Ett av följande scenarier kan finnas:

* Du har inte tilldelats uppgiften eller utgåvan.
* Aktivitets- eller utgivningsdatumet ligger utanför delegeringens tidsram.

>[!TIP]
>
>Planerade eller faktiska timmar för delegerade uppgifter och ärenden beaktas inte i resurshanteringsverktyg, som [!DNL Workload Balancer] eller [!DNL Resource Planner] för de delegerade användarna. Timmarna förblir bara kopplade till den tilldelade användaren.

### Hitta delegerat arbete i [!UICONTROL Home]

1. Gå till [!UICONTROL **Startsida**] klickar du på listrutan för filter och väljer ett eller flera av följande alternativ:
   * [!UICONTROL **Delegerad**]: för att visa uppgifter och ärenden som delegerats till dig eller av dig.
   * [!UICONTROL **Delegerat till mig**]: för att visa uppgifter och ärenden som delegerats till dig av en annan användare.
   * [!UICONTROL **Delegerad av mig**]: om du vill visa uppgifter och utgåvor som du har delegerat till andra användare.

   ![](assets/delegated-to-me-or-by-me-filters-in-home.png)

1. Klicka på [!UICONTROL sorting] för att sortera listan efter följande kriterier:
   * [!UICONTROL Planned Completion]. Detta är standardalternativet för sortering.
   * [!UICONTROL Planned Start]
   * [!UICONTROL Commit Date]
   * [!UICONTROL Project]
   * [!UICONTROL My Priority]
1. Expandera grupperingarna i [!UICONTROL **Arbetslista**] om du vill visa delegerade arbetsobjekt. Följande scenarier finns:
   * För objekt som du har delegerat till andra visas delegatens namn i [!UICONTROL **Arbetslista**] och [!UICONTROL **Uppdrag och delegationer**] till höger.

   * För objekt som har delegerats till dig visas den tilldelades namn i [!UICONTROL **Arbetslista**] och **[!UICONTROL Assignments and delegations]** till höger.
   >[!TIP]
   >
   >    Om delegeringen är inställd på att börja ett datum efter dagens datum, visas också delegeringens startdatum i [!UICONTROL Work List]. De delegerade objekten visas i den gruppering du väljer för [!UICONTROL Work List], enligt grupperingens typ. Om du t.ex. grupperar efter [!UICONTROL Planned Completion Date]visas de delegerade objekten i grupperingen som matchar deras planerade slutförandedatum.
