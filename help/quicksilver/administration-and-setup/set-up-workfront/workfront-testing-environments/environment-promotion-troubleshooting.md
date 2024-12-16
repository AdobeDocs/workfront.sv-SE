---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Felsökning av miljökampanjer
description: Felsök vanliga problem med vår miljömarknadsföring.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 830dd573-d954-4ba2-a1d3-d1645b3fbac8
source-git-commit: c3c9a423bd60b26b2605a1b52bd706c9bc6acdec
workflow-type: tm+mt
source-wordcount: '328'
ht-degree: 0%

---

# Felsökning av miljökampanjer

I den här artikeln beskrivs hur du felsöker miljökampanjer.

## Problem: Paketet för miljöbefordran försätts eller misslyckas

Om ditt miljöerbjudande inte fungerar eller inte fungerar kan du försöka med följande:

* Om en paketinstallation avbryts efter 10-15 minuter, eller om en paketinstallation misslyckas, sätter du ihop det befintliga paketet eller skapar ett nytt paket.

* Om en paketinstallation misslyckas kan det uppstå ett problem med ett eller flera objekt. Kontrollera felmeddelandena, som identifierar objektet och kan hjälpa till att identifiera problemet. När du har åtgärdat problemet med objektet sätter du ihop paketet igen och försöker installera igen.

* Om du fortfarande har problem med en installation kan du försöka replikera installationen i en annan målmiljö. Håll dig så nära den ursprungliga installationen som möjligt, inklusive valda objekt och installationsåtgärder.

* Vi rekommenderar att du alltid kontrollerar paketinnehållet när paketet har monterats för att bekräfta att det innehåller de objekt du förväntar dig.


## Problem: Det går inte att befordra anpassade formulär

Detta kan bero på att det anpassade formuläret innehåller ett beräkningsfält. Om ett beräkningsfält refererar till ett fält som inte refereras i ett anpassat formulär, befordras inte ett paket som innehåller det här formuläret och användaren kan se följande meddelande:

&quot;Följande fält är ogiltiga: Ogiltigt anpassat uttryck Ogiltigt uttryck: Ogiltigt anpassat uttryck.&quot;

Problemet kan uppstå när man refererar till ett befintligt fält som inte är kopplat till några anpassade formulär i målmiljön eller med ett nytt fält.

Gör något av följande för att lösa problemet:

* Skapa ett paket med ett anpassat formulär av projekttyp som innehåller det refererade fältet. När du har befordrat det här paketet till målmiljön ska du befordra det ursprungliga paketet som innehåller beräkningsfältet.
* Skapa det refererade fältet manuellt i målmiljön och associera det med ett anpassat formulär av projekttyp. När detta är gjort identifieras fältet och du kan befordra paketet utan att stöta på felet.
