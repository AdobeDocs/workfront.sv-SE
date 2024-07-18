---
title: Översikt över utökad autentisering
description: Dold från sökning och från vänster navigering
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: bf8e6c2b8a45cf65840a2ac8b3c25d11266d49f9
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# Översikt över utökad autentisering

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront förändrar systemhanteringen för användare och lösenord. De här ändringarna kommer att införas i en fasversion med namnet **Förbättrad autentisering**. Förbättrad autentisering ger en enhetligare och säkrare inloggningsupplevelse för alla Workfront-produkter och -tjänster.

Följande tabell innehåller information om nuvarande och framtida funktioner:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>Funktion</strong> </p> </th> 
   <th><strong>Äldre autentisering</strong> </th> 
   <th><strong>Förbättrad autentisering 1.0</strong> </th> 
   <th> <p>Förbättrad autentisering 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>Inloggningsalternativ</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Gör det möjligt att använda ett enda användarnamn för alla Workfront-produkter och -tjänster, inklusive utbildning, support med mera</p> </td> 
   <td>Inte tillgängligt</td> 
   <td> <p>Inte tillgängligt</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tillåt att samma e-postadress används i alla Workfront-instanser</p> </td> 
   <td> <p>✓</p> <p>Tillgänglig från och med version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Tillgänglig från och med version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Tillgänglig från och med version 2019.3</p> </td> 
  </tr> 
  <tr> 
   <td> <p>E-postadresser är inte skiftlägeskänsliga</p> </td> 
   <td> <p>✓</p> <p>Tillgänglig från och med version 2019.3</p> </td> 
   <td> <p>✓</p> <p>Flera användare kan inte ha samma e-postadress om adressen bara skiljer sig åt från fall till fall. </p> </td> 
   <td> <p>✓</p> <p>Flera användare kan inte ha samma e-postadress om adressen bara skiljer sig åt från fall till fall. </p> <p>Workfront-administratörer meddelas i slutet av 2019 för att börja korrigera dubblettadresser.</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Alternativ för lösenordshantering</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ange ett e-postmeddelande om återställning av lösenord för en användare som Workfront-administratör</p> </td> 
   <td> <p>Inte tillgängligt </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ange ett tillfälligt lösenord för en användare som Workfront-administratör</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>Inte planerat</p> <p>Den här funktionen är inte den bästa säkerhetsmetoden</p> </td> 
   <td> <p>Inte planerat</p> <p>Den här funktionen är inte den bästa säkerhetsmetoden</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Krav för lösenordsprincip</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Kräv att användare återställer lösenord efter en viss tidsram</p> </td> 
   <td>✓</td> 
   <td> <p>Inte planerat</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Begränsa användare från att använda ett tidigare lösenord </p> </td> 
   <td>✓</td> 
   <td>Inte planerat </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Skydda mot felaktiga försök att ange lösenord </p> </td> 
   <td> <p>✓ </p> <p>Låser kontot efter fem felaktiga lösenordsinmatningsförsök. Väntetiden som krävs efter att utelåsning har konfigurerats av Workfront-administratören</p> </td> 
   <td> <p>✓</p> <p>Väntetiden ökar exponentiellt efter varje efterföljande felaktigt lösenord baserat på branschens bästa praxis. Den tid som krävs kan inte konfigureras av Workfront-administratören</p> </td> 
   <td> <p>✓</p> <p>Använder en låsningsalgoritm som proaktivt blockerar en mängd olika misstänkta beteenden.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Kräv en blandning av gemener, versaler, siffror och specialtecken</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>Ökad flexibilitet vid val av specifika krav</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ange minsta längd för lösenord </p> </td> 
   <td> Inte tillgängligt </td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
  <tr> 
   <td colspan="3"> <p><strong>Stöd för Single Sign-On Protocol</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Stöder SSO-integreringar som är kompatibla med Active Directory- och LDAP-protokoll</p> </td> 
   <td> ✓ </td> 
   <td> <p> Föråldrat</p> <p>Active Directory-, Azure- och LDAP-system bör använda SAML 2.0</p> </td> 
   <td> <p>Föråldrat</p> <p>Active Directory-, Azure- och LDAP-system kan konfigureras med krypterad SAML 2.0 eller OpenID Connect.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Stöder SSO-protokoll som följer SAML 2.0 </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Stöd för Open ID Connect-protokoll</p> </td> 
   <td> <p>Inte tillgängligt</p> </td> 
   <td> <p>Inte tillgängligt</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Konfigurera inloggningssidan för Workfront så att den alltid dirigeras om till inloggningssidan för identitetsleverantören </p> </td> 
   <td> Aktiveras som standard och kan inte inaktiveras</td> 
   <td> <p>✓</p> <p>Workfront-administratören kan konfigurera inloggningssidan så att den dirigeras om till identitetsleverantörens inloggningssida eller så kan en eller flera inloggningsknappar konfigureras.</p> </td> 
   <td> <p>✓</p> <p> Workfront-administratörer kan konfigurera inloggningssidan så att den dirigeras om till identitetsleverantörens inloggningssida eller konfigurera en eller flera inloggningsknappar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Tillåt varje instans att aktivera flera SSO-providers</p> </td> 
   <td> <p>Ej tillämpligt</p> </td> 
   <td> <p>Inte planerat</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>Miljöstöd</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Ett och samma användarnamn och lösenord för förhandsvisningsmiljöer</p> </td> 
   <td> <p>Inte tillgängligt</p> </td> 
   <td> <p>Inte tillgängligt</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ett och samma användarnamn och lösenord för sandlådemiljöer</p> </td> 
   <td> <p>Inte tillgängligt</p> </td> 
   <td> <p>Inte tillgängligt</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p>✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>
