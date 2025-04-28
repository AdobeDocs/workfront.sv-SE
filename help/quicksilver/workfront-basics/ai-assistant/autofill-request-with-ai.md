---
title: Fyll i en begäran automatiskt med hjälp av AI
content-type: reference
description: Du kan använda AI för att fylla i begärandefält automatiskt.
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
source-git-commit: 9e1a5718092092bb9ca98cf92ddd2a1a07f32f51
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Fyll i en begäran automatiskt med hjälp av AI

AI kan hjälpa dig att fylla i begärandefält automatiskt. Det kan föreslå fältvärden baserat på tidigare förfrågningar eller tolka dem från text som e-post.

Du kan godkänna eller avvisa dessa inskickade svar innan du skickar in begäran.

Autofyll skriver inte över fält som du redan har fyllt i.

## Få förslag när du fyller i formulär

Autofyll kan föreslå fältvärden medan du fyller i formuläret. När du anger värden i begärandefälten jämför Workfront dessa värden med tidigare begäranden. Om det angivna värdet har en nära koppling till andra fältvärden i liknande sammanhang i tidigare begäranden föreslår Workfront dessa värden.

Om t.ex. en klinik alltid använder samma faktureringskod föreslår Workfront att faktureringskoden anges i rätt fält när det kliniska namnet anges.

Så här använder du förslag som baseras på tidigare begäranden:

1. Börja skapa en begäran.

   Instruktioner finns i [Skapa och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Börja fylla i fält.

   När du fyller i fält kan andra fält visa förslag.

1. För varje fältförslag väljer du **Acceptera** eller **Avvisa** under det fältet.

   eller

   Välj **Acceptera alla** eller **Ignorera alla** överst på sidan om du vill acceptera eller ignorera alla förslag.

## Få förslag från en textfråga

Autofyll kan föreslå fältvärden baserade på text som e-post. Du klistrar in i ett textblock och Workfront bearbetade texten för att föreslå fältvärden som baseras på texten.

Om e-postmeddelandet t.ex. innehåller&quot;Detta förfaller den 1 juni&quot; och formuläret innehåller ett fält för förfallodatum, föreslår Workfront 1 juni för det fältvärdet.

Den här typen av förslag kontrollerar även tidigare begäranden om liknande sammanhang. Om uppmaningen t.ex. anger att begäran gäller en viss klient kan Workfront automatiskt hitta och ange faktureringsadressen för den klienten baserat på tidigare begäranden.

Du kan klistra in text som ska användas i hela formuläret eller i ett enskilt avsnitt i formuläret.

Så här använder du förslag som baseras på en inklistrad textfråga:

1. Börja skapa en begäran.

   Instruktioner finns i [Skapa och skicka begäranden](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Klicka på **Fyll automatiskt med AI** i skärmens övre högra hörn om du vill använda textprompten i hela formuläret.

   eller

   Klicka på AI-ikonen ![AI-ikonen](assets/request-prompt-icon.png) bredvid avsnittsnamnet om du vill använda textprompten för ett enskilt avsnitt.

1. Klistra in texten i rutan.
1. Klicka på **Fyll i formuläret**.

   Workfront genererar förslag för formuläret.
1. För varje fältförslag väljer du **Acceptera** eller **Avvisa** under det fältet.

   eller

   Välj **Acceptera alla** eller **Ignorera alla** överst på sidan om du vill acceptera eller ignorera alla förslag.

