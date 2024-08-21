---
title: Översikt över anslutna posttyper
description: Ett sätt att ange hur enskilda posttyper relaterar till varandra är att koppla dem. Du kan även koppla posttyperna Adobe Workfront Planning till objekttyper från andra program för att förbättra användarupplevelsen och behålla fokus i ett program.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 0%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# Översikt över anslutna posttyper

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

Du kan ange att enskilda posttyper relaterar till varandra eller till objekt från andra program genom att koppla dem.

Den här artikeln är en översikt över posttypsanslutningar och beskriver de typer av anslutningar som du kan upprätta mellan post- och objekttyper.

Mer information om hur du ansluter posttyper finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).

## Att tänka på när du ansluter posttyper

Det finns två anslutningssteg i Workfront Planning:

1. Först måste du upprätta en anslutning mellan två posttyper eller en posttyp och en objekttyp från ett annat program. Mer information om hur du kan ansluta posttyper finns i [Koppla posttyper](/help/quicksilver/planning/architecture/connect-record-types.md).
1. För det andra kan du koppla enskilda poster av en typ till poster av en annan typ efter att de två posttyperna är kopplade. Mer information om att ansluta poster finns i [Koppla poster](/help/quicksilver/planning/records/connect-records.md).

Tänk på följande när det gäller att ansluta posttyper:

* Du kan ansluta följande enheter i Adobe Workfront Planning:

   * Två posttyper.

     Som standard kan du koppla två posttyper från samma arbetsyta. Du kan också ställa in posttyper för att ansluta till posttyper från andra arbetsytor. Mer information finns i [Redigera posttyper](/help/quicksilver/planning/architecture/edit-record-types.md).
   * En posttyp och en objekttyp från ett annat program.

* Du kan koppla posttyper för Workfront Planning till följande objekttyper från följande program:

   * Adobe Workfront:

      * Projekt
      * Portfolio
      * Program
      * Företag
      * Grupper

   * Adobe Experience Manager Assets:

      * Bilder
      * Mappar

     >[!IMPORTANT]
     >
     >Du måste ha en Adobe Experience Manager Assets-licens och din organisations instans av Workfront måste vara registrerad på Adobe Business Platform eller Adobe Admin Console för att kunna ansluta Workfront Planning-poster till Adobe Experience Manager Assets.
     >
     >Om du har frågor om hur du kommer igång med Adobe Admin Console kan du läsa [Adobe Unified Experience FAQ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* När du har skapat poster för de anslutna posttyperna kan du länka dem till varandra via det anslutna postfältet.  Mer information finns i [Anslut poster](/help/quicksilver/planning/records/connect-records.md).

* När du har kopplat en posttyp till en annan posttyp eller till en objekttyp från ett annat program finns följande scenarier:

   * **När du ansluter två typer av planeringspost** skapas ett länkat postfält för den posttyp som du ansluter från. Ett liknande länkat postfält skapas för den posttyp som du ansluter till.

     Om du till exempel ansluter posttypen&quot;Campaign&quot; med posttypen&quot;Product&quot; skapas ett länkat postfält (anslutningsfält) som du kallar&quot;Linked Product&quot; i posttypen Campaign. En länkad posttyp som automatiskt heter&quot;Campaign&quot; skapas på produktposttypen.

   * **När du ansluter en posttyp med en objekttyp från ett annat program**:

      * Ett länkat postfält skapas för den posttyp som du ansluter från. Inget länkat postfält skapas automatiskt i det andra programmets objekttyp.
      * Planeringspostfält är inte tillgängliga från Workfront-objekt.
      * Du kan planera postfält från Experience Manager-resurser när Workfront-administratören konfigurerar metadatamappningen genom integrationen mellan Workfront och Adobe Experience Manager Assets. Mer information finns i [Konfigurera mappning av metadata för resurser mellan Adobe Workfront och Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
      * Planeringsposter visas på Workfront-objektets planeringflik. Mer information finns i [Hantera poster i planeringsavsnittet för Adobe Workfront-objekt](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

   * **När du lägger till uppslagsfält från posten eller objektet som du ansluter till**: Förutom att skapa ett länkat postfält kan du även ansluta till fält från den anslutna posten eller objekttypen som kallas uppslagsfält. Ett länkat (eller sökfält) med information från den post som du ansluter till visas på den post som du ansluter från.

     Du kan koppla fält från andra posttyper eller objekt från andra program till posttypen Workfront Planning.

     Länkade fält är skrivskyddade och visar automatiskt information från anslutna poster.

     Du kan referera till uppslagsfält från andra post- eller objekttyper i formler, filter eller grupperingar.

     Om du t.ex. kopplar posttypen&quot;Campaign&quot; till ett Workfront-projekt och väljer att överföra fältet Planerat slutförandedatum för projektet till Workfront Planning-posten, skapas automatiskt ett länkat fält med namnet Planerat slutförandedatum (från projekt) för kampanjen. Du kan inte redigera det här länkade fältet manuellt. I fältet Planerat slutförandedatum (från projekt) visas det planerade slutförandedatumet för de länkade projekten.

     >[!IMPORTANT]
     >
     >Alla som har behörighet att visa eller högre på arbetsytan kan visa informationen i sökfälten, oavsett deras behörigheter eller åtkomstnivå i programmet för de länkade objekttyperna eller deras behörigheter i andra arbetsytor.

     Länkade postfält föregås av en relationsikon ![](assets/relationship-field-icon.png).

     Länkade fält föregås av en ikon som anger fälttypen. Länkade (eller uppslag) fält föregås av ikoner som anger att ett fält är ett tal, ett stycke eller ett datum.

<!--## Connection types

After you establish a connection between two record types or between a record and an object type from another application, you can add records in the connected record fields. 

Depending on how many records you can add to a connected record field, the following are the connection types you can choose from when connecting record types: 

* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)

>[!WARNING]
>
>These options are not available when connecting the following: 
>* Two records from different workspaces
>
>* A record type and Experience Manager assets

### Many-to-many connection type

![](assets/many-to-many-connection-picker.png)

When you create a many-to-many connection between record types, you can then select multiple records in the connection field from both record types. 

For example, if you create a many-to-many connection between campaigns and projects, you can select multiple projects for each campaign, and multiple campaigns for each project. 

A real-life example of a many-to-many relationship type is the relationship between movies and actors. Each movie can have multiple actors, and each actor can play in multiple movies. 

When you select this connection type, you cannot change the connection type after you save it. 

### One-to-many connection type

![](assets/one-to-many-connection-picker.png)


When you create a one-to-many connection between record types, you can then select multiple records in the connection field in the current record type, but the corresponding connection field in the record type you connect to will allow selecting only one record. The connected record field that is automatically created on the second record type is automatically set to a many-to-one relationship type. 

For example, if you create a one-to-many connection between campaigns and projects, you can select multiple projects for each campaign, but each project can be connected to only one campaign.

A real-life example of a one-to-many relationship type is the relationship between libraries and books: a library has many books in its inventory; but one particular book can only be in one library at a given point in time. 

When you select this connection type, you can later change it only to a many-to-many connection type. 

### Many-to-one connection type

![](assets/many-to-one-connection-picker.png)


When you create a many-to-one connection between record types, you can then connect each record in the current record type with only one record from the connected record type. The connected record field that is automatically created on the second record type is automatically set to a one-to-many relationship type. 

For example, if you connect campaigns with projects and you choose this type of connection, you can add only one project to a campaign. But you can add multiple campaigns to one project. 

A real-life example of a many-to-one relationship type is the relationship between many movies and one actor: one actor can be in many movies, but each movie can only have a specific actor once in its cast. 

When you select this connection type, you can later change it only to a many-to-many connection type.

### One-to-one connection type

![](assets/one-to-one-connection-picker.png)

When you create a one-to-one connection between record types, in both record types you can connect each record only with one record from the other record type.

For example, if you connect campaigns with projects and you choose this type of connection, you can connect one campaign with one project. One project can be connected only to one campaign. 

A real-life example of a one-to-one relationship is the one existing between a person and their country's unique identifier (like a Social Security Number, Passport ID, local identification ID): each person has only one unique identifier for a country and each unique identifier can be linked to only one person. 

When you select this connection type, you can later change it to any other connection type. 

-->



