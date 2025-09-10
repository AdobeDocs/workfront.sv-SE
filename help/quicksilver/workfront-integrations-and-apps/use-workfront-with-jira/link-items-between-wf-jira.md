---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Länka objekt mellan [!DNL Adobe Workfront] och [!DNL Jira]
description: Du kan länka [!DNL Jira] ärenden till [!DNL Adobe Workfront] uppgifter eller problem antingen automatiskt eller manuellt.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: 064418302767ad20e176080ba9a12db548750f3c
workflow-type: tm+mt
source-wordcount: '1298'
ht-degree: 0%

---

# Länka objekt mellan [!DNL Adobe Workfront] och [!DNL Jira]

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>För att kunna leverera mer stabila och skalbara integreringar går vi över till en modern, flexibel integrationsstrategi med hjälp av Workfront Automation and Integration (Fusion). Som en del av den här övergångsprocessen kommer integreringen av Workfront för Jira inte att vara tillgänglig efter **28 februari 2026**.
>
>Vi rekommenderar att du använder Workfront Automation and Integration för din organisations integreringsbehov med Jira.
>
>En översikt över Workfront Automation and Integration finns i [Adobe Workfront Fusion - översikt](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Mer information om de specifika funktionerna i Workfront Automation and Integration Module för Jira finns i [Jira Software modules](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/sv/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Du kan länka [!DNL Jira] utgåvor till [!DNL Adobe Workfront] uppgifter eller utgåvor antingen automatiskt eller manuellt.

Endast ett objekt i [!DNL Workfront] kan länkas till ett objekt i [!DNL Jira]. Du kan aldrig länka ett [!DNL Workfront]-objekt till flera [!DNL Jira]-utgåvor eller ett [!DNL Jira]-problem till flera [!DNL Workfront]-objekt.

## Åtkomstkrav

Du måste ha följande:

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a></td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över licenser för Adobe [!DNL Workfront]</a></td> 
   <td> 
   <p>Nytt: Standard<p>
   <p>eller</p>
   <p>Aktuell: Planera </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira-åtkomst</td> 
   <td> <p>Systemadministratörsåtkomst</p> <p><b>VIKTIGT</b>

Vi rekommenderar att du skapar separata systemadministratörskonton i [!DNL Jira] och [!DNL Workfront] för att dedikera till den här integreringen, i stället för att använda befintliga konton som kan vara kopplade till användare.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör. Mer information om [!DNL Workfront] administratörer finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du kan länka objekt mellan [!DNL Workfront] och [!DNL Jira] måste du göra följande:

* Installera [!DNL Workfront] för [!DNL Jira].

  Instruktioner finns i [Installera Adobe Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurera [!DNL Workfront] för Jira.

  Instruktioner finns i [Konfigurera Adobe Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Länka automatiskt [!DNL Workfront] objekt till [!DNL Jira] utgåvor

Som [!DNL Workfront]-administratör kan du definiera utlösare som automatiskt skapar ett problem i [!DNL Jira] varje gång vissa villkor uppfylls för en aktivitet eller ett problem i [!DNL Workfront]. Workfront- och [!DNL Jira]-objekten länkas.

När du har slutfört konfigurationen av [!DNL Workfront] för Jira skapas ett nytt objekt automatiskt i [!DNL Workfront] när ett objekt skapas eller uppdateras i [!DNL Jira] för att matcha dina utlösare.

Workfront-användare som skapar och uppdaterar Workfront-objekt behöver ingen [!DNL Jira]-licens för att aktivera skapandet av objekt i [!DNL Jira].

Mer information finns i [Konfigurera [!DNL Adobe Workfront] Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Du kan skapa [!DNL Jira] objekt automatiskt genom att koppla en mall till ett projekt. Om mallen innehåller uppgifter med tilldelningar som uppfyller [!DNL Jira]-utlösarna genereras nya [!DNL Jira]-utgåvor av de nya aktiviteterna.

Att automatiskt länka ett [!DNL Workfront]-problem till ett [!DNL Jira]-problem är identiskt med att automatiskt länka en [!DNL Workfront]-aktivitet till ett [!DNL Jira]-problem.

Så här länkar du automatiskt en [!DNL Workfront]-aktivitet till ett [!DNL Jira]-problem:

1. Kontrollera att systemadministratören för [!DNL Jira] har konfigurerat utlösare för att automatiskt skapa [!DNL Jira] problem när [!DNL Workfront] objekt tilldelas och logga sedan in på [!DNL Workfront] med en åtkomstnivå som gör att du kan skapa en uppgift.

   Mer information om åtkomst till aktiviteter finns i [Bevilja åtkomst till aktiviteter](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

{{step1-to-projects}}

1. Välj ett projekt på sidan **Projekt**.

1. Välj **[!UICONTROL Tasks]** på den vänstra projektpanelen.

1. Klicka på **+ Ny aktivitet**.

   >[!NOTE]
   >
   >Om du vill länka ett befintligt Workfront-objekt till ett Jira-problem väljer du **Redigera** på objektets **Mer** ![Mer-ikon](assets/more-icon.png) -meny.

1. Ange eller uppdatera något av de fält som är tillgängliga för uppgiften.
1. I fältet **[!UICONTROL Assignments]** söker du efter och väljer den användare, roll eller det team som har angetts som utlösare i integreringen av [!DNL Jira].

1. Klicka på **Skapa uppgift**. Uppgiften skapas i Workfront och en ny kommentar visas på aktivitetens **uppdateringsflik** för att ange att ett nytt problem också har skapats i [!DNL Jira].

1. (Valfritt) Klicka på länken **[!UICONTROL Integrations]** i området **[!UICONTROL Details]** i avsnittet **[!UICONTROL Go to Jira]** i huvud för aktiviteten eller problemet för att öppna problemet i Jira.

   Systemet eller gruppadministratören måste lägga till fältet [!UICONTROL Integrations] i layoutmallen för att kunna visa det i huvud för aktiviteten eller utgåvan. Mer information finns i [Anpassa objektrubriker med hjälp av en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Alla [!DNL Jira]-användare kan omedelbart börja arbeta med objekt som har skapats automatiskt från [!DNL Workfront] och deras uppdateringar överförs till [!DNL Workfront] utan att någon licens krävs för att [!DNL Workfront] ska kunna göra det.

   Endast de fält som du som [!DNL Workfront]-administratör konfigurerade under installationen av [!DNL Workfront]-tillägget uppdateras.

   Mer information om att synkronisera fält mellan Workfront och Jira finns i avsnittet Konfigurera Workfront för Jira i [Konfigurera Adobe Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >Utgåvan [!DNL Jira] tilldelas inte till någon i [!DNL Jira] när den skapas automatiskt från Workfront.

## Länka [!DNL Jira]-utgåvor manuellt till [!DNL Workfront]-objekt

När objekt har skapats i [!DNL Jira] och [!DNL Workfront] oberoende av varandra kan du manuellt länka ett [!DNL Jira]-problem till en befintlig [!DNL Workfront]-uppgift eller ett befintligt -problem.

Du kan inte länka ett [!DNL Workfront]-objekt manuellt från [!DNL Workfront] till ett befintligt [!DNL Jira]-objekt.

>[!NOTE]
>
>Om [!DNL Jira]-utgåvan inte finns i ett projekt som inte identifieras som en utlösare i [!DNL Workfront]-integreringen kan du inte länka den manuellt till ett Workfront-objekt när du använder integreringen med [!DNL Jira] On-Premise.\
>Mer information om hur du ställer in utlösare för arbetsflödet Workfront till Jira finns i [Länka automatiskt Workfront-objekt till Jira-problem](#automatically-link-workfront-items-to-jira-issues).

När [!DNL Workfront]- och [!DNL Jira]-objekt är länkade kan vissa fält från ett objekt uppdateras automatiskt på det andra.\
Mer information om hur du uppdaterar länkade objekt finns i [Uppdatera länkade objekt mellan Jira och Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Så här länkar du [!DNL Jira] ärenden manuellt till [!DNL Workfront] objekt:

1. (Villkorligt) Logga in på [!DNL Workfront] och hitta ett problem eller en uppgift som du vill länka till ett [!DNL Jira]-problem.
1. (Villkorligt) I avsnittet **Grundläggande information** på fliken **Aktivitetsinformation** eller **Ärendeinformation** kopierar du **[!UICONTROL Reference Number]** för objektet i Workfront.

   eller

   Kopiera **URL** för objektet i Workfront från adressfältet för objektet.

   >[!IMPORTANT]
   >
   >Om din organisation har anslutit till Adobe Unified Experience måste du använda **referensnumret** för att länka Workfront-objekt till Jira. (Alternativet URL är tillgängligt, men returnerar ett fel om du använder det.) Mer information om enhetlig upplevelse finns i [Adobe Unified Experience för Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
   >
   >För organisationer som inte använder Adobe Unified Experience bör du inte använda URL-alternativet eftersom URL:er kan ändras.

   >[!NOTE]
   >
   >Du måste ha en [!DNL Workfront]-licens för att kunna logga in på [!DNL Workfront]. Annars måste en [!DNL Workfront]-användare ange den här informationen till dig.

1. I [!DNL Jira] navigerar du till ett problem som du vill länka manuellt till [!DNL Workfront]-objektet.
1. Klistra in [!DNL Workfront] eller **[!UICONTROL Reference Number]** URL **för det**-objekt som du vill länka det till i den högra panelen [!DNL Workfront].

1. Klicka på **[!UICONTROL Link]**. De två objekten länkas och den högra panelen [!DNL Workfront] fylls i med information från objektet [!DNL Workfront].

   Som standard visas följande [!DNL Workfront]-fält i [!DNL Jira] på den högra panelen i [!DNL Workfront]:

   * Objektets **[!UICONTROL Name]**. Du kommer åt objektet [!DNL Workfront] genom att klicka på namnet på panelen.
   * **[!UICONTROL Project Name]**.
   * Objektets **[!UICONTROL Status]**.
   * Objektets **[!UICONTROL Priority]**.
   * Det datum då det skapades i [!DNL Workfront].
   * Objektets **[!UICONTROL Planned Hours]**.
   * **[!UICONTROL Reference Number]**. Du kommer åt objektet [!DNL Workfront] genom att klicka på **referensnumret** i panelen.

   Mer information om hur du aktiverar ytterligare fält som ska visas på den högra panelen finns i avsnittet Konfigurera fältsynkronisering mellan [!DNL Jira] och [!DNL Workfront] objekt i [Konfigurera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). En kommentar från [!DNL Workfront]-administratören som är associerad med integreringen publiceras på fliken **[!DNL Workfront]** i utgåvan [!DNL Jira] för att bekräfta att ett nytt [!DNL Jira]-objekt har skapats. Kommentaren innehåller en länk till utgåvan [!DNL Jira].

## Bryt länk mellan [!DNL Jira] och [!DNL Workfront]

Länkade objekt mellan [!DNL Jira] och [!DNL Workfront] kan brytas manuellt i [!DNL Jira]. Du kan inte ta bort länken för ett [!DNL Workfront]-objekt från deras [!DNL Jira]-motsvarighet i [!DNL Workfront].

Du behöver följande åtkomst för att bryta länken till manuellt länkade objekt:

* Du är den användare som manuellt länkade objekten.
* Du är [!DNL Jira]-systemadministratör.

>[!NOTE]
>
>Endast en [!DNL Workfront]-administratör kan bryta länken till objekt som har länkats automatiskt.

Så här bryter du länken för ett [!DNL Jira]-problem från ett [!DNL Workfront]-objekt:

1. Logga in på Jira.
1. Navigera till problemet som är länkat till en [!DNL Workfront]-aktivitet eller ett -problem.
1. Gå till den högra panelen i **Workfront**.
1. Klicka på ikonen **[!UICONTROL Unlink]** och sedan på **[!UICONTROL Unlink]**. De tidigare länkade [!DNL Jira]- och [!DNL Workfront]-objekten bryter länken.

   De fält, kommentarer eller dokument som uppdateras i framtiden uppdateras inte på sin tidigare motsvarighet i det andra programmet.
