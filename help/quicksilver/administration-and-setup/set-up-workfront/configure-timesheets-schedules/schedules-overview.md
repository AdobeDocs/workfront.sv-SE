---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: användare,schema
navigation-topic: configure-timesheets-and-schedules
title: Översikt över scheman
description: Du kan definiera din arbetsvecka med hjälp av scheman. Du kan associera ett schema med en användare eller ett projekt. Detta gör att  [!DNL Adobe Workfront]  kan beräkna tidslinjer och användartillgänglighet. Instruktioner finns i Skapa ett schema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 32da139d7385e05436a669bdc6f36b71ad83c8d2
workflow-type: tm+mt
source-wordcount: '732'
ht-degree: 0%

---

# Översikt över scheman

<!-- Audited: 1/2024 -->

Du kan definiera din arbetsvecka med hjälp av scheman och associera ett schema med en användare eller ett projekt. Detta gör att [!DNL Adobe Workfront] kan beräkna tidslinjer och användartillgänglighet. Instruktioner finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Tänk på följande när du arbetar med scheman i Workfront:

* Administratören [!DNL Workfront] identifierar arbetstiderna för organisationen i ett schema.

  På samma sätt kan en gruppadministratör identifiera arbetstiderna för ett schema som administreras av en grupp som de hanterar. Mer information om gruppadministratörer finns i [Gruppadministratörer](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Ett schema kan till exempel definieras som: måndag till fredag, 08:00 till 17:00, med en timbrytning till lunch.

* [!DNL Workfront] använder schemat för att avgöra när arbetsdagen börjar och slutar.

  Detta hindrar inte en användare från att arbeta med eller slutföra arbete på [!DNL Workfront] utanför normal kontorstid. Vanligtvis är det inte nödvändigt att skapa ett nytt schema eller ett schemaundantag för att fokusera på det arbete som planeras på kvällen.

  På samma sätt kan din organisation ha flexibla ankomsttider för din arbetsdag. Du kan ha en uppsättning anställda som anländer kl. 8 och en annan uppsättning som anländer kl. 9.00. Det är inte nödvändigt att skapa unika scheman för varje grupp om grupperna har liknande eller identiska scheman. Men om grupperna har helt olika scheman bör deras användare kopplas till unika scheman. En anställd förstår om ett uppdrag ska slutföras kl. 17.00 innebär det att arbetet måste utföras före arbetsdagens slut, oavsett när de börjar arbeta.

* Vi rekommenderar att du skapar separata scheman för varje tidszon som är associerad med organisationen.

  Du kan tilldela en specifik tidszon för varje schema för att se till att arbetet schemaläggs på rätt sätt för användare som arbetar i olika tidszoner.

* Standardschemat [!DNL Workfront] används i tidslinjeberäkningar när användare eller projekt inte är associerade med ett schema.

  Standardschemat levereras med ditt [!DNL Workfront]-system och kan inte tas bort om det inte ersätts med ett nytt schema som du skapar.

* Förutom att beräkna tidslinjer använder [!DNL Workfront] scheman för att beräkna användartillgänglighet.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] använder antingen användaren eller projektschemat för att fastställa resurstillgänglighet i resursplaneraren. Vilket schema som används beror på vad [!DNL Workfront]-administratören har valt för inställningen [!UICONTROL Calculate Resource Availability Using]. Mer information om inställningar för resurshantering finns i [Konfigurera inställningar för resurshantering](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Hierarki med scheman

Om en uppgift har tilldelats en användare som är kopplad till ett schema och finns i ett projekt som är kopplat till ett andra schema, har du minst två scheman som kan användas i tidslinjeberäkningar.

>[!IMPORTANT]
>
>[!DNL Workfront] använder schemat för en användare endast när inställningen [!UICONTROL Calculate Resource Availability Using] är inställd på [!UICONTROL The User's Schedule] i området [!UICONTROL Resource Management] i [!UICONTROL Setup]. Mer information om hur inställningen [!UICONTROL Calculate Resource Availability Using] påverkar vilket schema som används för resurshantering finns i [Konfigurera inställningar för resurshantering](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Den ordning i vilken tidsplanerna används av systemet när det finns fler än ett:

* När en användare tilldelas till en aktivitet använder [!DNL Workfront] användarens schema för att beräkna tidslinjen för aktiviteten. Detta inkluderar även användarens personliga tid. Projektets schema ignoreras.

  Mer information om personlig tid finns i [Konfigurera personlig tid ](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

* När flera användare har tilldelats en uppgift och användarna har olika scheman under aktivitetens tidsram, använder [!DNL Workfront] någon av följande scheman, enligt definitionen i [!UICONTROL Project Preferences]-området i [!UICONTROL Setup]:

   * Schemat för den användare som har utsetts till primär tilldelad
   * Det schema som är associerat med projektet.

     Mer information om projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Om användaren som är tilldelad till aktiviteten inte har något schema, eller om aktiviteten bara är tilldelad till en jobbroll, ett team eller inte är tilldelad, använder [!DNL Workfront] projektschemat för tidslinjeberäkningar.
* Om användaren som är tilldelad till aktiviteten inte har något schema, eller om aktiviteten bara är tilldelad till en jobbroll, ett team eller inte är tilldelad och projektet inte har något schema, använder [!DNL Workfront] schemat i det system som är angivet som standardschema för tidslinjeberäkningar.

  ![](assets/default-schedule.png)

## Collaboration i [!DNL Workfront] över tidszoner

Mer information om hur du använder scheman för att hjälpa användare att samarbeta i [!DNL Workfront] över tidszoner finns i [Arbeta över tidszoner](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
