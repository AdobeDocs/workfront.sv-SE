---
title: Redigera poster
description: Du kan redigera postinformation i Adobe Maestro. Du måste skapa posttyper innan du kan börja skapa och redigera poster.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Redigera poster

>[!IMPORTANT]
>
>Informationen i den här artikeln handlar om Adobe Maestro, ett nytt erbjudande från Adobe Workfront.
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder. Du måste vara Workfront-kund för att kunna använda Maestro-funktionerna.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

Du kan redigera postinformation i Adobe Maestro. Du måste skapa posttyper innan du kan börja skapa och redigera poster.
Mer information finns i [Skapa posttyper](../architecture/create-record-types.md).

&lt;!— här anger du att fälten i detaljvyn är desamma som fälten i tabellvyn - den här artikeln är länkad från vyerna Hantera post för att referera till den här informationen—>

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-avtal</p></td>
   <td>
<p>Din organisation måste vara registrerad i det betaprogram som Adobe Maestro stängt. Kontakta din kontorepresentant om du vill veta mer om det nya erbjudandet. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront</p></td>
   <td>
<p>Alla</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-licens</p></td>
   <td>
   <p>Alla</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Åtkomstnivå</td>
   <td> <p>Alla</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layoutmall</td>
   <td> <p>Systemadministratören måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/access-overview.md">Åtkomstöversikt</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permssions - replace the table with: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


## Att tänka på när du redigerar poster

* Du kan redigera poster som du eller någon annan användare har skapat. <!--will change with access levels-->
* Du kan inte redigera fält som är länkade från andra poster eller fält som innehåller beräkningar.
* Om de poster som du visar är länkade till andra poster, återspeglas den nya informationen om de poster som du redigerar på de länkade posterna.
* Du kan inte redigera flera poster samtidigt. <!--this will probably change-->
* URL-adresser känns bara igen som länkar i enradiga textfält när de börjar med följande: http://, https://, ftp:// eller www. .
* Du kan använda följande formateringsalternativ för RTF när du redigerar ett stycketextfält:

   * Fet
   * Kursiv
   * Understruken
   * Lägg till en länk
   * Lägga till en punktlista
   * Lägga till en numrerad lista

## Redigera poster

Du kan redigera en post i följande områden:

* [Från detaljsidan för en post](#edit-a-record-from-the-records-details-page)
* [Från tabellvyn för en posttyp](#edit-a-record-from-the-record-type-table-view)

### Redigera en post från postens informationssida

{{step1-to-maestro}}

Arbetsytan som du öppnar senast öppnas.

1. (Valfritt) Klicka på nedåtpilen till höger om arbetsytans namn för att markera arbetsytan vars poster du vill uppdatera.
1. Gör något av följande:

   * Klicka på en posts namn i en tabellvy.
   * Håll markören över namnet på en post i tabellvyn och klicka sedan på **Mer** meny ![](assets/more-menu.png)och sedan klicka **Visa**

     ![](assets/contextual-menu-for-record-row.png)
   * Klicka på ett postfält i en tidslinjevy.

   Posten **Information** sidan öppnas.

1. Klicka på **Mer** meny ![](assets/more-menu.png) till höger om postnamnet och klicka sedan på **Redigera**

   eller

   Klicka i ett redigerbart fält på detaljsidan för att redigera informationen.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Klicka **Spara ändringar**. <!--logged a bug for this - this needs to be "Save"-->

### Redigera en post från tabellvyn för en posttyp

{#step1-to-maestro}

Arbetsytan som du senast öppnade öppnas.

1. (Valfritt) Klicka på nedåtpilen till höger om arbetsytans namn för att markera arbetsytan vars poster du vill uppdatera.
1. Klicka på ett posttypskort.

   Posttypssidan öppnas.
1. (Villkorligt) Från **Visa** i den nedrullningsbara menyn i tabellens övre högra hörn väljer du en **Tabell** vy. Detta bör vara standardvyn, såvida du inte har visat posttypen i tidslinjevyn när du senast öppnade den.

   Posterna som är associerade med den valda posttypen visas i tabellvyn.
1. Klicka inuti en post för att börja redigera information om den infogade posten.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. Tryck **Retur** på tangentbordet eller klicka utanför en rad för att spara ändringarna. Ändringarna sparas automatiskt. En sparad indikator visas kort i tabellvyns övre högra hörn för att visa att ändringarna sparades.

   >[!NOTE]
   >
   >  Du kan inte redigera information för följande fält eftersom de är skrivskyddade och Workfront uppdaterar dem automatiskt:
   >  
   >  * Länkade fält som skapas genom att koppla posttyper. Mer information finns i [Koppla posttyper](../architecture/connect-record-types.md).
   >  * Fält av följande typer: Skapad av, Skapad, Senast ändrad av, Senast ändrad


1. (Valfritt) Kopiera ett eller flera befintliga värden för ett fält, klistra in dem i ett fält av samma typ på en annan post och klicka sedan på **Retur** på tangentbordet för att spara ändringarna.

   >[!NOTE]
   >
   >Tänk på följande:
   >
   >* Du kan inte kopiera information från en annan källa, förutom ett Maestro-fält av samma typ som det fält som du klistrar in informationen i.
   >
   >* Du kan inte kopiera och klistra in fältvärden i området Detaljer för en post. Den här funktionen stöds bara i tabellvyn för en posttyp.
   >* Du kan inte kopiera och klistra in fältvärden för följande fälttyper:
   >
   >
   >    * Länkade fält som skapas genom att koppla posttyper. Du kan kopiera och klistra in länkade postfält. Mer information finns i [Koppla posttyper](../architecture/connect-record-types.md).
   >    * Fält av följande typer: Skapad av, Skapad, Senast ändrad av, Senast ändrad

<!--1. (Optional) Use the following keyboard shortcuts to undo or redo editing or copying and pasting record information: 

    * **Undo**: CTRL/CMD + Z
    * **Redo**: CTRL/CMD + Shift + Z-->