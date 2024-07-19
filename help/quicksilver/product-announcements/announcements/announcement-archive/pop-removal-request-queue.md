---
content-type: reference
navigation-topic: announcements
title: Nytt Adobe Workfront-hanterat system som ersätter POP-e-post för begärandeköer med 21.1
description: Vi ersätter POP-e-postalternativet för begärandeköer med ett nytt system som hanteras av Adobe Workfront. Du kan fortfarande skicka begäranden via e-post, men du måste konfigurera en ny e-postadress som hanteras av Workfront i området Begärandekö i stället.
author: Luke
feature: Product Announcements
exl-id: d7147641-ba36-422b-a9b2-3c2f4ab609d8
source-git-commit: f05b462ff596ccc19215ca684802a9820a98211a
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Nytt Adobe Workfront-hanterat system som ersätter POP-e-post för begärandeköer med 21.1

Vi ersätter POP-e-postalternativet för begärandeköer med ett nytt system som hanteras av Adobe Workfront. Du kan fortfarande skicka begäranden via e-post, men du måste konfigurera en ny e-postadress som hanteras av Workfront i området Begärandekö i stället.

## Varför tar du bort POP-e-postalternativet?

POP-tekniken är ett otillförlitligt och mindre säkert e-postalternativ. Dessutom ser vi många kundproblem som är specifika för POP-e-post. Om du byter till ett system som hanteras av Workfront blir upplevelsen mer tillförlitlig.

## Vilken åtgärd behöver jag vidta?

Du måste skapa en ny e-postadress för varje begärandekö som du har konfigurerat med POP-e-post i produktionsmiljön och distribuera den nya e-postadressen efter behov. Mer information finns i [Gör det möjligt för användare att skicka ett problem via e-post till ett begärandeköprojekt](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

## Vad är övergångsplanen?

Från och med version 21.1 i början av februari har du 60 dagar på dig att övergå till den nya e-postadressen *@intag.workfront.com* som du skapar. Under 60-dagarsperioden fortsätter det POP-e-postmeddelande som användes tidigare att fungera.

## Hur testar jag detta i Preview?

Om du vill testa den här ändringen i förhandsgranskningen måste du aktivera e-post i förhandsvisningsmiljön. Det gör du genom att följa instruktionerna i Hantera e-postmeddelanden i förhandsgranskningsavsnittet i [Aktivera leverans av e-postmeddelanden från förhandsgranskningssandlådemiljön](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!IMPORTANT]
>
>Det du anger här kommer inte att överföras till produktionsmiljön. Du måste gå igenom den här processen igen när funktionen har släppts till Produktion.
