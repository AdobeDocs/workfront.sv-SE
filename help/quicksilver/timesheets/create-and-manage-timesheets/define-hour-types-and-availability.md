---
product-area: timesheets;system-administration
navigation-topic: create-and-manage-timesheets
title: Definiera timtyper och tillgänglighet för tidrapporter
description: En timtyp är en etikett som du kan använda för att kategorisera tidsangivelser. Beroende på organisationens rapporteringskrav för timmar kan detta vara en viktig del av loggningstiden.
author: Alina
feature: Timesheets
exl-id: 3c07a6b0-4751-4fce-ac28-6a83084025d4
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# Definiera timtyper och tillgänglighet för tidrapporter

En timtyp är en etikett som du kan använda för att kategorisera tidsangivelser. Beroende på organisationens rapporteringskrav för timmar kan detta vara en viktig del av loggningstiden.

Det finns två uppsättningar timtyper i Adobe Workfront:

* **Allmänna timmar:** Timmar som inte är kopplade till ett projekt, t.ex. sjuktid eller administration. Du kan bara logga allmänna timmar på tidrapporten.
* **Projektspecifika timmar:** Timmar som är inloggade på projekt, uppgifter och problem. Du kan logga projektspecifika timmar från alla platser där du kan logga tid.

När du loggar in i Workfront beror de projektspecifika timtyperna som är tillgängliga på de konfigurationsalternativ som ställs in på system-, projekt- och användarnivå. (Följande standardtyper av projektspecifika timmar är alltid tillgängliga: Projekttid, Aktivitetstid och Utfärdandetid.)

De timtyper som är tillgängliga att välja när loggningstiden (i projekt, uppgifter och ärenden) bestäms först av de timtyper som systemadministratören gör tillgängliga, och sedan av de timtyper som valts på projekt- och användarnivå.

När rätt timtyper har konfigurerats kan du logga tid från flera platser i Workfront enligt beskrivningen i [Loggtid](../../timesheets/create-and-manage-timesheets/log-time.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

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

&#42;Kontakta Workfront-administratören om du vill veta vilken plan eller licenstyp du har.

## Definiera tillgänglighet på systemnivå

Systemadministratören avgör vilka projektspecifika timtyper som blir tillgängliga i hela systemet enligt beskrivningen i [Hantera timtyper](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md) avsnitt i  [Hantera timtyper](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/hour-types.md).

## Definiera tillgänglighet på projektnivå {#define-availability-at-the-project-level}

Projektägaren avgör om alla timtyper som definieras på systemnivå är tillgängliga i projektet (och uppgifter och ärenden inom projektet) eller om bara en delmängd av dessa timtyper är tillgängliga. 

1. Gå till projektet där du vill fastställa tillgängligheten för timtyper.
1. Klicka på **Mer** -menyn bredvid aktivitetsnamnet och sedan klicka på **Redigera**.

1. Klicka **Redigera projekt**.
1. I **Inställningar** -avsnittet, leta upp **Timtyper för filter** alternativ.

1. Välj **Nej** för att göra alla projektspecifika timtyper tillgängliga i projektet.

   eller

   Välj **Ja** Om du bara vill göra en delmängd av de projektspecifika timtyperna tillgängliga i projektet väljer du de timtyper du vill göra tillgängliga. (Håll ned Skift om du vill markera flera timtyper.)

   Om du väljer det här alternativet blir endast de timtyper som du väljer tillgängliga när du loggar timmar i projektet (eller om uppgifter och problem i projektet). Om du väljer det här alternativet och inte väljer några timtyper visas endast allmänna timtyper.

   Samma val måste göras på den enskilda användarnivån för att användaren ska kunna se dessa alternativ för timtyper i projektet.

1. Klicka **Spara ändringar**.

## Definiera tillgänglighet på användarnivå

Du kan bara logga timmar för en viss timtyp i projekt, uppgifter och utgåvor om timtypen har gjorts tillgänglig på systemnivå, projektnivå och användarnivå.

Om du gör en timtyp tillgänglig på användarnivå enligt beskrivningen i det här avsnittet, men du inte ser den timtypen när du loggar in på ett projekt, en uppgift eller ett problem, har timtypen inte gjorts tillgänglig i projektet (enligt beskrivningen i [Definiera tillgänglighet på projektnivå](#define-availability-at-the-project-level)).

Så här definierar du de timtyper som är tillgängliga för en användare:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på din avatar i det övre vänstra hörnet.
1. Klicka på **Mer** -menyn bredvid användarnamnet och klicka sedan på **Redigera**.

1. Endast en systemadministratör kan redigera andra användare. Om du har en planlicens kan du redigera timtyperna i din egen profil.
1. I **Resursplanering** i **Tillgängliga timtyper** gör något av följande, beroende på vilka timtyper du vill göra tillgängliga när du loggar in på ett projekt, en uppgift eller ett problem:

   * **Så här gör du alla timtyper tillgängliga för användaren:** Markera alla timtyper.\
      Om du låter alla timtyper vara omarkerade är detta tekniskt detsamma som att välja alla timtyper. I det här fallet är dock alla timtyper tillgängliga för användaren endast i projekt, uppgifter och ärenden där **Nej** är markerat i **Timtyper för filter** vid redigering av projektet, enligt beskrivningen i [Definiera tillgänglighet på projektnivå](#define-availability-at-the-project-level).
   * **Så här gör du bara en delmängd av timtyperna tillgängliga för användaren:** Välj bara de timtyper som du vill göra tillgängliga.

      För att timtyperna som du väljer på användarnivå ska vara tillgängliga för projekt, uppgifter och ärenden måste samma timtyper också väljas i **Timtyper för filter** vid redigering av projektet, enligt beskrivningen i [Definiera tillgänglighet på projektnivå](#define-availability-at-the-project-level).

1. Klicka **Spara ändringar**.

   När du loggar timmar i ett projekt, en uppgift eller ett ärende är de timtyper du väljer tillgängliga om samma timtyper har gjorts tillgängliga på projektnivå.
