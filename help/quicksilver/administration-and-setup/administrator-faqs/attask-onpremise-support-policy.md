---
title: OnTask OnPremise - supportpolicy
user-type: administrator
content-type: faq
product-area: system-administration
navigation-topic: administrator-faqs
description: Adobe Workfront flyttade till en 100 % Software-As-A-Service-modell och slutade sälja program på plats den 31 december 2011. Från och med 2014 stöds inte längre AtTask OnPremise, med undantag för licensnyckelrelaterade problem. Det lokala programmet är inte längre tillgängligt för hämtning eller installation.
feature: System Setup and Administration
role: Admin
exl-id: 37c65360-6587-43b3-8eaf-4f1a9b375c1d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# OnTask OnPremise - supportpolicy

Adobe Workfront flyttade till en 100 % Software-As-A-Service-modell och slutade sälja program på plats den 31 december 2011. Från och med 2014 stöds inte längre AtTask OnPremise, med undantag för licensnyckelrelaterade problem. Det lokala programmet är inte längre tillgängligt för hämtning eller installation.

Om du redan har programmet och behöver installera om OnPremise hämtar du installationsguiden.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">OnPremise optimization tips can be found.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more about reporting in AtTask OnPremise, click.</p>
-->

Hämta instruktioner om SSL-/TSL-konfiguration.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör. Mer information finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Uppdatera OnPremise-licensnyckeln

Om du behöver en ny licensnyckel ringer du Workfront kundsupport på 844-306-HELP(4357).

När du har fått en ny licensnyckel,

1. Stoppa atTask-servern.
1. Byt namn på filen license.key (finns i mappen AtTaskDoc).
1. Kopiera den nya filen license.key till rätt plats.
1. Starta om aktivitetsservern.

Den här artikeln innehåller följande bilagor:
