---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Preview 5
description: Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön med R1 Preview 5. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 16 mars 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 0%

---

# R1 Preview 5

Den här sidan beskriver alla ändringar som är tillgängliga i förhandsvisningsmiljön med R1 Preview 5. Funktionerna på den här sidan gjordes tillgängliga i förhandsvisningsmiljön den 16 mars 2017.

En lista över alla ändringar som gjorts i R1 finns i [Aktivitetsöversikt för R1-release](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## Spåra projektförlopp med en användningsrapport

Nu kan en användare med behörigheten Hantera för ett projekt följa upp projektets förlopp med hjälp av en användningsrapport.

Tack vare utnyttjanderapporten kan du hålla ditt projekt inom budgeten genom att snabbt se hur de faktiska timmarna spårar mot de budgeterade timmarna eller planerade timmarna för en viss vecka eller månad, eller för hela projektet. Dessutom kan du visa detaljerad information om antalet timmar i varje kategori (budgeterad, planerad och faktisk), kategoriserat efter jobbroll eller enskild användare.

Mer information om hur du spårar användning i ett projekt finns i [Översikt över resursanvändningsrapporten](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

Som systemadministratör kan du konfigurera om fliken Användning ska vara tillgänglig för användare. Fliken Utnyttjande finns som standard i listrutan Mer i ett projekt. Du kan flytta fliken Användning till en annan plats eller dölja den helt. Om du har definierat anpassade layoutmallar för användare i din organisation måste du lägga till fliken Användning manuellt i de anpassade layoutmallarna.

Mer information om hur du konfigurerar platsen för fliken Utnyttjande finns i&quot;Anpassa flikar&quot; i&quot;Skapa och hantera layoutmallar&quot;.

## Ändra en befintlig global godkännandeprocess för ett enskilt objekt

Nu kan du ändra en befintlig global godkännandeprocess när du kopplar den globala godkännandeprocessen till ett objekt. De ändringar du gör gäller bara för godkännandeprocessen för objektet där du associerar det.

Mer information finns i [Associera en ny eller befintlig godkännandeprocess med arbete](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) in [Associera en ny eller befintlig godkännandeprocess med arbete](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## Konfigurera rapporter så att det nya Gantt-schemat visas som standard

Du kan konfigurera projekt- och uppgiftsrapporter som du skapar så att det nya Gantt-schemat visas som standard med det nya alternativet &quot;Visa den här rapporten i en Gantt-vy som standard&quot;.

Mer information om hur du konfigurerar rapporter för att visa det nya Gantt-schemat finns i [Redigera rapportinställningar](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

Mer information om hur du visar Gantt-schemat i projektrapporter och aktivitetsrapporter finns i [Visa information i Gantt-schemat](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)&quot; in [Visa information i Gantt-schemat](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## Förbättring av papperskorgen: Aktiviteter och underaktiviteter återställs till föregående ordning

När du återställer en uppgift eller en underuppgift efter att den har tagits bort återställs uppgiften eller underaktiviteten till sin tidigare plats (antingen i uppgiftslistan eller under den överordnade uppgiften), i samma ordning som den såg ut innan den togs bort.

Före den här ändringen återställdes uppgifter och underaktiviteter som återställdes alltid som den senaste uppgiften (antingen i uppgiftslistan eller under den överordnade uppgiften), oavsett i vilken ordning de visades innan de togs bort.

Mer information om hur du återställer objekt i Workfront finns i [Återställ borttagna objekt](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Förbättringar av vyn Milstolpe

Följande förbättringar är nu tillgängliga när du visar en projektlista eller en projektrapport i vyn Milstolpe:

* **Konfigurera om förloppsstatus och Procent färdigt ska visas i vyn:** Det finns ett nytt alternativ som gör att du kan konfigurera om Progress Status-ikoner ska visas i vyn Milstolpe. Dessutom kan du konfigurera om informationen Procent färdigt ska visas för projekt och uppgifter.\
  Mer information finns i [Använda vyn Milstolpe](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [Använda vyn Milstolpe](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Redigera Procent färdigt direkt från vyn Milstolpe:** Nu kan du redigera Procent färdigt i projekt och uppgifter direkt i vyn Milstolpe.\
  Mer information finns i [Använda vyn Milstolpe](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) in [Använda vyn Milstolpe](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md). 

## Uppdaterat utseende och känsla för flera systemkonfigurationssidor

Utseendet på följande sidor på menyn System i inställningsområdet har uppdaterats (funktionen är densamma):

* Diagnostik
* enkel inloggning (SSO) som innehåller:

   * Active Directory
   * LDAP
   * SAML 1.1
   * SAML 2.0

* Uppdatera användare för enkel inloggning

## Uppdaterade grupperingar för händelsemeddelanden i området för e-postinställningar

Organisationshuvuden för händelsemeddelanden i området E-postinställningar matchar nu avsnittsrubrikerna som används i området för användarprofilsinställningar.

Mer information om händelsemeddelanden finns i  [Konfigurera händelsemeddelanden för alla i systemet](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Opt out of Instant Notifications: In-Context Digest Configuration

Följande alternativ är nu tillgängliga i e-postmeddelanden direkt. De här alternativen är bara tillgängliga för snabbmeddelanden som också har en daglig sammanfattningsmotsvarighet:

* &quot;Lägg till det här i en daglig sammanfattning&quot;
* &quot;Stoppa e-postmeddelanden av den här typen&quot;

När du får ett e-postmeddelande direkt kan du nu antingen lägga till det meddelandet i ett dagligt meddelande eller helt avbryta prenumerationen på det meddelandet.

Dessa alternativ är tillgängliga i e-postmeddelandet. Mer information om hur du tar emot e-postmeddelanden finns i [Adobe Workfront-meddelanden](../../../../workfront-basics/using-notifications/wf-notifications.md)

## Olika e-postmeddelanden har flyttats från avsnittet Åtgärd krävs till andra projektrelaterade avsnitt

Flera meddelanden har flyttats från avsnittet Åtgärd krävs på användarprofilsidan till andra avsnitt, enligt följande:

Mer information om hur du konfigurerar e-postmeddelanden finns i [Ändra dina egna e-postmeddelanden](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Meddelande</strong> </th> 
   <th><strong>Gammalt avsnitt</strong> </th> 
   <th><strong>Nytt avsnitt</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ett problem har lagts till i ett projekt som jag äger</td> 
   <td> <p> Åtgärd krävs </p> </td> 
   <td>   <p>Information om projekt som jag äger</p></td> 
  </tr> 
  <tr> 
   <td>Ett problem har lagts till i ett projekt som jag är på</td> 
   <td>   <p>Åtgärd krävs</p><p> </p></td> 
   <td> <p> Information om projekt som jag äger </p>   </td> 
  </tr> 
  <tr> 
   <td>Ett otilldelat problem läggs till i ett projekt som jag äger</td> 
   <td>   <p>Åtgärd krävs</p></td> 
   <td>   <p>Information om projekt som jag äger</p></td> 
  </tr> 
  <tr> 
   <td> <p> Ett ej tilldelat problem läggs till i ett projekt som jag är på </p> </td> 
   <td> <p> Åtgärd krävs </p>   </td> 
   <td> <p> Information om projekt som jag äger </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> Bekräftelsedatumet ändras för en aktivitet i ett projekt </p> </td> 
   <td>   <p>Åtgärd krävs</p></td> 
   <td>   <p>Information om projekt som jag äger</p></td> 
  </tr> 
  <tr> 
   <td> <p> Bekräftelsedatumet ändras för ett problem i ett projekt </p>   </td> 
   <td>   <p>Åtgärd krävs</p></td> 
   <td> <p> Information om projekt som jag äger </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> Förfallodatumet ändras för en uppgift som jag har tilldelats till </p> </td> 
   <td>   <p>Åtgärd krävs</p></td> 
   <td>   <p>Information om arbete som tilldelats mig</p></td> 
  </tr> 
  <tr> 
   <td> <p> Förfallodatumet ändras för en utgåva som jag har tilldelats till </p> </td> 
   <td> <p> Åtgärd krävs </p>   </td> 
   <td>   <p>Information om arbete som tilldelats mig</p></td> 
  </tr> 
  <tr> 
   <td> <p> Statusändringarna för en uppgift som jag har tilldelats till </p>   </td> 
   <td> <p> Åtgärd krävs </p>   </td> 
   <td> <p> Information om arbete som tilldelats mig </p>   </td> 
  </tr> 
 </tbody> 
</table>

## Ny resursplaneringsfunktion (ej tillgänglig i produktion i R1)

>[!NOTE]
>
>Den här funktionen är för närvarande tillgänglig i förhandsvisningsmiljön. Den tas bort från förhandsvisningsmiljön ungefär en månad innan R1-versionen släpps för produktion. Den återinförs sedan i förhandsvisningsmiljön i R2 Preview 1.

 

Följande ändringar har lagts till som stöd för den framtida resursplaneringsfunktionen:

* Den aktuella fliken Resursplanering har bytt namn till Äldre resursplanering i området Personer. 
* En ny flik, &quot;Resursplanering&quot;, har lagts till i området Personer där den nya funktionen ska utvecklas.\
  Mer information om den nya fliken Resursplanering finns i [Kom igång med resursplanering](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md) 

* Det aktuella resurspoolobjektet har bytt namn till &quot;Äldre resurspool&quot;.\
  Mer information om hur du skapar nya användarbaserade resurspooler finns i [Översikt över resurspooler](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* Ett nytt resurspool-objekt har skapats med stöd för de nya (användarbaserade) resurspoolerna.

  >[!NOTE]
  >
  >
  >   
  >   
  * Om du för närvarande kör rapporter om befintliga äldre resurspooler ändras inte de befintliga rapporterna.
  * Om du vill skapa en ny rapport för de befintliga (jobbrollbaserade) äldre resurspoolerna måste du välja &quot;Äldre resurspooler&quot; som objekt för rapporten.
  * Om du vill skapa en ny rapport för de nya (användarbaserade) resurspoolerna måste du välja Resurspooler som objekt för rapporten.
  >   
  >
