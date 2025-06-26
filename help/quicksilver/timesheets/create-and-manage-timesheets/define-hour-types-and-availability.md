---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definiera timtyper och tillgänglighet
description: En timtyp är en etikett som du kan använda för att kategorisera tidsangivelser. Beroende på organisationens rapporteringskrav för timmar kan detta vara en viktig del av loggningstiden.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: 594f224e11b0e7708ed555410b7c331741113791
workflow-type: tm+mt
source-wordcount: '1488'
ht-degree: 0%

---

# Definiera timtyper och tillgänglighet

<!--Audited: 6/2025-->

En timtyp är en etikett som du kan använda för att kategorisera tidsangivelser. Beroende på organisationens rapporteringskrav för timmar kan detta vara en viktig del av loggningstiden.

Det finns två uppsättningar timtyper i Adobe Workfront:

* **Allmänna timmar**: Timmar som inte är associerade med ett projekt, till exempel sjuktid eller administration. Du kan bara logga allmänna timmar på tidrapporten.
* **Projektspecifika timmar**: Timmar som är inloggade på projekt, uppgifter och problem. Du kan logga projektspecifika timmar från valfri plats där du kan logga tid.

När du loggar in i Workfront beror de projektspecifika timtyperna som är tillgängliga på de konfigurationsalternativ som ställs in på system-, projekt- och användarnivå. (Följande standardtyper av projektspecifika timmar är alltid tillgängliga: Projekttid, Aktivitetstid och Utgivningstid.)

De timtyper som är tillgängliga att välja när loggningstiden (i projekt, uppgifter och ärenden) bestäms först av de timtyper som systemadministratören gör tillgängliga, och sedan av de timtyper som valts på projekt- och användarnivå.

När rätt timtyper har konfigurerats kan du logga tid från flera platser i Workfront. Mer information finns i [Loggtid](../../timesheets/create-and-manage-timesheets/log-time.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Nytt: Standard</p> 
   <p>Aktuell: Planera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Systemadministratörsåtkomst för att definiera systemomfattande timtyper och för att redigera alla användare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Hantera åtkomst till projektet för att definiera timtyper i ett projekt</td> 
  </tr> 
 </tbody> 
</table>

*Mer information om informationen i den här tabellen finns i [Åtkomstkraven i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Definiera tillgänglighet på systemnivå

Systemadministratören avgör vilka projektspecifika timtyper som blir tillgängliga i hela systemet. Mer information finns i [Hantera timtyper](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definiera tillgänglighet på projektnivå {#define-availability-at-the-project-level}

Projektägaren avgör om alla timtyper som definieras på systemnivå är tillgängliga i projektet (och uppgifter och ärenden inom projektet) eller om bara en delmängd av dessa timtyper är tillgängliga.

{{step1-to-projects}}

1. På sidan **Projekt** väljer du det projekt som du vill fastställa tillgängligheten för timtyper för.
1. Klicka på ikonen **Mer** ![Mer ](assets/more-icon.png) bredvid projektnamnet i sidhuvudet och klicka sedan på **Redigera**. Panelen **Redigera projekt** öppnas.

1. Gå till inställningen **Filtertimtyper** i avsnittet **Projektinställningar**.

1. Välj **Nej** om du vill göra alla projektspecifika timtyper tillgängliga i projektet.

   eller

   Välj **Ja** om du bara vill göra en delmängd av de projektspecifika timtyperna tillgängliga i projektet och välj sedan de **timtyper** som du vill göra tillgängliga. Du kan välja flera timtyper.

   >[!NOTE]
   >
   >   Tänk på följande:
   >   
   >   * Om du väljer **Ja** blir endast de timtyper som du väljer tillgängliga när du loggar timmar i projektet (eller om aktiviteter och problem i projektet).
   >   
   >   * Om du väljer **Ja** och inte väljer några timtyper visas endast allmänna timtyper.
   >
   >   * Samma val måste göras på den enskilda användarnivån för att användaren ska kunna se dessa alternativ för timtyper i projektet.
   >
   >   * När användarens standardtimtyp och ett projekt av typen Filtrerad timtyp matchar, väljs timtypen som standard vid loggningstid.

1. Klicka på **Spara**.

## Definiera tillgänglighet på användarnivå

Du kan bara logga timmar för en viss timtyp i projekt, uppgifter och utgåvor om timtypen har gjorts tillgänglig på systemnivå, projektnivå och användarnivå.

Om du gör en timtyp tillgänglig på användarnivå enligt beskrivningen i det här avsnittet men inte ser timtypen när du loggar in på ett projekt, en uppgift eller ett problem, har timtypen inte gjorts tillgänglig i projektet. Mer information finns i följande avsnitt i den här artikeln: [Definiera tillgänglighet på projektnivå](#define-availability-at-the-project-level).

Så här definierar du de timtyper som är tillgängliga för en användare:

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på din avatar i det övre vänstra hörnet.

   eller

   Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/adobe-main-menu.png) i det övre högra hörnet, om den är tillgänglig, och klicka sedan på **Workfront-profil**.

1. Klicka på ikonen **Mer** ![Mer](assets/more-icon.png) bredvid användarnamnet och klicka sedan på **Redigera**. Rutan **Redigera person** öppnas.

   >[!IMPORTANT]
   >
   >Endast en systemadministratör kan redigera andra användare. Om du har en planlicens kan du redigera timtyperna i din egen profil.


1. I avsnittet **Resursplanering** gör du något av följande i listrutan **Tillgängliga timtyper**, beroende på vilka timtyper du vill göra tillgängliga när du loggar tid för ett projekt, en uppgift eller ett problem:

   * **Gör alla timtyper tillgängliga för användaren:** Markera alla timtyper.\
     Om du låter alla timtyper vara omarkerade är detta tekniskt detsamma som att välja alla timtyper. I det här fallet är dock alla timtyper bara tillgängliga för användaren i projekt, uppgifter och ärenden där **Nej** har valts i alternativet **Filtertimtyper** när projektet redigeras, vilket beskrivs i [Definiera tillgänglighet på projektnivå](#define-availability-at-the-project-level) .
   * **Om du bara vill göra en delmängd av timtyperna tillgängliga för användaren:** Markera endast de timtyper som du vill göra tillgängliga.

     För att timtyperna som du väljer på användarnivå ska vara tillgängliga för projekt, uppgifter och utgåvor måste dessa timtyper också väljas i alternativet **Filtrera timtyper** när du redigerar projektet, vilket beskrivs i [Definiera tillgänglighet på projektnivå](#define-availability-at-the-project-level).

1. (Valfritt) Välj en timtyp i listrutan **Standardtimtyp**. När användarens standardtimtyp och en projekts filtrerade timtyp matchar, väljs timtypen som standard vid loggningstid.

1. Klicka på **Spara ändringar**. När du loggar timmar i ett projekt, en uppgift eller ett ärende blir de timtyper du väljer tillgängliga om samma timtyper har gjorts tillgängliga på projektnivå.

## Hur timtyper på användarnivå och projektnivå fungerar tillsammans

I följande lista beskrivs vilka timtyper som visas på ett objekt efter att du har anpassat och filtrerat timtyper på både användarnivå och projektnivå när du loggar tid på objektet:

* När du har anpassat standardtimtypen för användaren och de filtrerade timtyperna för projekt visas en av följande timtyper på den nedrullningsbara menyn Timtyp:

   * När användaren har en standardtimtyp i sin profil och projektet har samma filtrerade timtyp, visas den här timtypen som vald standardtyp vid loggningstid: Projekt, Aktivitet eller Ärendetid som ytterligare alternativ.

   * När användaren inte har någon standardtimtyp och projektet har filtrerade timtyper, visas standardtimtypen för loggningstid som Projekt, Aktivitet eller Utgivningstid, men de filtrerade timtyperna från projektet visas också som ytterligare alternativ.

   * När användaren inte har någon standardtimtyp och projektet inte har några filtrerade timtyper visas bara timtyperna Projekt, Aktivitet eller Utgivningstid som standard beroende på vilket objekt du loggar tid till.

   * När användaren har en standardtimtyp och projektet inte har några filtrerade timtyper visas projektet, aktiviteten eller problemtiden som standard när användaren loggar in på objekten. Inga andra timtyper är tillgängliga som alternativ, inklusive användarens standardtimtyp.

* När du har anpassat timtyper och definierat tillgängliga timtyper för användaren eller filtrerat timtyper för ett projekt finns följande scenarier:

   * När du har valt alla timtyper för fältet Tillgänglig timtyp i din användarprofil och projektets timtyper inte har filtrerats visas alla tillgängliga timtyper när du loggar tid.
   * När du bara valde en delmängd av timtyper för fältet Tillgänglig timtyp i din användarprofil och projektets timtyper inte filtreras, visas endast användarens timtyper när du loggar tid.
   * När du har valt alla timtyper för fältet Tillgänglig timtyp i din användarprofil och projektets timtyper har filtrerats, visas endast projektets timtyper och standardtimtyper som Projekttid, Aktivitetstid, Utgivningstid beroende på objektet.
   * När du bara valde en delmängd av timtyper för fältet Tillgänglig timtyp i din användarprofil och projektets timtyper filtreras, visas bara de timtyper som är gemensamma för användaren och projektet. Om inga timtyper är gemensamma för användaren och projektet visas endast standardtimtyperna (Projekttid, Aktivitetstid, Utgivningstid).

>[!TIP]
>
>   Om du väljer en annan timtyp än standardtimtypen för ett objekt blir timtypen fast. Nästa gång du loggar in på samma objekt blir timtypen automatiskt den som du senast valde.

