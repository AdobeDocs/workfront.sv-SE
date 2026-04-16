---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Definiera tariffattribut
description: Graderingsattribut utökar Adobe Workfront funktion för hastighetskort och tariffer genom att göra det möjligt att lägga till ytterligare dimensioner till hastigheter utöver jobbrollen. Workfront kan sedan automatiskt välja rätt tilldelningsgrad för att säkerställa att alla projekt är ekonomiskt korrekta och konsekventa.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d570ef6a-935f-4dd0-9c54-a480163ec9d8
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '1373'
ht-degree: 0%

---

# Definiera tariffattribut

Graderingsattribut utökar Adobe Workfront funktion för hastighetskort och tariffer genom att göra det möjligt att lägga till ytterligare dimensioner till hastigheter utöver jobbrollen. Detta är viktigt för myndigheter och företag där priset inte bara varierar beroende på befattningsroll utan även på faktorer som myndighet, plats, varumärke, kostnadsställe eller andra.
Genom att kombinera dessa attribut kan Workfront automatiskt välja rätt grad för tilldelningar, vilket garanterar att alla projekt är ekonomiskt korrekta och konsekventa.

>[!IMPORTANT]
>
>Klassificeringsattribut är en grundkonfiguration som används en gång.

När attributen har aktiverats och tillämpats på tariffkort och priser kan en senare ändring av dem äventyra dataintegriteten i hela din finansiella konfiguration.

## Översikt över tariffattribut

Klassificeringsattribut betraktas som en engångsinställning eftersom:

* Attribut blir en del av den finansiella datamodellen när de har aktiverats.
* Hastigheter, tilldelningar, planerade värden och faktiska värden beror alla på de valda attributvärdena.
* Om du ändrar attribut senare (byter namn, tar bort eller ändrar ordning) kan det orsaka:

   * Förlorad koppling mellan satser och attribut
   * Ogiltiga eller &quot;överblivna&quot; frekvenser
   * Feljustering vid fakturering och rapportering

Därför bör attribut utformas noggrant under den initiala Workfront-implementeringen och ändras inte efteråt.

### Objekt som används som tariffattribut

Workfront har för närvarande stöd för tre systemobjekt som kan användas som tariffattribut:

* **Grupp**: Namnet har ofta ändrats till _Agency_ eller _Business Unit_.
* **Företag**: Kan representera _varumärke_, _klient_ eller _kund_.
* **Plats**: Används vanligtvis som _Market_, _Region_ eller _Office_.

  Platsen är hierarkiskt definierad upp till 3 nivåer. (Exempel: Om du definierar&quot;Plats&quot; som Los Angeles används även Kalifornien och USA i matchningar.)

Du kan byta namn på objekten så att de matchar organisationens terminologi när du skapar attributen.
Exempel:

* &quot;Agency&quot; label = Group object reference
* Etiketten&quot;Kostnadsställe&quot; = Referens för undergruppsobjekt
* &quot;Location&quot; label = Location object reference

Detta gör att konfigurationen kan spegla din affärsstruktur samtidigt som Workfront datamodell upprätthålls.

### Anteckningar om tariffattribut i Workfront

* Workfront har stöd för upp till 5 attributnivåer. Systemet följer alltid attributhierarkin och väljer den mest specifika matchningen som är tillgänglig.

   * 0 = generisk basränta
   * 1 - 5 = progressivt mer specifika frekvenser

* Du kan byta namn på attribut så att de återspeglar din verksamhet (byrå, varumärke, marknad, kostnadsställe, osv.).
* Installationen är endast en gång: om du ändrar attributen senare riskerar du att skada den finansiella dataintegriteten.
* Attribut som inte refereras någonstans i systemet kan tas bort på ett säkert sätt.

  Om ett attribut redan används (refereras i tariffkort, användarprofiler, resurser eller tilldelningar) blockeras borttagningen för att skydda dataintegriteten. I dessa fall uppstår ett fel om du försöker ta bort attributet, särskilt genom ett API-anrop.

* Testa före publicering: Skapa ett pilottariffkort och validera att rätt frekvenser löses i tilldelningar.
* Dokumentera konfigurationen: Dela dina prisattribut med era team så att de förstår hur taxorna fungerar.

### Var tariffattribut kan användas

Attributen för prissättning stöds i alla områden där det finns tariffer i Workfront:

* Klassificeringskort: Definiera frekvenser per jobbroll plus attribut.
* Åsidosättningar på projektnivå: Använd attribut när du åsidosätter frekvenser på projektnivå.
* Jobbroller (i konfigurationen): Ange standardrollfrekvenser för jobb med attribut.
* Användare (användarprofiler): Tilldela enskilda användare systemspecifika attribut så att deras tilldelningar automatiskt anpassas till rätt frekvenser.

<!--
BULLET POINT Staffing plan resources
BULLET POINT Non-labor resources: Attributes can also be defined on resources such as equipment or services.-->

<!--Non-labor resource categories and -->Jobbroller saknar stöd för hastighetsattribut direkt på objektnivå. De är kopplade till tariffattribut via de hastigheter som definierats på dem.

När du kan skapa platshållartilldelningar som är knutna till rätt attributvärden, fylls dina värden i i enlighet med detta.

* När du senare ersätter platshållaren med en riktig användare för jobbroller återställer systemet automatiskt tilldelningens attribut till dem som definierats i användarens profil. I det här läget kan attribut inte längre redigeras på uppdragsnivån. De ärver från användaren för att bevara konsekvensen och förhindra felpassning mellan användarattribut och tillämpad frekvens.

<!-- BULLET POINT For non-labor resource categories, placeholder assignments can be used similarly: You assign the category through a placeholder that carries the required attributes. Once the actual non-labor resource is substituted, the attributes are automatically pulled from the resource's profile. Just like with users, these attributes cannot be overridden manually at the assignment level, ensuring financial data integrity and preventing accidental mismatches between resources and their designated attributes.-->

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>Arbetsflöde Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera tariffattribut

Varje attribut har en uppsättning konfigurerbara alternativ, inklusive allmänna egenskaper och filter.
Filter styr hur attributvärden föreslås och valideras när frekvenser definieras. De är nödvändiga för att attributmarkeringarna ska vara konsekventa, för att hjälpa användarna att hitta giltiga alternativ och för att förhindra ogiltiga kombinationer.

{{step-1-to-setup}}

1. Klicka på **Klassificeringsattribut** i den vänstra panelen.
1. Klicka på en plusteckenikon i diagrammet för att lägga till ett attribut.

   >[!NOTE]
   >
   >Du kan ha upp till fem attribut i diagrammet. Ordningen uppifrån och ned definierar hierarkin för hur attributen tillämpas. Klicka på ikonen **Rotera** ![Rotera](assets/rotate-attribute-view-icon.png) för att visa diagrammet från vänster till höger. Du kan också zooma in eller ut och anpassa diagrammet till skärmen.

1. Välj ett attribut för att öppna konfigurationspanelen till höger på skärmen.

   ![Konfigurera tariffattribut](assets/configure-rate-attributes.png)

1. Byt namn på objekten (Grupp, Företag, Plats) till de villkor som behövs för ditt företag (till exempel Byrå, Plats, Kostnadsställe).
1. Klicka på **Spara** för varje attribut för att spara namnkonventionen.

   Namnen på dessa attribut visas på alla tariffkort och frekvenser i systemet.

1. Ange egenskaperna för varje attribut på konfigurationspanelen:

   * **Obligatoriskt**: Välj om attributet är ett obligatoriskt fält för frekvenser.
   * **Ska användas i intäktsberäkning**: Inkluderar det här attributet i faktureringsberäkningar.
   * **Ska användas i kostnadsberäkning**: Inkluderar det här attributet i kostnadsberäkningar.

     >[!NOTE]
     >
     >Minst ett av beräkningsalternativen måste väljas för att attributet ska fungera i finansiella beräkningar.

   * (Valfritt) **Hierarkisk**: Tillåter attributet att respektera överordnade-underordnade relationer, till exempel Ort > Läge > Land.

     Den här egenskapen är bara tillgänglig för Location-objektet.

### Definiera filter för attributen

Det finns två typer av filter för attributen:

* Förslagsfilter begränsar listan med tillgängliga alternativ baserat på systemlogik eller tidigare attributval. De gör listrutor sammanhangsberoende och enkla att använda.

  Exempel: Byrå > Plats > Kostnadsställe

  I den här inställningen bör attributet för kostnadsställe ha ett förslagsfilter som refererar till både byrå och plats.

  När du lägger till en frekvens och först väljer Agency = &quot;Star&quot;, föreslår listrutan Location bara platser som tillhör &quot;Star&quot;.

  Om du sedan väljer Location = Chicago för taxan föreslår listrutan Cost Center bara de kostnadsställen som är kopplade till &quot;Star&quot; och Chicago.

* Relationsfilter skapar en beroendekedja mellan attribut. De ser till att systemet förstår hur attribut relaterar till varandra och framtvingar giltiga beroenden.

  Exempel: Byrå > Plats > Kostnadsställe

  I den här konfigurationen bör byråns attribut ha ett relationsfilter som knyter det till giltiga platser och kostnadsställen.

Filter måste alltid konfigureras i båda riktningarna. Om attribut A har ett relationsfilter med attribut B bör attribut B ha ett förslagsfilter tillbaka till attribut A. Detta garanterar dataintegritet och en ren användarupplevelse.

1. Välj alternativ för att definiera förslagsfilter och relationsfilter för attributet på konfigurationspanelen:

   * **Filtertyp**:

      * Ett **Standard** -filter tillämpar ett universellt villkor på attributobjektet. Till exempel plats > Är aktiv = true (endast aktiva platser visas).

        Filtret Standard används alltid, oavsett om andra attribut är markerade eller inte.

      * Ett **attribut**-filter länkar ett attribut till ett annat i kedjan. Exempel: Plats > Referens = Myndighet (endast platser som är knutna till den valda myndigheten visas).

        Attributfiltret används bara om det refererade attributet har ett värde. Om du t.ex. väljer Byrå föreslås bara giltiga platser. Om byrån är tom visas alla platser (men kan ändå begränsas av standardfilter som tillämpas på platsen).

   * **Fält**: Det direkta fältet från attributobjektet, till exempel plats-ID eller aktiv flagga.
   * **Operator**: Dessa alternativ beror på den valda fälttypen. Exemplen innehåller lika med, inte lika med, Är tom, Sant/falskt.
   * (Endast standardfiltertyp) **Value**: Till exempel är Aktiv = Sant.
   * (Endast attributfiltertyp) **Referens**: Det attribut som det här filtret är beroende av, till exempel Agency.
   * (Endast attributfiltertyp) **Referensfält**: Det fält i det refererade attributet som måste matcha, till exempel byråns ID.

1. Klicka på **Spara** för varje attribut för att spara egenskaper och filter.
