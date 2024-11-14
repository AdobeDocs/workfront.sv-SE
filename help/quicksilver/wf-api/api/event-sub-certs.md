---
content-type: api
navigation-topic: api-navigation-topic
title: Prenumerationscertifikat för evenemang
description: Prenumerationscertifikat för evenemang
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: c747d3697fd2a4e74dd4af5a8a418d0f52cf71ed
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Konfigurera klient-TLS för händelseprenumeration

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

Med Klient-TLS kan du verifiera att det händelseteckningsmeddelande du får verkligen kommer från Adobe Workfront. Om du vill aktivera den här funktionen måste servern vara konfigurerad att begära och validera Workfront x509-certifikat.


## Verifiera Workfront klientcertifikat

Den här proceduren förutsätter att servern är konfigurerad att acceptera TLS-anslutningar. Workfront stöder inte självsignerade certifikat.

I allmänhet krävs följande steg för att aktivera klientautentisering för servern:

1. Hämta PEM-versionen av DigitalCert Global Root CA-certifikatet.
1. Aktivera verifiering av klientcertifikat.

   Ange certifikatutfärdarcertifikatet från steg 1 som pålitligt.

1. Ange verifieringsdjupet till 2 eftersom vårt certifikat faktiskt signeras av DigitalCert SHA2 Secure Server CA, som är en mellanliggande CA under DigiCert Global Root CA.
1. Kontrollera att klientcertifikatet verkligen kommer från Workfront genom att kontrollera dess ämnesdomännamn.

## Exempel på serverkonfiguration

### NGINX

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

Mer information finns i dokumentationen för [NGiNX för ngx_http_ssl_module](https://nginx.org/en/docs/http/ngx_http_ssl_module.html).

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

Mer information finns i

* [Klientautentisering och åtkomstkontroll](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Apache-modulläge_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## Mappning av certifikat till miljö

| WF-miljö | Certifikatets namn | Certifikatämne (DN) |
| -- | -- | -- |
| Produktion | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com |
| Förhandsgranska | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| Sandlåda 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| Sandlåda 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Hämta certifikat

Klicka på följande länkar för att hämta klientcertifikaten.

* [Klientcertifikat - produktionsmiljö](assets/prod-environment-nov-2024.crt)
* [Klientcertifikat - förhandsvisningsmiljö](assets/preview-environment-nov-2024.crt)
* [Klientcertifikat - sandlådemiljö](assets/sandbox-environment-nov-2024.crt)

>[!NOTE]
>
>Du kan använda samma klientcertifikat för båda sandlådemiljöer.
