---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Systemuppgiftsstatus
description: De tre inbyggda aktivitetsstatusarna i Workfront krävs, vilket innebär att du kan låsa upp, byta namn på och ordna om dem, men du kan inte dölja eller ta bort dem. Du kan också lägga till nya aktivitetsstatusar för systemet för att passa behoven i din organisation. Att ändra status för en uppgift är vanligtvis en manuell process, men ibland ändras status för en uppgift automatiskt beroende på andra faktorer som inträffar i systemet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Systemuppgiftsstatus

De tre inbyggda aktivitetsstatusarna i Workfront krävs, vilket innebär att du kan låsa upp, byta namn på och ordna om dem, men du kan inte dölja eller ta bort dem.

Du kan också lägga till nya aktivitetsstatusar för systemet för att passa behoven i din organisation.

Att ändra status för en uppgift är vanligtvis en manuell process. Det finns emellertid tidpunkter som beskrivs i följande lista när en uppgifts status ändras automatiskt, beroende på andra faktorer som inträffar i systemet.

Följande uppgiftsstatusvärden finns i din Workfront-instans:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Systemaktivitetsstatus</th> 
   <th>När den här statusen inträffar</th> 
   <th>Åtgärder som inträffar när en aktivitet har den här statusen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Ny (obligatorisk status)</td> 
   <td>Det här är standardstatus för alla nya uppgifter som skapas.</td> 
   <td>Om aktiviteten finns i ett projekt med statusen Aktuell, visas uppgiften på fliken Arbetsbegäran för de användare som är tilldelade till uppgifterna. Användarna kan nu börja arbeta med uppgiften.</td> 
  </tr> 
  <tr> 
   <td>Pågår (obligatorisk status)</td> 
   <td>Du kan placera en uppgift i den här statusen för att ange att arbetet med den uppgiften har startat.</td> 
   <td> <p>När du markerar en uppgift som Pågår visas ett värde för Faktiskt startdatum.</p> <p>Förloppet för aktiviteten registreras inte förrän du manuellt uppdaterar procentandelen färdigt för uppgiften.</p> </td> 
  </tr> 
  <tr> 
   <td>Slutförd (obligatorisk status)</td> 
   <td> <p>Du kan markera en uppgift som slutförs manuellt när arbetet är slutfört.</p> <p>När spårningsläget för en uppgift är inställt på Komplettera automatiskt markeras aktiviteten automatiskt som Slutförd när det planerade slutförandedatumet uppnås.</p> </td> 
   <td> <p>När en uppgift är slutförd markeras procentandelen slutförd för uppgiften som 100 %. Uppgiften tas bort från den tilldelades arbetslista i hemområdet när den är slutförd.</p> <p>När du markerar en uppgift som slutförd visas ett värde för Faktiskt slutförandedatum.</p> <p><b>Obs!</b> Om aktiviteten har ofullständiga problem och du ändrar aktivitetsstatus till Fullständig, ändras statusen automatiskt till Fullständigt - väntande problem.</p> </td> 
  </tr> 
 </tbody> 
</table>
