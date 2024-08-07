---
content-type: api
navigation-topic: api-navigation-topic
title: Inaktuella tecken i API-svar
description: Inaktuella tecken i API-svar
author: Becky
feature: Workfront API
role: Developer
exl-id: 1477b98e-1cdc-4661-b3ee-0b6ab1e8c3ee
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 4%

---

# Inaktuella tecken i API-svar

Syntaxen för vissa API-svar kan innehålla undantagstecknet `\` (omvänt snedstreck). Ett escape-tecken anger att tecknet eller teckensträngen som omedelbart följer escape-tecknet har ett specialvärde. `\t` säger till exempel till läsenheten att `t` ska tolkas som `tab` och inte som bokstaven&quot;t&quot;. En sträng med ett eller flera tecken efter det omvända snedstrecket kallas en escape-sekvens.

Hexadecimal escape-sekvens kräver att giltiga hexadecimala siffror används. I följande tabell visas de escape-sekvenser som är kodade i Adobe Workfront API-svar:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Escape-sekvens</strong> </th> 
   <th><strong>Unicode-tecken</strong> </th> 
   <th><strong>Representerar</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>\u000<em>x</em></p> <p>Där, <em>x</em> är den hexadecimala koden för siffrorna 0 till 7</p> </td> 
   <td>0-7</td> 
   <td>Unicode-tecken som representeras av kodpunkterna 0 till 7</td> 
  </tr> 
  <tr> 
   <td>\b</td> 
   <td>8</td> 
   <td>Backsteg</td> 
  </tr> 
  <tr> 
   <td>\t</td> 
   <td>9</td> 
   <td>Tabb</td> 
  </tr> 
  <tr> 
   <td>\n</td> 
   <td>10</td> 
   <td>Ny rad</td> 
  </tr> 
  <tr> 
   <td>\u000b</td> 
   <td>11</td> 
   <td>Lodrät flik</td> 
  </tr> 
  <tr> 
   <td>\f</td> 
   <td>12</td> 
   <td>Formulärfeed</td> 
  </tr> 
  <tr> 
   <td>\r</td> 
   <td>13</td> 
   <td>Radretur</td> 
  </tr> 
  <tr> 
   <td> <p>\u00<em>xx</em></p> <p><em>Där är xx den hexadecimala koden för  tal 14 till 31 </em> </p> </td> 
   <td>14-31</td> 
   <td>Unicode-tecken som representeras av kodpunkterna 14 till 31</td> 
  </tr> 
  <tr> 
   <td> <p>\/</p> </td> 
   <td>47</td> 
   <td>/ (Snedstreck)</td> 
  </tr> 
  <tr> 
   <td> <p>\u003c</p> </td> 
   <td>60</td> 
   <td>&lt; (mindre än)</td> 
  </tr> 
  <tr> 
   <td> <p>\\</p> </td> 
   <td>92</td> 
   <td>\ (omvänt snedstreck)</td> 
  </tr> 
  <tr> 
   <td> <p>\u<em>xxxx</em></p> <p>Där <em>xxxx</em> är den hexadecimala koden för ett tal över 127</p> </td> 
   <td>128+</td> 
   <td>Unicode-tecken för alla kodpunkter över 127</td> 
  </tr> 
 </tbody> 
</table>
