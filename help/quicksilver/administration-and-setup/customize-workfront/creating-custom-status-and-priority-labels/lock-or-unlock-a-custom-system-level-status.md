---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Låsta och olåsta statusvärden på systemnivå
description: Genom att låsa anpassade statusvärden kan du se till att alla i organisationen använder samma processer i sitt arbetsflöde. När en status är låst är den tillgänglig för alla användare i systemet. Även om du kan redigera eller ta bort den kan gruppadministratörer inte göra det för sina grupper. Omvänt gör det möjligt för gruppadministratörer att hantera de unika arbetsflöden som används i deras grupper mer flexibelt om man låser upp anpassade statusar. De kan ändra attributen för en olåst status eller ta bort den för sina grupper.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: c70a10a920d32ad00a2e833b331c92a598902d21
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Låsta och olåsta statusvärden på systemnivå

Genom att låsa anpassade statusvärden kan du se till att alla i organisationen använder samma processer i sitt arbetsflöde. När en status är låst är den tillgänglig för alla användare i systemet. Även om du kan redigera eller ta bort en status som du låser kan gruppadministratörer inte göra det för sina grupper. De kan bara ändra visningsordningen i statuslistan.

Omvänt gör det möjligt för gruppadministratörer att hantera de unika arbetsflöden som används i deras grupper mer flexibelt om man låser upp anpassade statusar. När en status är olåst kan gruppadministratörer ändra dess attribut eller ta bort den för sina grupper.

>[!IMPORTANT]
>
>Om du låser en anpassad status efter att den har låsts upp under en tidsperiod, ersätter dina systemomfattande statusinställningar de som gjorts av gruppadministratörer. När statusen är låst kan gruppadministratörer inte ändra eller ta bort statusen för sina grupper.

Instruktioner om hur du låser eller låser upp en systemnivåstatus finns i [Skapa eller redigera en status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Olåsta statusvärden i godkännandeprocesser

Du kan använda både låsta och olåsta lägen i en systemgodkännandeprocess. Om du skapar en systemgodkännandeprocess med en olåst systemstatus kan användare i hela systemet bifoga godkännandeprocessen till alla projekt, aktiviteter eller utgåvor i systemet.

Varningsmeddelanden visas i följande scenarier för att hjälpa dig och dina användare att förstå resultaten av följande scenarier:

* En administratör låser upp en systemnivåstatus som används i en godkännandeprocess. Ett meddelande varnar som kan ta bort den olåsta statusen för sina grupper, vilket skulle förhindra gruppmedlemmar från att använda godkännandeprocessen korrekt för objekt som tilldelats deras grupp.

* En användare börjar redigera en godkännandeprocess som använder en olåst status. Ett meddelande varnar användaren om olåst status så att de kan utvärdera om det skulle vara en bra idé att låsa om eller ersätta den.

* En godkännandeprocess på systemnivå med olåst status bifogas till ett objekt och statusen togs bort för gruppen som tilldelats till objektet. När en gruppmedlem går till avsnittet Godkännanden för objektet, visas ett meddelande om att godkännandeprocessen inte kan initieras för objektet.

Du kan använda både låsta och olåsta lägen i en gruppgodkännandeprocess. Om du skapar en process för gruppgodkännande med olåst gruppstatus kan användarna bifoga godkännandeprocessen till alla projekt, aktiviteter eller utgåvor som är kopplade till gruppen.