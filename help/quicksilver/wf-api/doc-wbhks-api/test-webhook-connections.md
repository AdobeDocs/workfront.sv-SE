---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Testa webkrockanslutningar
description: Testa webkrockanslutningar
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---


# Testa webkrockanslutningar

Kör de manuella testerna i det här avsnittet för att kontrollera att implementeringen av dokumentwebkroken fungerar som den ska. Dessa steg går igenom Adobe Workfront webbgränssnitt och når indirekt slutpunkterna för webkromimplementeringen.

## Förutsättningar

Följande krav krävs för att köra testerna:

* Ett Workfront-konto med ADM (Advanced Document Management) aktiverat

* En Workfront-användare för det här kontot med systemadministratörsbehörighet

* En webkrockinstans för dokument med HTTP-slutpunkter som är tillgängliga för Workfront

Dessa tester förutsätter också att din Document Webkroch-instans är registrerad. (Du kan registrera din instans i Workfront under Konfigurera > Dokument > Anpassade integreringar.)

**Test 1: Etablera dokumentwebbkroktjänsten för en användare**

Testar autentiserings-URL:en och tokens slutpunkts-URL:en för OAuth-baserade webkrockproviders.

1. I Workfront går du till huvuddokumentsidan genom att klicka på länken Dokument i det övre navigeringsfältet.
1. Klicka på listrutan Lägg till dokument och välj webbhotell för dokument under Lägg till tjänst.
1. (Endast OAuth-tjänster) När du har slutfört föregående steg visas tjänstens OAuth2-autentiseringssida i ett popup-fönster. (Obs! Du kan uppmanas att logga in på tjänsten först.) Från autentiseringssidan ger du Workfront åtkomst till användarens konto genom att klicka på knappen Lita på eller Tillåt.
1. Kontrollera att tjänsten har lagts till i listrutan Lägg till dokument. Om du inte ser den från början kan du försöka med att uppdatera webbläsaren.

**Test 2: Länka ett dokument till Workfront Testar följande slutpunkter: /files, /metadata**

1. I Workfront går du till huvuddokumentsidan genom att klicka på länken Dokument i det övre navigeringsfältet.
1. Välj webbkroktjänsten för dokument under Lägg till dokument.
1. Navigera i mappstrukturen från modala medier.
1. Kontrollera att du kan navigera i mappstrukturen.
1. Markera och länka ett dokument till Workfront

**Test 3: Navigera till ett dokument i innehållshanteringssystemet**

Testar följande slutpunkter: /metadata (särskilt viewLink)

1. Länka ett dokument till Workfront
1. Markera dokumentet och klicka på länken Öppna.
1. Kontrollera att dokumentet öppnas på en ny flik.

**Test 4: Navigera till ett dokument i innehållshanteringssystemet (med inloggning)**

Testar följande slutpunkter: /metadata (särskilt viewLink)

1. Se till att du är utloggad från innehållshanteringssystemet.
1. Länka ett dokument till Workfront.
1. Markera dokumentet och klicka på länken Öppna.
1. Verifiera att inloggningsskärmen för innehållshanteringssystemet läses in på en ny flik.
1. Logga in och verifiera att du kommer till dokumentet

**Test 5: Hämta dokumentet från innehållshanteringssystemet**

Testar följande slutpunkter (särskilt nedladdningslänken): /metadata 

1. Länka ett dokument till Workfront.
1. Markera dokumentet och klicka på länken Hämta.
1. Kontrollera att hämtningen börjar.

**Test 6: Sök efter innehåll**

Testar följande slutpunkter: /search

1. I Workfront går du till huvuddokumentsidan genom att klicka på länken Dokument i det övre navigeringsfältet.
1. Välj webbkroktjänsten för dokument under Lägg till dokument.
1. Utför en sökning från modal.
1. Kontrollera att sökresultaten är korrekta.

**Test 7: Skicka dokument från Workfront till innehållshanteringssystemet**

Testar följande slutpunkter: /files, /uploadInit, /upload

1. I Workfront går du till huvuddokumentsidan genom att klicka på länken Dokument i det övre navigeringsfältet.
1. Överföra ett dokument till Workfront från datorn
1. Gå till sidan med dokumentinformation
1. I listrutan Dokumentåtgärder väljer du webbkroktjänsten för dokument under Skicka till...
1. Gå till önskad målmapp och klicka på knappen Spara.
1. Kontrollera att dokumentet har överförts till rätt plats i innehållshanteringssystemet.

**Test 8: Visa miniatyrbilder i Workfront**

Testar följande slutpunkter: /miniatyrbild

1. Länka ett dokument till Workfront.
1. Markera dokumentet i listan.
1. Kontrollera att miniatyrbilden visas på den högra panelen.

**Test 9: Hämta innehållets byte**

Testar följande slutpunkter: /download

1. Länka ett dokument till Workfront.
1. Gå till dokumentinformationssidan.
1. Skicka dokumentet till Workfront genom att välja Dokumentåtgärder > Skicka till.. > Workfront. Då skapas en ny dokumentversion i Workfront.
1. Hämta dokumentet från Workfront genom att klicka på länken Hämta.

**Test 10: Uppdatera åtkomsttoken (endast OAuth2-webbhotell)**

Testar följande slutpunkter: Token Endpoint URL

1. Tillhandahålla en webbkroktjänst för dokument för en användare
1. Invalidera användarens åtkomsttoken genom att antingen 1 ) vänta på timeout eller 2) ogiltigförklara den manuellt i det externa systemet.
1. Uppdatera åtkomsttoken i Workfront. Du kan göra detta t.ex. genom att länka ett dokument till Workfront. Du kommer att känna till att åtkomsttoken uppdaterades korrekt om du kunde navigera till och länka ett dokument.

>[!NOTE]
>
>För närvarande är Skicka till inte tillgängligt för länkade dokument. Detta läggs till av Workfront. Du kan testa slutpunkten för /download genom att trycka på slutpunkten manuellt med en REST-klient, till exempel Postman. Alternativt kan du testa slutpunkten för /download genom att generera ett digitalt korrektur. Om du vill aktivera korrektur på webben kontaktar du Workfront.
