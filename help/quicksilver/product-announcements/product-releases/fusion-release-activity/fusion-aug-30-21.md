---
title: Workfront Fusion-släppningsaktivitet:&nbsp;Vecka den 30 augusti 2021
description: Workfront Fusion-släppningsaktivitet:&nbsp;Vecka den 30 augusti 2021
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Versionsaktivitet för Workfront Fusion: 30 augusti 2021

Den här sidan beskriver alla förbättringar som gjorts i Adobe Workfront Fusion den 30 augusti 2021.

En lista med alla senaste ändringar finns på [Versionsaktivitet för Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

En lista med de senaste felkorrigeringarna i Workfront Fusion finns i [Workfront Maintenance Updates](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) och sök efter uppdateringar som heter Workfront Fusion Maintenance Update.

## Filtrera händelser som utlöser Workfront > Bevakningshändelser

1. Konfigurera ett eget filter för händelser som utlöser Workfront > Bevakningshändelser

   För att minska antalet onödiga scenariokörningar har vi uppdaterat modulen Workfront > Bevakade poster för att aktivera händelsefiltrering. Nu kan du ange ett filter när du skapar en webkrok. Detta gör att scenariot bara kan utlösas när händelsen uppfyller vissa villkor.

   Händelsefiltret erbjuder för närvarande följande åtgärder:

   * Lika med: Utlös ett scenario endast när en händelse matchar villkoren för filtret. Du kan till exempel konfigurera ett filter som utlöser ett scenario endast om händelsen inträffar i ett visst projekt.
   * Inte lika med: Utlös bara ett scenario om en händelse inte matchar villkoren för filtret. Du kan t.ex. skapa ett filter som utlöser ett scenario endast om det problem som en händelse inträffar i inte har statusen Stängt.

   Tidigare skulle modulen Bevakade poster hämta alla poster. Användare kan bara filtrera genom att konfigurera filter senare i scenariot.

   Om du vill använda händelsefiltrering skapar du en ny webkrok i modulen Bevaka händelser. Det är för närvarande inte möjligt att redigera befintliga webbböcker så att de innehåller den här funktionen. Vi rekommenderar starkt att du skapar nya webbböcker med händelsefilter för dina befintliga scenarier.

1. Filtrera ut händelser som utlöses av den aktuella anslutningen.

   För att göra det enklare att ställa in dina webbböcker för modulen Workfront > Bevaka händelser har vi tagit med det vanligaste händelsefiltret. Nu har webbokroken ett alternativ för att filtrera bort ändringar som gjorts av moduler med den anslutning som angetts för bevakningsmodulen. Med andra ord, om det här filtret är aktiverat kan eventuella ändringar som görs av Workfront-användaren och som är kopplade till anslutningen inte utlösa scenariot.

   Tidigare var det här filtret inte tillgängligt. Därför var det enklare för ändringar som gjorts i Workfront-moduler att utlösa scenarier som innehåller dessa moduler, vilket eventuellt kan göra att scenarier utlöses i en oändlig slinga.

Mer information om händelsefilter i modulen Workfront > Bevakade händelser finns i [Adobe Workfront-moduler](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

