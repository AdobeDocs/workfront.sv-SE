---
title: Posttypöversikt för arbetsytan över
description: Du kan aktivera posttyper som ska vara globala eller anslutningsbara. Globala posttyper kan läggas till i flera arbetsytor från en central eller primär arbetsyta i Adobe Workfront Planning, medan kopplingsbara posttyper kan anslutas till från andra arbetsytor än sina egna.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: aeedd871-dcd3-4fb3-bfc5-99db3e7c9296
source-git-commit: 5bccad02f90fd99135b50c5a929913b16cc5b809
workflow-type: tm+mt
source-wordcount: '1640'
ht-degree: 0%

---


# Posttypöversikt för arbetsytan över flera arbetsytor

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span> -->

{{planning-important-intro}}

Du kan aktivera funktioner för olika arbetsytor för en posttyp i Adobe Workfront Planning. En posttyp för arbetsytan kan refereras till eller nås från mer än en arbetsyta.

>[!IMPORTANT]
>
>Din organisation måste köpa följande paket för att kunna aktivera funktioner för olika arbetsytor för olika posttyper:
>
>Så här konfigurerar du kopplingsbara posttyper:
>
>
>* Alla Workfront-paket och alla Planning-paket
>
>   eller
>
>* Alla arbetsflöden och ett Planning Prime- eller Ultimate-paket
>
>Så här konfigurerar du globala posttyper:
>
>* Alla Workfront-paket och ett Planning Plus-paket
>     
>   eller
>
>* Alla arbetsflöden och ett Planning Prime- eller Ultimate-paket
>
>Mer information om vad som ingår i respektive Workfront Planning-paket får du av Workfront.
>Mer information finns i [Åtkomstöversikt för Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).

Följande är funktioner för olika arbetsytor för posttyper:

* **Globala posttyper**: Användare kan lägga till globala posttyper i andra arbetsytor som de hanterar.

* **Anslutningsbara posttyper**: Användare kan ansluta till den här posttypen från andra arbetsytor.

I den här artikeln finns en översikt över posttyper för arbetsytor. Mer information om hur du definierar en posttyps funktioner för arbetsytan mellan olika arbetsytor finns i [Konfigurera funktioner för arbetsytor mellan arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

## Översikt över globala posttyper

Globala posttyper kan läggas till på flera arbetsytor från en central eller primär arbetsyta i Workfront Planning.

När du implementerar Workfront Planning för en organisation med flera team och gemensamma arbetsflöden kan du behöva definiera en sammanhängande struktur och metadata för nyckelposttyper (som kampanjer och slutprodukter) som kan läggas till i varje teames arbetsytor för att fånga och hantera deras arbete.

Ni kan också behöva varje teames arbete för att komma till en central nivå.

I ett sådant arbetsflöde kan du se till att teamen hämtar sitt arbete på ett enhetligt sätt samtidigt som de låser upp synligheten mellan team, utan att behöva lägga till allt på en arbetsyta, eller så kan alla i organisationen göra det på varje arbetsyta. Du kan använda globala posttyper för att uppnå detta.

Så här använder du globala posttyper:

1. Konfigurera en posttyp som global på en arbetsyta som du hanterar.

   En arbetsytehanterare kan ge behörigheter till användare med en standardlicens, eller till team, grupper, roller och företag för att lägga till en vald posttyp i de arbetsytor som de hanterar.

   Den ursprungliga posttypen kommer att finnas på den ursprungliga arbetsytan, men kommer att synas på andra arbetsytor.

   Mer information finns i [Konfigurera funktioner för arbetsytan över arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Lägg till en posttyp på en sekundär arbetsyta från en befintlig som har konfigurerats som en global posttyp.

   Posttypen kommer att finnas på följande arbetsytor:

   * Dess ursprungliga arbetsyta där den angavs som global posttyp.
   * En sekundär arbetsyta.

   Mer information finns i [Lägga till befintliga posttyper från en annan arbetsyta](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).

   I följande avsnitt beskrivs överväganden om globala posttyper och hur de fungerar på antingen den ursprungliga eller den sekundära arbetsytan.

### Att tänka på när det gäller globala posttyper på deras ursprungliga arbetsyta

Posttypen som konfigurerats som global har följande egenskaper:

* All information (utseende, originalfält) kan bara redigeras på den ursprungliga arbetsytan.

* Du kan utföra följande åtgärder på den globala posttypen från den ursprungliga arbetsytan:

   * Redigera den

     När du redigerar en global posttyp kan du redigera dess utseende, funktioner för flera arbetsytor och alla fält som har skapats på den ursprungliga arbetsytan.
   * Dela

     När du delar en posttyp läggs användarna till på arbetsytan och posterna delas med dessa användare.
   * Ta bort den

     Du kan bara ta bort en global posttyp från den ursprungliga arbetsytan efter att du har tagit bort alla instanser av den från alla de sekundära arbetsytorna där den lades till.

     Mer information finns i [Ta bort posttyper](/help/quicksilver/planning/architecture/delete-record-types.md).
   * Gör den anslutningsbar från andra arbetsytor
   * Skapa och hantera förfrågningsformulär
   * Skapa och hantera automatisering

* Posterna som du lägger till i en global posttyp visas bara för användare som har behörigheten Visa på arbetsytan där de lades till.
* Posterna som du lägger till från en sekundär arbetsyta läggs upp och visas på den ursprungliga arbetsytan. Alla medlemmar på den ursprungliga arbetsytan får behörigheten Visa till dem.
* När den ursprungliga globala posttypen läggs till i flera sekundära arbetsytor finns följande scenarier:

   * Medlemmar i den ursprungliga arbetsytan får automatiskt behörigheten Visa för alla poster som läggs till från en arbetsyta, även om de inte är medlemmar i den arbetsytan.
   * Sekundära arbetsytemedlemmar kan bara visa poster från arbetsytor där de är medlemmar.

* Posttyperna som är kopplade till en global posttyp blir tillgängliga för anslutning från arbetsytorna där den här posttypen läggs till.

  Om du till exempel har en global posttyp för Campaign som har en anslutning till posttypen Region, och du lägger till posttypen Campaign på en sekundär arbetsyta, kan regioner bli en kopplingsbar arbetsyta mellan olika arbetsytor från den sekundära arbetsytan. Medlemmar i den sekundära arbetsytan kan nu skapa kampanjer och länka dem till regioner.

* Fält som skapats för en global posttyp från den ursprungliga arbetsytan visas från alla arbetsytor där posttypen läggs till.

  Du kan bara redigera fältinställningar från den ursprungliga arbetsytan.

  Inställningarna för de fält som skapades i den ursprungliga arbetsytan är skrivskyddade i de sekundära arbetsytorna för alla medlemmar, oavsett deras behörigheter på den sekundära arbetsytan.

  Sekundära arbetsytehanterare kan inte ändra fältinställningarna för fält som konfigurerats i den ursprungliga arbetsytan. Det är bara arbetsytehanterarna på den ursprungliga arbetsytan som kan ändra fältinställningarna på den ursprungliga arbetsytan.

### Överväganden om globala posttyper i en sekundär arbetsyta

* Deltagare på den sekundära arbetsytan får Contribute-behörighet till den globala posttypen på deras arbetsyta. De kan lägga till och hantera poster i den från den sekundära arbetsytan.

* De sekundära arbetsytevisningsprogrammen får behörigheten Visa för den globala posttypen på deras arbetsyta. De kan inte lägga till och hantera poster i den.

* Sekundära arbetsytehanterare kan utföra följande åtgärder på posttypen som lagts till från en global posttyp på en sekundär arbetsyta:

   * Ta bort den.

     Om du tar bort posttypen från en sekundär arbetsyta tas den bara bort från den sekundära arbetsytan. Posterna och fälten som läggs till i den sekundära arbetsytan tas också bort från den sekundära arbetsytan. Posterna som läggs till i den sekundära arbetsytan finns kvar på den primära arbetsytan. Detta tar inte bort posttypen från den ursprungliga arbetsytan eller från andra sekundära arbetsytor där den har lagts till.

     Mer information finns i [Ta bort posttyper](/help/quicksilver/planning/architecture/delete-record-types.md).

   * Dela

     Genom att dela en global posttyp på en sekundär arbetsyta händer följande också:

      * Användare läggs till på arbetsytan med behörigheten Visa.
      * Användarna får samma behörigheter som alla poster av den globala posttypen på den sekundära arbetsytan.
   * Dela vyerna för posttyperna.

     Du kan inte dela en vy offentligt från en global posttyp på en sekundär arbetsyta. Du kan bara dela vyer internt från en sekundär arbetsyta. Du kan dela en vy internt och offentligt för en global posttyp på den ursprungliga arbetsytan.

     Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).


<!--when they will be able to add fields to the secondary space, this bullet will need this extra information: 
    After adding fields to the global record type in the secondary workspace, shared views might not open for other users in workspaces. The fields exist only in the secondary workspace and they would not be visible in any other workspace. Only fields created in the primary workspace are visible in all secondary workspaces where there the record type is added.-->

<!--These two capabilities will come later - and edit some of the bullets below after these capabilities are released:
* Add new fields
    Fields added to a global record from a secondary workspace are visible only from the secondary workspace. 
* Add request forms to it
* Add automations to it-->

* Ingen användare kan utföra följande åtgärder på en global posttyp på en sekundär arbetsyta:

   * Redigera den

     Du kan inte redigera utseendet, funktionerna för en arbetsyta eller fälten som lagts till från den ursprungliga arbetsytan.
   * Skapa och hantera förfrågningsformulär
   * Skapa och hantera automatisering

* Poster som läggs till i en sekundär arbetsyta visas från följande arbetsytor om du har behörigheten Visa eller högre för dessa arbetsytor:

   * Den sekundära platsen där de lades till
   * Den globala posttypens ursprungliga arbetsyta

* Följande scenarier finns för poster som skapats i sekundära arbetsytor:

   * Om du har behörigheten Hantera på den ursprungliga arbetsytan, och inga behörigheter på en sekundär arbetsyta, kan du visa poster som lagts till från den sekundära arbetsytan i den ursprungliga arbetsytan, men du kan inte hantera dem från den ursprungliga arbetsytan.
   * Om du har behörigheten Hantera på den sekundära arbetsytan kan du hantera posterna både från den globala posttypens ursprungliga arbetsyta och från den sekundära arbetsytan där de lades till.
     <!--not anymore: * You can view the records in additional secondary workspaces where the global record type is added only if you have View permissions to those workspaces-->
* Du kan inte dela vyer offentligt från en global posttyp på en sekundär arbetsyta.

### Åtkomst till anslutningar av global posttyp

Posttyper som är kopplade till den globala posttypen på den ursprungliga arbetsytan blir synliga från andra arbetsytor där den globala posttypen läggs till och de är tillgängliga för anslutningar från de sekundära arbetsytorna där den globala posttypen läggs till.

### API-åtkomst för en global posttyp

När du lägger till poster till en global posttyp från en sekundär arbetsyta med hjälp av Workfront Planning API, kontrollerar systemet om användaren har åtkomst att skapa poster på den ursprungliga arbetsytan för den globala posttypen.

Följande fall finns:

* Om användaren har åtkomst skapas posten på den globala posttypens ursprungliga arbetsyta.

* Om användaren inte har åtkomst får användaren ett felmeddelande om att han/hon inte har åtkomst till den globala posttypens ursprungliga arbetsyta och måste ange det arbetsyte-ID där han/hon har åtkomst för att skapa poster.

## Översikt över kopplingsbara posttyper

Du kan ansluta till en posttyp som har definierats som anslutningsbar från en arbetsyta som du hanterar.

Dina team kan behöva länka sina poster till posttyper från andra arbetsytor eller visa information som samlats in på poster som tillhör poster på andra arbetsytor. Du kan uppnå den här konfigurationen genom att ange en posttyp som anslutningsbar.

Så här använder du kopplingsbara posttyper:

1. Konfigurera en posttyp som ska kunna anslutas på en viss arbetsyta.

   En arbetsytehanterare kan välja vilka arbetsytor en angiven posttyp kan ansluta till.

   Den ursprungliga posttypen kommer att finnas på den ursprungliga arbetsytan och det går att ansluta till den från en annan arbetsyta.

   Mer information finns i [Konfigurera funktioner för arbetsytan över arbetsytor för posttyper](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).
1. Anslut till en posttyp som är angiven som anslutningsbar från en annan arbetsyta som du hanterar.

   Mer information finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
