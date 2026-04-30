---
product-area: documents
navigation-topic: manage-documents
title: Kontrollera dokumentlagringsgränser
description: Som Adobe Workfront-administratör kan du visa dokumentlagringsanvändning och -kvot på sidan Kundinformation. Hur lagringsutrymmet ser ut beror på om din organisation använder äldre Workfront-lagring eller Adobe Enterprise-lagring.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: e25be455e16beee813e612b983bca1302f129e6f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Kontrollera dokumentlagringsgränser

{{highlighted-preview}}

Även om det inte finns några begränsningar för vilka typer och storlekar enskilda filer som användare kan överföra till din Workfront-instans, innehåller din Workfront-plan en total lagringskvot. Som Workfront-administratör övervakar du användningen och kvoten i området Inställningar på sidan Kundinformation.

Hur lagringsutrymmet ser ut beror på om din organisation använder äldre Workfront-lagring eller Adobe Enterprise-lagring:

* Om du använder äldre Workfront-lagring läser du [Äldre Workfront-lagring](#legacy-workfront-storage) i den här artikeln.
* Om du använder Adobe Enterprise-lagring läser du [Adobe Enterprise-lagring](#adobe-enterprise-storage) i den här artikeln.

  Mer information om Enterprise-lagring finns i [Översikt över Adobe Enterprise-lagring](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Workfront</td> 
   <td> <p>Alla Workfront-paket som hanterar dokument med äldre lagringsutrymme</p>
      <p>Alla arbetsflödespaket för att hantera dokument med Adobe Enterprise-lagring</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Äldre Workfront-lagring

Om din organisation använder äldre Workfront-lagring visas en lagringskvot på kundinformationssidan för dokument som överförs direkt till Workfront.

Så här kontrollerar du äldre dokumentlagring i Workfront:

{{step-1-to-setup}}

1. Klicka på **System** > **Kundinformation** i den vänstra panelen.
1. Gå till **Lagringskvot** i avsnittet **Grundläggande information**. Här kan du se hur mycket lagringsutrymme du använder just nu samt hur mycket lagringsutrymme din Workfront-plan omfattar.

Lagringskvoten uppdateras dagligen för att visa det senaste antalet.

>[!NOTE]
>
>Denna gräns gäller inte dokument som du länkar till Workfront från någon annan tredjepartsleverantör av tjänster (SharePoint, Google Drive, Webdam, Box, Dropbox eller någon annan leverantör av dokumenthantering).

<div class="preview">

## Adobe Enterprise-lagring

Om din organisation använder Adobe Enterprise-lagring visar kundinformationen en översikt över lagringsutrymmet som bryter användningen i olika avsnitt för äldre Workfront-lagring, Adobe Enterprise-lagring och Frame.io. Workfront lägger också på ett valfritt tak för överföringar när användningen överskrider din kvot, så att användare fortfarande kan överföra dokument.

### Visa lagringsanvändning i kundinformation

Så här kontrollerar du dokumentlagring i Adobe Enterprise:

{{step-1-to-setup}}

1. Klicka på **System** > **Kundinformation** i den vänstra panelen.
1. Gå till avsnittet **Lagringsöversikt**.
1. Visa hur Adobe Enterprise-lagring används.
   <!--Both Workfront and Frame.io usage are broken down separately, but roll up to the total usage for Adobe enterprise storage.-->

![Adobe användning av företagslagring i kundinformation](assets/storage-usage.png)

Användningssiffrorna uppdateras regelbundet så att du ser ett aktuellt antal.

### E-postmeddelanden för administratörer

När användningen överskrider 75 %, 85 % eller 100 % av din lagringskvot skickar Workfront ett e-postmeddelande till systemadministratörerna.

</div>