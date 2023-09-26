---
title: Skapa arbetsytor
description: En arbetsyta är en samling driftsposttyper och taxonomier som används av ett team och som representerar teamets arbetslivscykel. Du kan anpassa arbetsytorna helt i Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Skapa arbetsytor

>[!IMPORTANT]
>
>För närvarande ingår Adobe Maestro i ett betaprogram som är öppet för ett begränsat antal kunder.
>
>Kontakta din kontorepresentant om du vill ha mer information om hur du går med i betaprogrammet för Maestro.
>
>Mer information finns i [Adobe Maestro - översikt](../maestro-overview.md).

I Adobe Maestro är arbetsytorna centraliserade platser där team kan planera sitt arbete.

En arbetsyta är en samling driftsposttyper och taxonomier som används av ett team och som representerar teamets arbetslivscykel. Du kan anpassa arbetsytorna helt i Maestro.

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
   <td> <p>Systemadministratören måste lägga till Maestro-området i layoutmallen. Mer information finns i <a href="../access/grant-access.md">Ge åtkomst till Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Att tänka på när det gäller arbetsytor

* Du kan skapa arbetsytor för specifika organisationsenheter inom organisationen, så att de matchar det unika sätt som varje enhet fungerar på.
* De posttyper och taxonomier som en arbetsyta innehåller bör återspegla arbetslivscykeln för en organisationsenhet.
* När du skapar en arbetsyta kan alla i organisationen visa, redigera eller ta bort den.  <!--this will change with access levels and permissions-->
* Du kan ha högst 1 000 arbetsytor i din organisation.
* Arbetsytor innehåller posttyper som är unika för varje arbetsyta. <!--this might change-->

## Skapa en arbetsyta

1. (Villkorligt) Om du inte har några arbetsytor klickar du på **Huvudmeny** icon ![](assets/main-menu-workfront.png) i Workfront övre högra hörn, <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> klicka sedan på **Maestro** ![](assets/maestro-icon.png).

   Du kan också klicka på nedåtpilen till höger om arbetsytans namn från en befintlig arbetsyta och sedan klicka på **Skapa arbetsyta**.

   ![](assets/workspace-drop-down-right-menu.png)

   Nu öppnas arbetsytan i Maestro.
1. (Valfritt och villkorligt) Klicka på **Förhandsgranska** i någon av följande fördefinierade arbetsytemallar:

   * Marknadsföringshantering
   * Försäljningshantering
   * Produkthantering

   Det finns en indikation på vilka operativa posttyper, taxonomier och hur många fält som är associerade med varje mall.

   ![](assets/previewing-a-workspace-template.png)

   Mer information om mallar för arbetsytan i Maestro finns i [Lista över arbetsytemallar](../architecture-and-fields/workspace-templates.md).

1. Klicka **Använd mall** för att börja skapa arbetsytan från den valda mallen

   eller

   Klicka **Skapa arbetsyta** för att skapa en arbetsyta från grunden.

   En av följande typer av arbetsytor skapas:

   * En tom arbetsyta där du kan börja lägga till posttyper manuellt.
   * En arbetsyta med exempelposttyper som du kan anpassa ytterligare.

1. Klicka inuti arbetsytans namn i arbetsytans sidhuvud för den nya arbetsytan och tryck sedan på Retur

   eller

   Klicka på **Mer** meny ![](assets/more-menu.png)till höger om arbetsytans namn i sidhuvudet och klicka sedan på **Byt namn**.

1. (Valfritt) Klicka på **Lägg till posttyp** om du vill lägga till posttyper på arbetsytan.

   Mer information finns i [Skapa posttyper](../architecture-and-fields/create-record-types.md).

1. (Valfritt) Klicka på **Lägg till taxonomi** för att lägga till taxonomier på arbetsytan.

   Mer information finns i [Skapa taxonomier](../architecture-and-fields/create-a-taxonomy.md).