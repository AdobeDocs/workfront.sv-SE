---
content-type: reference
product-area: documents
navigation-topic: workfront-dam-within-workfront
title: Adobe Workfront rolltyper för licensiering kontra rolltyper för Adobe Workfront DAM
description: Adobe Workfront-administratörer använder åtkomstnivåer för att avgöra vad användare kan göra i ett program.
author: Courtney
feature: Digital Content and Documents
exl-id: dcca0158-dc31-4aba-bd87-90ccc64e77cb
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Adobe Workfront rolltyper för licensiering kontra rolltyper för Adobe Workfront DAM

Adobe Workfront-administratörer använder åtkomstnivåer för att avgöra vad användare kan göra i ett program.

* I Workfront avgör licensieringen en användares åtkomstnivå.
* I Workfront DAM definierar rolltyper användarnas åtkomst till resurser i DAM.

Eftersom licenstyper och rolltyper inte är utbytbara innebär en åtkomstnivå i ett program inte åtkomst i det andra programmet. En användare med en Work-licens i Workfront tilldelas till exempel inte automatiskt en Contributor-roll i Workfront DAM.

## Workfront-licenstyper

Som Workfront-administratör definierar du åtkomstnivån som användare har genom att tilldela licenstyper. Varje licens har en uppsättning standardåtkomstfunktioner som du kan ändra innan du tilldelar licensen till användaren. 

Ni använder licenser för att avgöra vad en användare kan se och göra i Workfront. Det finns fem licensieringstyper i Workfront:

* Plan
* Arbete
* Granska
* Begäran
* Extern

Se [Översikt över äldre licenser](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md) om du vill ha en beskrivning av de olika licenstyperna i Workfront.

## Rolltyper för Workfront DAM

Som Workfront DAM Workfront-administratör tilldelar du rolltyper till användare för att definiera åtkomsten de har till resurser. Dessutom anger rolltyperna de områden i DAM där användarna kan arbeta.

Rolltyper fungerar tillsammans med grupper när användaråtkomsträttigheter fastställs. Grupper styr åtkomsten som användare har till mappar och till själva resurserna. Rolltyper avgör vilka åtgärder användare kan utföra med resurser. Alla DAM-användare måste vara associerade med minst en grupp. Mer information om rolltyper och åtkomstkonfiguration finns i hjälpen i Workfront DAM.

Det finns fyra olika rolltyper i Workfront DAM:

### Brand Portal

Användare med den här rolltypen har endast åtkomst till Brand Connect-portalen i DAM. På portalen kan användare visa och hämta resurser som de har behörighet till.

Brand Portal-användare kan samarbeta med andra genom att skapa och dela ljusbord.

### Vanlig användare

Användare med den här rolltypen kan visa och hämta resurser från Workfront DAM och Brand Connect-portalen.

Vanliga användare kan också samarbeta med andra genom att skapa och dela ljusbord.

### Medarbetare

Användare med den här rolltypen har tillgång till Workfront DAM och Brand Connect-portalen.

Medarbetare kan visa, hämta, överföra, redigera, flytta och ta bort resurser och mappar som de har åtkomst till. Medarbetare kan dessutom samarbeta med andra genom att skapa och dela ljusbord. 

### Administratör

Workfront-administratörer har tillgång till allt i Brand Connect-portalen och Workfront DAM, inklusive material som har upphört att gälla eller som har inaktiv status.

För att få administratörsåtkomst måste användare med rolltypen Administratör finnas i gruppen Administratörer.
