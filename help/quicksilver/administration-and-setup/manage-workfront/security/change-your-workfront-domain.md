---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Ändra din Adobe Workfront-domän
description: Som Adobe Workfront-administratör och behörig Workfront Support-kontakt kan du begära hjälp från Workfront Support-team för att ändra din organisations Workfront-domän.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d817bd2b-1aaa-4dde-8e75-392c1da2943a
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Ändra din Adobe Workfront-domän

>[!IMPORTANT]
>
>Den procedur som beskrivs på denna sida gäller endast organisationer som ännu inte har anslutit sig till Admin Console. Om din organisation har anslutit sig till Adobe Admin Console går det inte att ändra din Workfront-domän.
>
>En lista över procedurer som skiljer sig åt beroende på om din organisation har anslutit sig till Adobe Admin Console finns i [Plattformsbaserade administrationsskillnader (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Som Adobe Workfront-administratör och behörig Workfront Support-kontakt kan du begära hjälp från Workfront Support-team för att ändra din organisations Workfront-domän.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Begär en domänändring

1. Börja skapa en supportanmälan på Experience League.
1. I rutan **Beskrivning** tar du med den nya domänen som du vill ha samt tidsramen när du vill att den nya domänen ska vara aktiv.
1. Fyll i rutorna för supportärendet och klicka sedan på **Skicka**.

Du kan även ringa Workfront Support och få hjälp med att ändra din domän.

## Uppdatera den nya domänen om du är en SSO-kund

Om ditt företag använder enkel inloggning krävs följande steg när du har ändrat din Workfront-domän.

>[!NOTE]
>
>Detta är inte tillgängligt om din organisations Workfront-instans har aktiverats med Adobe IMS. Kontakta nätverks- eller IT-administratören om du behöver mer information.

{{step-1-to-setup}}

1. Klicka på **System** > **Kundinformation** i det vänstra sidofältet och kontrollera att din domän är uppdaterad på sidan Kundinformation.

1. Klicka på **System** > **enkel inloggning (SSO)** i den vänstra sidofältet.

1. Klicka på **Hämta SAML 2.0-metadata**.
1. När filen har laddats ned öppnar du den och ser till att du har följande:

   1. **entityID** pekar på den nya domänen.
   1. Alla platser inom **`<md:AssertionConsumerService>`** pekar på den nya domänen.

1. Skicka den hämtade metadatafilen till din identitetsleverantör så att de kan uppdatera den när de vill.
1. Se till att domänen uppdateras för alla Workfront-integreringar som används av din organisation.
