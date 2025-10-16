---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Återställ borttagna objekt
description: Om du är Workfront-administratör kan du återställa projekt, uppgifter, utgåvor, dokument och mallar i Adobe Workfront om de har tagits bort de senaste 30 dagarna. Efter 30 dagar tas dessa objekt bort permanent och kan inte återställas.
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 0%

---

# Återställ borttagna objekt

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Om du är Workfront-administratör kan du återställa projekt, uppgifter, utgåvor, dokument och mallar i Adobe Workfront om de har tagits bort de senaste 30 dagarna. Efter 30 dagar tas dessa objekt bort permanent och kan inte återställas.

När du återställer ett objekt återställs även alla dess underordnade objekt och fält. Om du till exempel återställer ett projekt återställs även alla uppgifter, ärenden, dokument, timmar, anteckningar, tilldelningar och anpassade data i projektet.

En gruppadministratör kan också återställa dessa objekt för en grupp som de hanterar.

>[!IMPORTANT]
>
>* Om du tar bort en rapport, instrumentpanel, användare, grupp, team eller upprepning kan den inte återställas.
>* Om någon annan än gruppadministratören i en grupp överför ett dokument direkt till dokumentområdet för ett objekt, kan bara en Workfront-administratör återställa dokumentet.
>
>* Om du flyttar en uppgift eller ett problem och väljer att inte flytta dokumenten som är bifogade till uppgiften eller problemet, tas dokumenten bort och placeras i papperskorgen i 30 dagar. En administratör kan återställa dem och de kopplas till den flyttade aktiviteten eller problemet. Om uppgiften eller problemet har tagits bort sedan den flyttades, återställs dokumenten i området Dokument på administratörens användarsida, som återställer dem.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Systemadministratör</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Information som återställs när du återställer ett projekt, en uppgift eller ett ärende

När du återställer ett projekt, en uppgift eller ett problem återställs följande associerade information tillsammans med projektet:

* Kommentarer och svar i uppdateringsområdet
* Godkännanden
* Uppdrag
* Anpassad Forms
* Köinställningar
* Affärsfall, inklusive styrkort, mål och risker
* Projektgrupper
* Datum
* Problem
* Uppgifter
* Underaktiviteter
* Status
* Ekonomisk information:

   * Faktureringsposter
   * Faktureringstariffer
   * Utgifter

* Information om tidslinjen:

   * Föregående
   * Aktivitetsbegränsningar
   * Typ av varaktighet

* Baslinjer

  Uppgiftsbaslinjer återställs när du återställer det överordnade projektet eller den överordnade aktiviteten, men inte när du återställer enskilda borttagna uppgifter.

* Timmar (och tim-ID)

  Om timmar återställs till det borttagna objektet beror på vilka inställningar du har valt när du konfigurerar inställningar för tidrapporter och timmar. Mer information finns i [Konfigurera påverkan på timmar när ett objekt tas bort och återställs](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* Objektets URL

  När det återställs ändras inte objektets URL. Om någon har skapat webbläsarbokmärken för objektet är de fortfarande giltiga.

* Åtkomst och behörigheter

  Användare som hade åtkomst till objektet innan det togs bort återfår åtkomsten efter att det återställts.

* Dokument (inklusive korrekturdokument)

  Tänk på följande när du återställer dokument och dokumentversioner:

   * Dokument som har tagits bort individuellt kan återställas individuellt.

     Dokument som har tagits bort tillsammans med deras överordnade projekt, uppgift eller utgåva återställs när du återställer det överordnade projektet, men du kan inte återställa dem individuellt.

   * Alla versioner av ett dokument eller ett dokumentkorrektur återställs när dokumentet återställs.\
     Det går inte att återskapa enskilda versioner av ett dokument eller dokumentkorrektur som tagits bort individuellt.

## Information som inte återställs när du återställer ett projekt, en uppgift eller ett problem

När du återställer ett projekt, en uppgift eller ett problem återställs inte följande associerade information tillsammans med projektet:

* Liknar
* Slutsatser
* Ange e-postadress i en begärandekö
* Favoriter

  Ett projekt, en uppgift eller ett problem som du lade till på Favoriter-menyn innan du tog bort det visas inte igen på Favoriter-menyn när du har återställt det.

* Lösa objekt

  Ett matchande objekt är ett konverterat fel som har konfigurerats med alternativet **Behåll det ursprungliga felet och koppla dess upplösning till det här** &lt;**(projekt** eller **aktivitet)**>. Om du tar bort det överordnade projektet eller den överordnade aktiviteten identifieras problemet inte längre som ett matchande objekt eftersom det inte längre finns någon länk som ansluter det till projektet eller aktiviteten. Om du återställer den överordnade länken återställs inte länken.

  Mer information om hur en Workfront-administratör eller gruppadministratör konfigurerar problem så att de matchar matchande objekt när de konverteras finns i [Konfigurera inställningar för systemomfattande åtgärder och problem](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) och [Konfigurera inställningar för aktiviteter och problem för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

  Mer information om hur du konverterar problem finns i [Översikt över hur du konverterar problem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Återställ objekt

{{step-1-to-setup}}

1. Klicka på **Papperskorgen** > **Nyligen borttagen**.
1. Klicka på fliken **Projekt**, **Åtgärder**, **Problem**, **Mallar** eller **Dokument**, beroende på vilken typ av objekt du vill återställa.

   Objekten sorteras som standard i kolumnen **Borttagningsdatum** .

1. Välj upp till 10 objekt som du vill återställa.

   Om du tar bort en underordnad uppgift visas den i listan.

   Om du tar bort en överordnad uppgift visas endast den överordnade uppgiften i listan. Alla underordnade uppgifter återställs dock när du återställer en överordnad uppgift.

1. Klicka på **Återställ** om du vill återställa de markerade objekten till deras ursprungliga plats.
1. (Valfritt) Om du snabbt vill visa det återställda objektet följer du stegen i [Visa återställt objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   Mer information om vad som händer efter att du har återställt ett objekt finns i avsnittet [Vad som händer efter att du har återställt objekt](#what-happens-after-you-restore-items) i den här artikeln.

## Vad som händer när du återställer objekt {#what-happens-after-you-restore-items}

* När du återställer uppgifter och underaktiviteter visas de i den ordning de hade innan de togs bort.

  Om ordningen för andra uppgifter ändras medan uppgiften tas bort, kan uppgiften återställas till slutet av listan med uppgifter eller underaktiviteter.

* När du har återställt ett objekt:

   * Ett meddelande visas som talar om för dig om du lyckades.

     Du får även ett e-postmeddelande. Om du har återställt flera objekt visas de i e-postmeddelandet.

   * En kommentar visas i uppdateringsområdet för projektet, aktiviteten eller utgåvan och i det överordnade objektet.

     Detta händer inte när du återställer ett dokument eller en mall.

## Återställda korrektur

När någon återställer ett dokument som har ett korrektur kan sidan Korrekturaktiviteter för korrekturet visa namnet på den första aktiva Workfront-administratören som anges för din organisations instans (i den ordning som profil-ID:t används) i stället för den faktiska personen som återställde korrekturet.
