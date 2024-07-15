---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definiera timtyper och tillgänglighet
description: En timtyp är en etikett som du kan använda för att kategorisera tidsangivelser. Beroende på organisationens rapporteringskrav för timmar kan detta vara en viktig del av loggningstiden.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: bfaf566e556882078875649549c0dfadacd800b8
workflow-type: tm+mt
source-wordcount: '1470'
ht-degree: 0%

---

# Definiera timtyper och tillgänglighet

En timtyp är en etikett som du kan använda för att kategorisera tidsangivelser. Beroende på organisationens rapporteringskrav för timmar kan detta vara en viktig del av loggningstiden.

Det finns två uppsättningar timtyper i Adobe Workfront:

* **Allmänna timmar:** timmar som inte är associerade med ett projekt, till exempel sjuktid eller administration. Du kan bara logga allmänna timmar på tidrapporten.
* **Projektspecifika timmar:** timmar loggade in på projekt, uppgifter och problem. Du kan logga projektspecifika timmar från alla platser där du kan logga tid.

När du loggar in i Workfront beror de projektspecifika timtyperna som är tillgängliga på de konfigurationsalternativ som ställs in på system-, projekt- och användarnivå. (Följande standardtyper av projektspecifika timmar är alltid tillgängliga: Projekttid, Aktivitetstid och Utgivningstid.)

De timtyper som är tillgängliga att välja när loggningstiden (i projekt, uppgifter och ärenden) bestäms först av de timtyper som systemadministratören gör tillgängliga, och sedan av de timtyper som valts på projekt- och användarnivå.

När rätt timtyper har konfigurerats kan du logga tid från flera platser i Workfront, enligt beskrivningen i [Loggtid](../../timesheets/create-and-manage-timesheets/log-time.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Planera eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Systemadministratörsåtkomst för att definiera systemomfattande timtyper och för att redigera alla användare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Hantera åtkomst till projektet för att definiera timtyper i ett projekt</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill ta reda på vilken plan eller licenstyp du har.

+++

## Definiera tillgänglighet på systemnivå

Systemadministratören avgör vilka projektspecifika timtyper som blir tillgängliga i hela systemet, enligt beskrivningen i [Hantera timtyper](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definiera tillgänglighet på projektnivå {#define-availability-at-the-project-level}

Projektägaren avgör om alla timtyper som definieras på systemnivå är tillgängliga i projektet (och uppgifter och ärenden inom projektet) eller om bara en delmängd av dessa timtyper är tillgängliga.

1. Gå till projektet där du vill fastställa tillgängligheten för timtyper.
1. Klicka på menyn **Mer** bredvid aktivitetsnamnet och klicka sedan på **Redigera**.

1. Klicka på **Redigera projekt**.
1. Gå till alternativet **Filtertimtyper** i avsnittet **Inställningar**.

1. Välj **Nej** om du vill göra alla projektspecifika timtyper tillgängliga i projektet.

   eller

   Välj **Ja** om du bara vill göra en delmängd av de projektspecifika timtyperna tillgängliga i projektet. Välj sedan de timtyper som du vill göra tillgängliga. (Håll ned Skift om du vill markera flera timtyper.)

   Om du väljer det här alternativet blir endast de timtyper som du väljer tillgängliga när du loggar timmar i projektet (eller om uppgifter och problem i projektet). Om du väljer det här alternativet och inte väljer några timtyper visas endast allmänna timtyper.

   Samma val måste göras på den enskilda användarnivån för att användaren ska kunna se dessa alternativ för timtyper i projektet.

   När användarens standardtimtyp och en projekts filtrerade timtyp matchar, väljs timtypen som standard vid loggningstid.

1. Klicka på **Spara ändringar**.

## Definiera tillgänglighet på användarnivå

Du kan bara logga timmar för en viss timtyp i projekt, uppgifter och utgåvor om timtypen har gjorts tillgänglig på systemnivå, projektnivå och användarnivå.

Om du gör en timtyp tillgänglig på användarnivå enligt beskrivningen i det här avsnittet, men du inte ser den timtypen när du loggar tid för ett projekt, en uppgift eller ett problem, har timtypen inte gjorts tillgänglig i projektet (enligt beskrivningen i [Definiera tillgänglighet på projektnivå](#define-availability-at-the-project-level)).

Så här definierar du de timtyper som är tillgängliga för en användare:

1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på din avatar i det övre vänstra hörnet.
1. Klicka på menyn **Mer** bredvid användarnamnet och klicka sedan på **Redigera**.

1. Endast en systemadministratör kan redigera andra användare. Om du har en planlicens kan du redigera timtyperna i din egen profil.
1. I avsnittet **Resursplanering** gör du något av följande i listrutan **Tillgängliga timtyper**, beroende på vilka timtyper du vill göra tillgängliga när du loggar tid för ett projekt, en uppgift eller ett problem:

   * **Gör alla timtyper tillgängliga för användaren:** Markera alla timtyper.\
     Om du låter alla timtyper vara omarkerade är detta tekniskt detsamma som att välja alla timtyper. I det här fallet är dock alla timtyper bara tillgängliga för användaren i projekt, uppgifter och ärenden där **Nej** har valts i alternativet **Filtertimtyper** när projektet redigeras, vilket beskrivs i [Definiera tillgänglighet på projektnivå](#define-availability-at-the-project-level) .
   * **Om du bara vill göra en delmängd av timtyperna tillgängliga för användaren:** Markera endast de timtyper som du vill göra tillgängliga.

     För att timtyperna som du väljer på användarnivå ska vara tillgängliga för projekt, uppgifter och utgåvor måste dessa timtyper också väljas i alternativet **Filtrera timtyper** när du redigerar projektet, vilket beskrivs i [Definiera tillgänglighet på projektnivå](#define-availability-at-the-project-level).

1. (Valfritt) Välj en timtyp i listrutan **Standardtimtyp**.

   När användarens standardtimtyp och en projekts filtrerade timtyp matchar, väljs timtypen som standard vid loggningstid.

1. Klicka på **Spara ändringar**.

   När du loggar timmar i ett projekt, en uppgift eller ett ärende är de timtyper du väljer tillgängliga om samma timtyper har gjorts tillgängliga på projektnivå.


## Hur timtyper på användarnivå och projektnivå fungerar tillsammans

I följande lista beskrivs vilka timtyper som visas på ett objekt efter att du har anpassat och filtrerat timtyper på både användarnivå och projektnivå när du loggar tid på objektet:

* När du har anpassat standardtimtypen för användaren och de filtrerade timtyperna för projekt visas en av följande timtyper på den nedrullningsbara menyn Timtyp:

   * När användaren har en standardtimtyp i sin profil och projektet har samma filtrerade timtyp, visas den här timtypen som vald standardtyp vid loggningstid: Projekt, Aktivitet eller Ärendetid som ytterligare alternativ.

   * När användaren inte har någon standardtimtyp och projektet har filtrerade timtyper, visas standardtimtypen för loggningstid som Projekt, Aktivitet eller Utgivningstid, men de filtrerade timtyperna från projektet visas också som ytterligare alternativ.

   * När användaren inte har någon standardtimtyp och projektet inte har några filtrerade timtyper visas bara timtyperna Projekt, Aktivitet eller Utgivningstid som standard, beroende på vilket objekt du loggar tid till.

   * När användaren har en standardtimtyp och projektet inte har några filtrerade timtyper, visas projekt-, uppgifts- eller problemtimtyp som standard när användaren loggar in på objekten och inga andra timtyper är tillgängliga som alternativ, inklusive användarens standardtimtyp.

* När du har anpassat timtyper och definierat tillgängliga timtyper för användaren eller filtrerat timtyper för ett projekt finns följande scenarier:

   * När du har valt alla timtyper för fältet Tillgänglig timtyp i din användarprofil, och projektets timtyper inte filtreras, visas alla tillgängliga timtyper när du loggar tid.
   * När du bara har valt en delmängd av timtyper för fältet Tillgänglig timtyp i din användarprofil och projektets timtyper inte filtreras, visas endast användarens timtyper när du loggar tid.
   * När du har valt alla timtyper för fältet Tillgänglig timtyp i din användarprofil, och projektets timtyper har filtrerats, visas endast projektets timtyper och standardtimtyper som Projekttid, Aktivitetstid, Utgivningstid beroende på objektet.
   * När du bara har valt en delmängd av timtyper för fältet Tillgänglig timtyp i din användarprofil och projektets timtyper filtreras, visas bara de timtyper som är gemensamma för användaren och projektet. Om inga timtyper är gemensamma för användaren och projektet visas endast standardtimtyperna (Projekttid, Aktivitetstid, Utgivningstid).

>[!TIP]
>
>   Om du väljer en annan timtyp i stället för standardtimtypen för ett objekt, kommer timtypen att klistras in. Nästa gång du loggar in på samma objekt blir timtypen automatiskt den som du senast valde.

