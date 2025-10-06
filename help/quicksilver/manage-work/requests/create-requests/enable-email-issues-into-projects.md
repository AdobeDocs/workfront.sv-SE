---
product-area: requests
navigation-topic: create-requests
title: Gör det möjligt för användare att skicka ett ärende via e-post till ett begärandeköprojekt
description: Du kan konfigurera ett projekt så att användare kan lägga till problem i projektet via e-post.
author: Alina, Courtney
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: bca543ad2ee8ead26cfa662900eb513af36f743c
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Gör det möjligt för användare att skicka ett ärende via e-post till ett begärandeköprojekt

<!-- Audited: 4/2025 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Du kan konfigurera ett projekt så att användare kan lägga till problem i projektet via e-post. Du kan bara tillåta att utleveranser e-postas till ett projekt om projektet har angetts som en frågekö. Mer information om hur du skapar ett begärandeköprojekt finns i [Skapa en begärandekö](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> <p>Nytt: Medarbetare eller högre</p>
   eller
   <p>Aktuell: Begäran eller senare</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till problem</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> Produkt</td> 
   <td> <ul><li>Adobe Workfront</li><li>Du måste ha Adobe Workfront Planning för att kunna visa planeringsförfrågningar eller begära formulär</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Följande villkor krävs för att konfigurera ett projekt så att användare kan lägga till problem i projektet via e-post:

* Användare som skickar e-postmeddelanden till det här kontot måste vara aktiva användare med en licens för Workfront.
* Användare som skickar e-postmeddelanden till det här kontot måste ha behörigheten Lägg till problem i projektet.
* Externa användare kan inte skicka e-postmeddelanden till en begärandekö eftersom de inte har åtkomst att skapa problem.
* Det är bara e-postmeddelanden som kommer från en e-postadress som är kopplad till en aktiv Workfront-användare som kan skicka utgåvor till projektet. E-postmeddelanden som vidarebefordras till en aktiv Workfront-användare via e-post som inte är kopplad till ett Workfront-konto kan inte skapa problem under projektet eftersom den ursprungliga avsändarens e-postadress måste kopplas till ett aktivt Workfront-konto.
* Projektet är konfigurerat som en begärandekö.
* E-postkontot som är kopplat till projektet är inte länkat till ett Workfront-användarkonto.

## Konfigurera projektet i Workfront

>[!NOTE]
>
>Tänk på följande när du aktiverar inställningar för e-postkö:
>
>* Workfront tillåter en unik e-postkö per begäran för alla kluster. Om du väljer att inaktivera din begärandekö behåller du den e-postadress du skapade så länge som den fortfarande finns i rutan Ange e-postadress. Om du väljer att inte längre använda e-postadressen måste du ta bort den från fältet Intag-e-post så att den kan användas senare.
>
>* Om det finns flera köämnen eller ämnesgrupper i kön i begärandekön väljer Workfront slumpmässigt det köämne som förfrågningarna ska gå till, vilket gör det svårt att hantera e-postförfrågningar.
>  >Vi rekommenderar att det projekt som du ställer in för att ta emot begäranden via e-post inte ska ha mer än ett köämne. Om de inskickade förfrågningarna är avsedda för olika resurser eller projekt bör du dirigera eller flytta dem manuellt efter att de har skickats.

1. Gå till det projekt som du vill aktivera för att ta emot utgåvor via e-post.
1. Klicka på **Köinformation** i den vänstra panelen.
1. I området **Kötyp** väljer du **Publicera som kö för hjälpbegäran**.

1. Bläddra ned till området **Inställningar för e-postkö** och välj sedan **Aktivera inmatning av begäran via e-post**.

1. Ange början på e-postadressen i rutan **Ange e-postadress**.

   Du måste skapa en unik e-postadress. Vi rekommenderar att du använder ditt företagsnamn som en del av din e-postadress.

   >[!CAUTION]
   >
   >* E-postadressen kan inte återställas från papperskorgen om projektet som innehåller begärandekön tas bort.
   >
   >* Eftersom e-postadressen måste vara unik kanske den inte är tillgänglig i framtiden om den tas bort.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Valfritt) Markera **Vidarebefordra alla problem som inte kan skickas via e-post** och ange sedan en e-postadress för vidarebefordran i rutan nedan.

   Den här e-postadressen får information om e-postmeddelanden som inte kunde skickas till projektet.

1. Klicka på **Spara**. När användare med ett aktivt Workfront-konto skickar ett e-postmeddelande till den här e-postadressen skapas nu ett problem i Workfront-projektet.

   >[!NOTE]
   >
   >Användarna måste kunna skapa problem i projektet för att kunna skicka via e-post. Du kan bevilja den här åtkomsten i dialogrutan Delning under Avancerade inställningar.
   >
   >Externa användare kan inte skicka e-postmeddelanden till en begärandekö eftersom de inte har åtkomst att skapa problem.

## Ta emot utgåvan i Workfront

När en Workfront-användare skickar ett e-postmeddelande till Workfront händer följande:

* Ämnesraden i e-postmeddelandet blir Ärendenamn.
* E-postmeddelandets brödtext blir en beskrivning av problemet.
* Om det finns några dokument bifogade till e-postmeddelandet bifogas dessa dokument till utgåvan i Workfront.

  >[!NOTE]
  >
  > MSG-filer stöds inte och kommer inte att bifogas i Workfront.

* Användaren som skickar e-postmeddelandet blir den primära kontakten för den nya utgåvan i Workfront.
* E-postmeddelandets brödtext får inte vara längre än 4 000 tecken.
* E-postbilagor får inte överskrida totalt 7 MB.
