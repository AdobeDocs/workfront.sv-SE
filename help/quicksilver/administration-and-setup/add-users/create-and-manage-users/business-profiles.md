---
title: Affärsprofiler - översikt
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: add-users-to-workfront
description: Affärsprofiler är en förbättrad behörighetsmodell som gör det möjligt för kunder som myndigheter att effektivt hantera användaråtkomst och säkerställa exakt kontroll över behörigheter på gruppnivå. I en affärsprofil har användarna distinkta behörigheter för gruppspecifika objekt. Ytterligare objekt kan också delas direkt med affärsprofilen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 7f62de33-e544-4be9-8dcf-03a2e09e8a05
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 2b190de6b6ef9ce53e96475d426a4d39cfbd4df4
workflow-type: tm+mt
source-wordcount: '1443'
ht-degree: 0%

---

# Översikt över affärsprofiler

Affärsprofiler är en förbättrad behörighetsmodell som gör det möjligt för kunder som myndigheter att effektivt hantera användaråtkomst och säkerställa exakt kontroll över behörigheter på gruppnivå. I en affärsprofil har användarna distinkta behörigheter för gruppspecifika objekt. Ytterligare objekt kan också delas direkt med affärsprofilen.

En affärsprofil för en användare liknar den användaren som har en specifik roll i en grupp, t.ex. en styrekonom eller projektledare, och som får de behörigheter som följer med den rollen för den angivna gruppen. Affärsprofilen kan vara tillfällig, så att behörigheterna kan gälla under en tidsperiod som är inställd på att gå ut och så att databegränsningarna för gruppen eller byrån upprätthålls.

Workfront systemadministratör:

* Skapar åtkomstnivåer och definierar begränsade fält efter behov
* Uppdaterar användarprofilen med gruppen och åtkomstnivån för den gruppen (det här är affärsprofilen)
* Definierar giltighetsdatum för affärsprofilen efter behov
* Tilldelar layoutmallar till åtkomstnivåerna

Alla användare som har åtkomst till delade objekt kan dela dem med affärsprofilen, och alla användare med profilen kan se objektet.

## Exempel på affärsprofil

>[!BEGINSHADEBOX]

Sam behöver olika åtkomst till projekt för byrå A och byrå B. Båda byråerna är upplagda i Workfront. (Mer information om grupper finns i Översikt över grupper.)

För byrå A fungerar Sam som styrekonom och behöver tillgång till alla finansiella områden i sina projekt. För byrå B fungerar Sam som projektledare och måste hantera uppgifter och problem, men ska inte kunna se den ekonomiska informationen.

Workfront systemadministratör skapar nya åtkomstnivåer som kallas för styrekonom och projektledare. Dessa åtkomstnivåer har rätt åtkomst för finansiella data. Administratören öppnar sedan Sam användarprofil och väljer&quot;Agency A&quot; som grupp med åtkomstnivån&quot;Financial Controller&quot; för att skapa den första affärsprofilen och&quot;Agency B&quot; som grupp med åtkomstnivån&quot;Project Manager&quot; för att skapa den andra affärsprofilen.

När affärsprofilerna är klara kommer alla projekt för byrå A och byrå B att visas när Sam går till projektlistan (tillsammans med andra projekt som Sam har skapat eller fått tillstånd till). De finansiella fälten i Agency A:s projekt är synliga för Sam både i listvyn och i projektinformationen, men de finansiella fälten i Agency B:s projekt är dolda. Fältnamnen visas men fältdata är tomma.

Om andra användare på någon av byråerna delar projekt med affärsprofilerna&quot;Financial Controller - Agency A&quot; eller&quot;Project Manager - Agency B&quot; är dessa projekt synliga för Sam. De finansiella områdena i byråns projekt förblir alltid dolda eftersom detta definieras i åtkomstnivån.

>[!ENDSHADEBOX]

## Hur affärsprofiler definieras

Adobe Workfront systemadministratör ansvarar för att definiera alla områden i en affärsprofil.

### Skapa åtkomstnivå

Workfront systemadministratör skapar åtkomstnivån med nödvändig åtkomst och definierar eventuella begränsade fält efter behov.

Mer information finns i [Skapa och ändra anpassade åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Lägg till affärsprofil för användare

Workfront systemadministratör lägger till affärsprofilen i en användarprofil genom att välja en grupp och åtkomstnivå. Kombinationen av de två skapar affärsprofilen. Varje grupp kan bara användas i en affärsprofil per användare. <!--how does this combine with more than one access level per group. As far as I can see a business profile is one level and one group-->

Affärsprofilen kan ha mer än en åtkomstnivå per grupp. Nivån med den högsta åtkomstnivån har företräde.

Administratören kan tilldela giltighetsdatum till en affärsprofil, så att användarens åtkomst upphör vid ett framtida datum. Start- och slutdatumen anger när användaren börjar och slutar med profilen i den gruppen. Om du använder giltighetsdatum för att avsluta åtkomsten i stället för att ta bort profilen kan profilen aktiveras igen i framtiden.

Flera affärsprofiler tillåts för en användare.

<!--image?-->

Mer information finns i [Redigera en användares profil](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). <!--may be separate article now since it's not in the profile-->

### Tilldela layoutmallar till åtkomstnivå

Workfront systemadministratör kan också tilldela en layoutmall till åtkomstnivån för att säkerställa att användare med relaterad affärsprofil ser relevant information och åtgärder baserat på deras roll i systemet.

Mer information finns i [Tilldela användare till en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

## Hur affärsprofiler fungerar

När en affärsprofil läggs till för en användare avgör behörigheterna i kombinationen av gruppen och åtkomstnivån vad användaren kommer att se i Workfront.

### Workfront layout

När gruppen i affärsprofilen är kopplad till ett projekt används layoutmallen för åtkomstnivån i affärsprofilen. Alla användare med affärsprofilen ser menyalternativen, hemsidan och andra layoutelement som ingår i mallen. Layoutmallen för affärsprofiler har företräde framför en layoutmall som tilldelats användaren.

Om affärsprofilen har flera åtkomstnivåer med samma grupp kombineras layoutmallarna för båda åtkomstnivåerna. Alla tillgängliga layoutelement visas. Om ett menyalternativ visas i en mall men döljs i en annan, visas det. Endast objekt som är dolda i alla mallar för affärsprofilen är dolda.

I situationer där samma objekt visas i flera layoutmallar men där objektens ordning är olika (t.ex. vänster navigering eller punkter), används ordningen från mallen för åtkomstnivån som listas först i affärsprofilen.

### Projekt och andra delade objekt

När ett projekt är kopplat till en grupp kan en användare med en affärsprofil för den gruppen visa projektet. Synligheten för fält i projektet baseras på åtkomstnivån i affärsprofilen. Om gruppen tilldelas flera åtkomstnivåer i användarens affärsprofil gäller nivån med de högsta behörigheterna.

En användare har till exempel två affärsprofiler: den första ger styrekonomer åtkomst till en grupp (för att se finansfält) och den andra ger projektledaren åtkomst till en annan grupp (där finansfält inte ska visas).

Användaren skulle se projekt för båda grupperna i listan över alla projekt. I både listvyn och projektinformationen skulle användaren bara se ekonomiska data för den första gruppen. Finansieringsområdena för den andra gruppens projekt skulle vara tomma.

Alla användare som har tillgång till delade objekt kan dela dessa objekt med en affärsprofil. Alla användare som är tilldelade profilen får de angivna behörigheterna till objektet. Om åtkomsten är begränsad i den åtkomstnivå som tilldelats av administratören i affärsprofilen, har åtkomstnivån företräde framför behörigheter som ges vid delning. Om åtkomstnivån till exempel inte tillåter att uppgifter skapas, kan användaren inte lägga till uppgifter i ett projekt, även om de får behörigheten Hantera för ett projekt när det delas med affärsprofilen.

Om en användare tilldelas en affärsprofil efter att ett objekt redan har delats med profilen, kommer användaren att se objektet med den angivna åtkomsten.

När en affärsprofil har flera åtkomstnivåer har nivån med den högsta åtkomstnivån företräde.

Mer information om delning finns i [Dela ett objekt](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Mer information om hur åtkomstnivåer och behörigheter fungerar tillsammans finns i [Översikt över åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

## Att tänka på när det gäller affärsprofiler

* En användare behöver inte vara medlem i en grupp för att kunna tilldelas en affärsprofil för den gruppen.
* Åtkomstnivån i affärsprofilen kan bara uppgradera en användares grundläggande åtkomstnivå. Affärsprofilen kan inte ta bort de grundläggande åtkomstnivåbehörigheterna.
* I objektlistor och rapporter har användaren alla behörigheter som är tillgängliga för dem från alla deras tilldelade affärsprofiler i de grupper som sammanfogats med deras basåtkomstnivå. På andra sidor har användaren de grundläggande åtkomstnivåbehörigheterna.
* När en grupp tas bort från Workfront tas alla tilldelade affärsprofiler för den gruppen bort från de associerade användarna.
* Om en åtkomstnivå ingår i en företagsprofil och du tar bort åtkomstnivån uppmanas du att välja en ny åtkomstnivå att använda i stället.
* Uppdateringar av affärsprofiler spåras i Workfront granskningsloggar. Mer information finns i Översikt över granskningsloggar.
