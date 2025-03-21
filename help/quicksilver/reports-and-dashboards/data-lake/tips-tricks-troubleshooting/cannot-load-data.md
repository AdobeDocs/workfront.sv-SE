---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Det går inte att upprätta en anslutning
description: När du försöker ansluta skrivbordet till Data Connect får du ett felmeddelande.
author: Courtney
feature: Reports and Dashboards
source-git-commit: e8b1d553ac4761e2b6eae79ae384956105939d90
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Det går inte att upprätta en anslutning

## Problem

När du försöker ansluta skrivbordet till Data Connect visas följande fel:

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## Orsak

Det här felet orsakas av en proxyinställning på den lokala datorn som förhindrar att data läses in från Data Connect.

Data Connect tillhandahålls via Snowflake molntjänster från tredje part. För att kommunicera med Snowflake måste nätverket vara öppet.

## Lösning

Du kan försöka med följande för att lösa problemet:

* **Felsök genom att inaktivera säkerhetsverktyget**: Stäng av säkerhetsverktyget, som Zscaler eller Cisco, för att se om det löser anslutningsproblemet. Om detta löser anslutningsproblemet kontrollerar du att säkerhetsverktyget är uppgraderat till den senaste versionen och lägger till IP-adressen för Data Connect (Snowflake) till VPN-tillåtelselista med ditt interna nätverksteam.

* **Lägg till IP-adresser i Tillåtelselista**: Kontrollera att brandväggsinställningarna tillåter de IP-adresser som används av Data Connect. Använd kommandot `SYSTEM$ALLOWLIST()` för att hämta IP-adressen, som du sedan kan tillåtslista i VPN.

* **Kontrollera brandväggs- och proxyinställningar**: Kontrollera om någon brandvägg eller proxykonfiguration i nätverket blockerar åtkomst till Snowflake slutpunkter. Du kan behöva kontakta din nätverksadministratör för att lägga till de nödvändiga Snowflake IP-adresserna och portarna i företagets tillåtelselista.

* **Tillfällig lösning**: Skapa ett extrakt från en kalkylbladsskärm i stället för Data Source-rutan i Tableau. Anslutningen bryts inte och extraheringsprocessen slutförs.

