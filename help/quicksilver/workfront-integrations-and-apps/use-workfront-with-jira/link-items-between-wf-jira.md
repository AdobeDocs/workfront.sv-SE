---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Länka objekt mellan [!DNL Adobe Workfront] och [!DNL Jira]
description: Du kan länka [!DNL Jira] ärenden till [!DNL Adobe Workfront] uppgifter eller problem antingen automatiskt eller manuellt.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '1199'
ht-degree: 0%

---

# Länka objekt mellan [!DNL Adobe Workfront] och [!DNL Jira]

Du kan länka [!DNL Jira] utgåvor till [!DNL Adobe Workfront] uppgifter eller utgåvor antingen automatiskt eller manuellt.

Endast ett objekt i [!DNL Workfront] kan länkas till ett objekt i [!DNL Jira]. Du kan aldrig länka ett [!DNL Workfront]-objekt till flera [!DNL Jira]-utgåvor eller ett [!DNL Jira]-problem till flera [!DNL Workfront]-objekt.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plan]</a>*</td> 
   <td> <p>[!UICONTROL Pro] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] licensöversikt</a>*</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Jira-åtkomst</td> 
   <td> <p>Systemadministratörsåtkomst</p> <p><b>VIKTIGT</b>

Vi rekommenderar att du skapar separata systemadministratörskonton i [!DNL Jira] och [!DNL Workfront] för att dedikera till den här integreringen, i stället för att använda befintliga konton som kan vara kopplade till användare.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör. Mer information om [!DNL Workfront] administratörer finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja en användare fullständig administrativ åtkomst</a>.</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du kan länka objekt mellan [!DNL Workfront] och [!DNL Jira] måste du

* Installera [!DNL Workfront] för [!DNL Jira]

  Instruktioner om hur du installerar Workfront för Jira finns i [Installera Adobe Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurera [!DNL Workfront] för Jira

  Instruktioner om hur du konfigurerar Workfront för Jira finns i [Konfigurera Adobe Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Länka automatiskt [!DNL Workfront] objekt till [!DNL Jira] utgåvor

Som [!DNL Workfront]-administratör kan du definiera utlösare som automatiskt kan skapa ett problem i [!DNL Jira] varje gång vissa villkor uppfylls för en aktivitet eller ett problem i [!DNL Workfront]. Workfront- och [!DNL Jira]-objekten länkas.

När du har slutfört konfigurationen av [!DNL Workfront] för Jira skapas ett nytt objekt automatiskt i [!DNL Jira] när ett objekt skapas eller uppdateras i [!DNL Workfront] för att matcha dina utlösare.\
Workfront-användare som skapar och uppdaterar Workfront-objekt behöver ingen [!DNL Jira]-licens för att aktivera skapandet av objekt i [!DNL Jira].

Mer information om hur du definierar utlösare för att automatiskt skapa Jira-problem finns i [Konfigurera [!DNL Adobe Workfront] för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Du kan skapa [!DNL Jira] objekt automatiskt genom att koppla en mall till ett projekt. Om mallen innehåller uppgifter med tilldelningar som uppfyller [!DNL Jira]-utlösarna genereras nya [!DNL Jira]-utgåvor av de nya aktiviteterna.

Att automatiskt länka ett [!DNL Workfront]-problem till ett [!DNL Jira]-problem är identiskt med att automatiskt länka en [!DNL Workfront]-aktivitet till ett [!DNL Jira]-problem.

Så här länkar du automatiskt en [!DNL Workfront]-aktivitet till ett [!DNL Jira]-problem:

1. Kontrollera att systemadministratören för [!DNL Jira] har konfigurerat utlösare för att automatiskt skapa [!DNL Jira] problem när [!DNL Workfront] objekt tilldelas och logga sedan in på [!DNL Workfront] med en åtkomstnivå som gör att du kan skapa en uppgift.

   Mer information om åtkomst till aktiviteter finns i [Bevilja åtkomst till aktiviteter](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Gå till ett projekt och välj **[!UICONTROL Tasks]** ![Aktivitetsikonen](assets/tasks-icon-in-left-panel-14x14.png) i den vänstra panelen.

1. Klicka på **[!UICONTROL New Task]**

   eller

   Markera en befintlig aktivitet och klicka sedan på **Redigera**.

1. Ange eller uppdatera något av de fält som är tillgängliga för uppgiften.
1. Klicka på **[!UICONTROL Assignments]** och tilldela uppgiften till en användare, roll eller team som har angetts som utlösare i integreringen av [!DNL Jira].

1. Klicka på **Spara ändringar**.

   En ny uppgift skapas i Workfront.

   I området **[!UICONTROL Updates]** för den nya aktiviteten finns det en kommentar som anger att ett nytt problem också har skapats i [!DNL Jira].

1. (Valfritt) Klicka på länken till Jira-problemet för att öppna det i Jira.

   eller

   Klicka på länken **[!UICONTROL Go to Jira]** i området **[!UICONTROL Integrations]** i avsnittet **[!UICONTROL Details]** eller på uppgifts- eller ärendehuvudet för att öppna problemet [!DNL Jira].

   Systemet eller gruppadministratören måste lägga till fältet [!UICONTROL Integrations] i layoutmallen för att kunna visa det i huvud för aktiviteten eller utgåvan. Mer information finns i [Anpassa objektrubriker med hjälp av en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Alla [!DNL Jira]-användare kan omedelbart börja arbeta med objekt som har skapats automatiskt från [!DNL Workfront] och deras uppdateringar överförs till [!DNL Workfront] utan att någon licens krävs för att [!DNL Workfront] ska kunna göra det.

   Endast de fält som du som [!DNL Workfront]-administratör konfigurerade under installationen av [!DNL Workfront]-tillägget uppdateras.

   Mer information om att synkronisera fält mellan Workfront och Jira finns i avsnittet [Konfigurera Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) i [Konfigurera Adobe Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >Utgåvan [!DNL Jira] tilldelas inte till någon i [!DNL Jira] när den skapas automatiskt från Workfront.

## Länka [!DNL Jira]-utgåvor manuellt till [!DNL Workfront]-objekt

När objekt har skapats i [!DNL Jira] och [!DNL Workfront], oberoende av varandra, kan du manuellt länka ett [!DNL Jira]-problem till en befintlig [!DNL Workfront]-uppgift eller ett befintligt -problem.\
Du kan inte länka ett [!DNL Workfront]-objekt manuellt från [!DNL Workfront] till ett befintligt [!DNL Jira]-objekt.

>[!NOTE]
>
>Om [!DNL Jira]-utgåvan inte finns i ett projekt som inte identifieras som en utlösare i [!DNL Workfront]-integreringen kan du inte länka den manuellt till ett Workfront-objekt när du använder integreringen med [!DNL Jira] On-Premise.\
>Mer information om hur du ställer in utlösare för arbetsflödet Workfront till Jira finns i [Länka automatiskt Workfront-objekt till Jira-problem](#automatically-link-workfront-items-to-jira-issues).

När [!DNL Workfront]- och [!DNL Jira]-objekt är länkade kan vissa fält från ett objekt uppdateras automatiskt på det andra.\
Mer information om hur du uppdaterar länkade objekt finns i [Uppdatera länkade objekt mellan Jira och Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Så här länkar du [!DNL Jira] ärenden manuellt till [!DNL Workfront] objekt:

1. (Villkorligt) Logga in på [!DNL Workfront] och hitta ett problem eller en uppgift som du vill länka till [!DNL Jira] -problemet.
1. (Villkorligt) Kopiera **[!UICONTROL Reference Number]** för objektet i Workfront från området [!UICONTROL Details].

   eller

   Kopiera **URL** för objektet i Workfront från adressfältet för objektet.

   >[!IMPORTANT]
   >
   >Om din organisation har anslutit sig till Adobe Unified Experience måste du använda **Reference Number** för att länka Workfront-objekt till Jira. (Alternativet URL är tillgängligt, men returnerar ett fel om du använder det.) Mer information om den enhetliga upplevelsen finns i [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
   >
   >För organisationer som inte använder Adobe Unified Experience bör du inte använda URL-alternativet eftersom URL:er kan ändras.

   >[!NOTE]
   >
   >Du måste ha en [!DNL Workfront]-licens för att kunna logga in på [!DNL Workfront]. Annars måste en [!DNL Workfront]-användare ange den här informationen till dig.

1. I [!DNL Jira] navigerar du till ett problem som du vill länka manuellt till [!DNL Workfront]-objektet.
1. Klistra in **[!UICONTROL Reference Number]** eller **URL** för det [!DNL Workfront]-objekt som du vill länka till i den högra panelen [!DNL Workfront].

1. Klicka på **[!UICONTROL Link]**.

   De två objekten länkas och den högra panelen [!DNL Workfront] fylls i med information från objektet [!DNL Workfront].

   Följande [!DNL Workfront]-fält visas som standard i [!DNL Jira] på den högra panelen i [!DNL Workfront]:

   * Objektets **[!UICONTROL Name]**: Du kan komma åt [!DNL Workfront]-objektet genom att klicka på namnet på panelen.
   * **[!UICONTROL Project Name]**
   * Objektets **[!UICONTROL Status]**
   * Objektets **[!UICONTROL Priority]**
   * Det datum då den skapades i [!DNL Workfront]
   * Objektets **[!UICONTROL Planned Hours]**
   * **[!UICONTROL Reference Number]**: Du kommer åt [!DNL Workfront]-objektet genom att klicka på [!UICONTROL Reference Number] på panelen.

Mer information om hur du aktiverar ytterligare fält som ska visas på den högra panelen finns i avsnittet [Konfigurera fältsynkronisering mellan [!DNL Jira] och [!DNL Workfront] objekt](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) i [Konfigurera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). En kommentar från [!DNL Workfront]-administratören som är associerad med integreringen publiceras på fliken **[!DNL Workfront]** i utgåvan [!DNL Jira] för att bekräfta att ett nytt [!DNL Jira]-objekt har skapats. Kommentaren innehåller en länk till utgåvan [!DNL Jira].

## Bryt länk mellan [!DNL Jira] och [!DNL Workfront]

Länkade objekt mellan [!DNL Jira] och [!DNL Workfront] kan brytas manuellt från [!DNL Jira].\
Du kan inte ta bort länken för ett [!DNL Workfront]-objekt från deras [!DNL Jira]-motsvarighet i [!DNL Workfront].

Du behöver följande åtkomst för att bryta länken till manuellt länkade objekt:

* Du är den användare som manuellt länkade objekten
* Du är [!DNL Jira]-systemadministratör

Endast en [!DNL Workfront]-administratör kan bryta länken till objekt som har länkats automatiskt.

Så här bryter du länken för ett [!DNL Jira]-problem från ett [!DNL Workfront]-objekt:

1. I [!DNL Jira] navigerar du till ett problem som är länkat till en [!DNL Workfront]-aktivitet eller ett -problem.
1. Gå till den högra panelen [!DNL Workfront] och klicka på ikonen **[!UICONTROL Unlink]** och klicka sedan på **[!UICONTROL Unlink]**.

   De tidigare länkade [!DNL Jira]- och [!DNL Workfront]-objekten är nu inte länkade. Eventuella fält, kommentarer eller dokument som kan uppdateras individuellt i framtiden uppdateras inte på den tidigare motsvarigheten i det andra programmet.
