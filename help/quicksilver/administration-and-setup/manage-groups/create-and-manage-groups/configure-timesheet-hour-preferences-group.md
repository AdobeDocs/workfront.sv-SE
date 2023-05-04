---
user-type: administrator
product-area: system-administration;user-management
keywords: grupp,inställningar,uppgift,grupper,problem,låsa upp
navigation-topic: create-and-manage-groups
title: Konfigurera tidrapport och timinställningar för en grupp
description: På systemnivå kan en Adobe Workfront-administratör låsa upp tidrapport- och timinställningsavsnitten Allmänna inställningar och Fyll i i förväg med tidrapporter. Detta gör att gruppadministratörer kan konfigurera alternativen i dessa avsnitt separat för sina egna grupper.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1ee9343e-9452-4e41-a9ff-a6c865d4813b
source-git-commit: 3b0a82381d1c33d897b123a597df21ba54cc2565
workflow-type: tm+mt
source-wordcount: '1368'
ht-degree: 0%

---

# Konfigurera tidrapport och timinställningar för en grupp

{{highlighted-preview}}

En Adobe Workfront-administratör kan låsa upp följande avsnitt av tidrapport och timinställningar på systemnivå så att gruppadministratörer kan konfigurera dem oberoende av varandra för sina egna grupper:

* Allmänna inställningar
* <span class="preview">Var användarna kan logga tid</span>
* Förifyll tidrapporter

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

Följande avsnitt på sidan Inställningar för tidrapport och timmar kan bara konfigureras på systemnivå och kan inte låsas upp för grupper:

* Borttagna projekt, uppgifter och ärenden

Mer information om hur en Workfront-administratör låser upp en tidrapport och timinställning finns i avsnittet [Lås upp tidrapport och timinställningar för grupper](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) i artikeln [Konfigurera tidrapport och timinställningar](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

>[!TIP]
>
>Konfiguration på gruppnivå kan även användas för projektinställningar och för uppgifter och utgåvor. Mer information finns i [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) och [Konfigurera inställningar för aktiviteter och utgåvor för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

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

## Gruppera tidrapport och timinställningar

Tänk på följande information om hur du konfigurerar en olåst tidrapport eller timinställning för en grupp:

* Om du är gruppadministratör och konfigurerar en tidrapport eller timinställning för gruppen, påverkar det personer som använder gruppen som hemgrupp.
* Normalt förblir en olåst inställning olåst i oändlighet. Om Workfront-administratören låser om den aktiveras systeminställningen igen och inställningarna som gjorts av gruppadministratörerna går förlorade.
* En tidrapport ärver tidrapport- och timinställningarna som konfigurerats för tidrapportägarens hemgrupp.

   <!--
  Add example here?
  -->

* När en Workfront-administratör har låst upp en inställning på systemnivå och konfigurerat den för din grupp kan du sedan låsa den för att se till att alla i grupperna under din använder samma konfiguration. Detta är parallellt med möjligheten för en Workfront-administratör att konfigurera och låsa en inställning för alla i systemet. Mer information finns i [Lås eller lås upp en grupptidrapport och timinställning](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

## Konfigurera en olåst tidrapport eller timinställning för en grupp

>[!TIP]
>
>Om du är Workfront-administratör kan du kringgå steg 1-4 genom att gå till Inställningar > Tidrapport och timmar > Inställningar och sedan söka efter gruppens namn i rutan längst upp på sidan.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Grupper** ![](assets/groups-icon.png).

1. Klicka på namnet på gruppen vars tidrapport eller timinställningar du vill konfigurera.
1. Klicka på i den vänstra panelen **Tidrapporter och timmar**.

1. På sidan som visas i **Allmänna inställningar** konfigurerar du något av följande alternativ:

   >[!TIP]
   >
   >Om du håller muspekaren över en inställning och ett verktygstips visas som talar om att den är låst, kan du be Workfront-administratören att låsa upp den för alla grupper i organisationen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Loggtid för framtida datum</td> 
      <td> <p>Tillåter användare att logga tid för framtida datum i hela systemet i:</p> 
       <ul> 
       <li>Projekt, uppgifter och problem där de har åtkomst till loggtid, oavsett projektgrupp</li> 
       <li>Deras tidrapporter som allmän tid</li>
       </ul> 
       <p>Detta är användbart när användare tänker vara borta från kontoret och vill logga in den tiden i förväg.</p> 
       <p><b>ANMÄRKNING</b>: Du kan inte hindra användare från att logga in på uppgifter eller problem som har stängts eller avbrutits. Du kan bara hindra användare från att logga in på fullständiga eller döda projekt. Vi rekommenderar att du använder filter i listor med uppgifter och problem för att utesluta de som har slutförts eller avbrutits från att vara synliga för användarna.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lägga till utgifter från en tidrapport</td> 
      <td> <p>Gör att användare kan registrera både tid och utgifter i tidrapporten.</p> 
      <p>När den här inställningen är aktiverad för en grupp och gruppen är inställd som hemgrupp för vissa användare, visas en utgiftsikon bredvid projekt och uppgifter på dessa användares tidrapporter. Användarna kan klicka på den här ikonen för att lägga till eller redigera utgifter för projektet eller uppgiften.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tilldela jobbroller till timposter manuellt</td> 
      <td> <p>Tillåt användare att manuellt välja en jobbroll som tilldelats i deras användarprofil eller tilldelats till objektet.</p> <p><b>VIKTIGT</b>:  
        <ul> 
         <li>Om du inaktiverar den här inställningen efter att du har tilldelat jobbroller till timposter, måste användarna justera timmar som loggats under olika roller på fliken Timmar i projektet, uppgiften eller utgåvan.</li> 
         <li>Om användaren inte har tilldelats någon jobbroll i sin profil och det finns en uppgift tilldelad som aktivitetsägare i dialogrutan Avancerade uppdrag, visas den jobbrollen när användaren loggar tid för uppgiften.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Begränsa redigering av tidrapporter till ägare och administratörer</td> 
      <td> <p>Begränsa redigering till tidrapportägare, oavsett projektgrupp och Workfront-administratörer. När det här alternativet är inaktiverat kan tidrapporter även redigeras av:</p> 
       <ul> 
        <li> <p>Användare med administrativ åtkomst till tidrapporter och timmar på åtkomstnivå</p> </li> 
        <li> <p>Tidrapporten godkänner om"Kan redigera timmar" är aktiverat på tidrapporten</p> </li> 
        <li> <p>Chefen för tidrapportägaren</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Begränsa timredigering till ägare och administratörer</td> 
      <td>Begränsa redigeringen till den användare som anger timmar och Workfront-administratörer. Den här inställningen gäller för fliken Timmar i ett projekt eller i en timrapport.</td> 
     </tr> 
    </tbody> 
   </table>

1. <span class="preview">I **Var användarna kan logga tid** konfigurerar du något av följande alternativ:</span>

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><span class="preview">Logga tid direkt i projekt</span></td> 
      <td><span class="preview">Tillåter användare att logga tid på projektet (både på fliken Uppdateringar och på tidrapporten). Om du vill hindra användarna från att registrera tid på projektnivå låter du det här alternativet vara avmarkerat.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><span class="preview">Logga in på projekt som är slutförda</span></td>
      <td><span class="preview">Tillåter användare att registrera tid i ett projekt som har markerats som slutfört. Om det här alternativet är inaktiverat kan användare inte registrera tid för det arbete de har slutfört i projekt med statusen Fullständigt.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><span class="preview">Logga in på projekt som är döda</span></td> 
      <td><span class="preview">När det här alternativet är aktiverat kan användare logga timmar i projekt med statusen Död.</span></td>
     </tr>
    </tbody>
   </table>

   >[!NOTE]
   >
   >Den här inställningen används baserat på konfigurationen av användarens hemgruppsinställningar. Om de här inställningarna är aktiverade i användarens hemgruppsinställningar kan användaren logga tiden direkt i projekt, inklusive slutförda eller döda projekt, oavsett om det är tillåtet enligt projektets gruppinställningar eller inte.

1. I **Förifyll tidrapporter** konfigurerar du något av följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Arbete som finns i &lt;number of="" weeks=""&gt; av tidrapportens arbetsområde</td> 
      <td> <p>Definierar antalet veckor före och efter datumintervallet för tidrapporten som innehåller datum för uppgifter och ärenden som tilldelats användaren. Standardinställningen är 1 vecka, och du kan utöka intervallet till 4 veckor. Det innebär att tidrapporten är förifylld med uppgifter och ärenden som har datum var som helst mellan fyra veckor före datumintervallet i tidrapporten upp till fyra veckor efter datumintervallet i tidrapporten, om du väljer 4 veckor för intervallet. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Uppgifter och ärenden som har slutförts</td> 
      <td>Om flera resurser vanligtvis tilldelas till en enskild uppgift rekommenderar vi den här inställningen. Detta innebär att när en resurs registrerar tid mot aktiviteten och markerar den som slutförd, kan de andra resurser som tilldelats aktiviteten fortfarande hitta uppgiften eller problemet i sin tidrapport för att registrera sina timmar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aktiviteter och problem som har planerade datum i tidrapportens datumintervall</td> 
      <td> <p>När du väljer det här alternativet innehåller tidrapporten uppgifter och utgåvor som har antingen ett planerat startdatum eller ett slutförandedatum som ligger inom datumintervallet för tidrapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> Uppgifter som har projektdatum i tidrapportens datumintervall</td> 
      <td> <p>När det här alternativet är markerat innehåller tidrapporten uppgifter som antingen har ett planerat startdatum eller ett slutförandedatum som ligger inom tidsramen för projektet, även om det planerade datumet för utleveransen eller uppgiften ligger utanför tidsintervallet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **Spara**.
