---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Länka objekt mellan [!DNL Adobe Workfront] och [!DNL Jira]
description: Du kan länka [!DNL Jira] problem med [!DNL Adobe Workfront] uppgifter eller problem antingen automatiskt eller manuellt.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# Länka objekt mellan [!DNL Adobe Workfront] och [!DNL Jira]

Du kan länka [!DNL Jira] problem med [!DNL Adobe Workfront] uppgifter eller problem antingen automatiskt eller manuellt.

Endast ett objekt i [!DNL Workfront] kan länkas till ett objekt i [!DNL Jira]. Du kan aldrig länka en [!DNL Workfront] objekt till flera [!DNL Jira] problem, eller ett [!DNL Jira] utgåva till flera [!DNL Workfront] objekt.

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

Vi rekommenderar att du skapar separata systemadministratörskonton i [!DNL Jira] och [!DNL Workfront] att ägna sig åt den här integreringen, i stället för att använda befintliga integreringar som kan vara kopplade till användarna.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara en [!DNL Workfront] administratör. För information om [!DNL Workfront] administratörer, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Förutsättningar

Innan du kan länka objekt mellan [!DNL Workfront] och [!DNL Jira]måste du

* Installera [!DNL Workfront] for [!DNL Jira]

   Anvisningar om hur du installerar Workfront för Jira finns i [Installera Adobe Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Konfigurera [!DNL Workfront] för Jira

   Instruktioner om hur du konfigurerar Workfront för Jira finns i [Konfigurera Adobe Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Länka automatiskt [!DNL Workfront] objekt till [!DNL Jira] problem

Som [!DNL Workfront] kan du definiera utlösare som automatiskt kan skapa ett problem i [!DNL Jira] varje gång vissa villkor uppfylls för en uppgift eller ett problem i [!DNL Workfront]. Workfront och [!DNL Jira] objekt blir länkade.

När du har slutfört konfigurationen av [!DNL Workfront] för Jira, när ett objekt antingen skapas eller uppdateras i [!DNL Workfront] för att matcha dina utlösare skapas ett nytt objekt automatiskt i [!DNL Jira].\
Workfront-användare som skapar och uppdaterar Workfront-objekt behöver ingen [!DNL Jira] licens för att aktivera skapande av objekt i [!DNL Jira].

Mer information om hur du definierar utlösare för att automatiskt skapa Jira-problem finns i  [Konfigurera [!DNL Adobe Workfront] för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Du kan skapa [!DNL Jira] objekt automatiskt genom att koppla en mall till ett projekt. Om mallen innehåller uppgifter med tilldelningar som uppfyller [!DNL Jira] utlösare, de nya aktiviteterna genererar nya [!DNL Jira] problem.

Länka en [!DNL Workfront] skicka till [!DNL Jira] utgåvan är identisk med att automatiskt länka en [!DNL Workfront] till en [!DNL Jira] problem.

Länka en [!DNL Workfront] till en [!DNL Jira] utgåva:

1. Se till att [!DNL Jira] systemadministratören har konfigurerat utlösare för att automatiskt skapa [!DNL Jira] problem när [!DNL Workfront] objekten tilldelas och loggar sedan in på [!DNL Workfront] med en åtkomstnivå som gör att du kan skapa en uppgift.

   Mer information om åtkomst till uppgifter finns i [Bevilja åtkomst till uppgifter](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Gå till ett projekt och välj **[!UICONTROL Tasks]** ![](assets/tasks-icon-in-left-panel-14x14.png) i den vänstra panelen.

1. Klicka på **[!UICONTROL New Task]**

   eller

   Markera en befintlig uppgift och klicka sedan på **Redigera**.

1. Ange eller uppdatera något av de fält som är tillgängliga för uppgiften.
1. Klicka **[!UICONTROL Assignments]** och tilldela uppgiften till en användare, roll eller team som anges som utlösare i [!DNL Jira] integrering.

1. Klicka **Spara ändringar**.

   En ny uppgift skapas i Workfront.

   I **[!UICONTROL Updates]** i den nya aktiviteten finns det en kommentar som anger att en ny utgåva också har skapats i [!DNL Jira].

1. (Valfritt) Klicka på länken till Jira-problemet för att öppna det i Jira.

   eller

   Klicka på **[!UICONTROL Go to Jira]** i **[!UICONTROL Integrations]** området på **[!UICONTROL Details]** -avsnittet eller huvud för aktiviteten eller utgåvan, för att öppna [!DNL Jira] problem.

   Systemadministratören eller gruppadministratören måste lägga till [!UICONTROL Integrations] till layoutmallen för att visa den i huvud för uppgift eller utgåva. Mer information finns i [Anpassa objektrubriker med hjälp av en layoutmall](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Alla [!DNL Jira] kan du börja arbeta med automatiskt skapade objekt från [!DNL Workfront] och uppdateringarna överförs till [!DNL Workfront] utan licens för [!DNL Workfront] att göra det.

   Endast de fält som du är [!DNL Workfront] administratör konfigurerad under installationen av [!DNL Workfront] tillägget uppdateras.

   Mer information om att synkronisera fält mellan Workfront och Jira finns i [Konfigurera Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) avsnitt i  [Konfigurera Adobe Workfront för Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >The [!DNL Jira] utgåvan har inte tilldelats någon i [!DNL Jira] när det skapas automatiskt från Workfront.

## Länka manuellt [!DNL Jira] problem med [!DNL Workfront] objekt

När artiklar har skapats i [!DNL Jira] och [!DNL Workfront], oberoende av varandra, kan du manuellt länka en [!DNL Jira] utgåva till en befintlig [!DNL Workfront] aktivitet eller problem.\
Du kan inte länka en [!DNL Workfront] objekt från [!DNL Workfront] till en befintlig [!DNL Jira] objekt.

>[!NOTE]
>
>Om [!DNL Jira] problemet inte finns i ett projekt som inte identifieras som en utlösare i [!DNL Workfront] Integrationen du inte kan länka manuellt till ett Workfront-objekt när du använder integreringen med [!DNL Jira] Lokalt.\
>Mer information om hur du ställer in utlösare för arbetsflödet Workfront till Jira finns i [Länka automatiskt Workfront-objekt till Jira-problem](#automatically-link-workfront-items-to-jira-issues).

När [!DNL Workfront] och [!DNL Jira] objekt är länkade, vissa fält från ett objekt kan uppdateras automatiskt på det andra.\
Mer information om hur du uppdaterar länkade objekt finns i [Uppdatera länkade objekt mellan Jira och Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Länka manuellt [!DNL Jira] problem med [!DNL Workfront] objekt:

1. (Villkorligt) Logga in på [!DNL Workfront] och hitta ett problem eller en uppgift som du vill länka till [!DNL Jira] problem.
1. (Villkorligt) Kopiera **URL** av objektet i Workfront.

   eller

   Från [!UICONTROL Details] område, kopiera **[!UICONTROL Reference Number]** av objektet i Workfront.

   >[!NOTE]
   >
   >Du måste ha en [!DNL Workfront] licens att logga in på [!DNL Workfront]. I annat fall, en [!DNL Workfront] användaren måste ange den här informationen till dig.

1. I [!DNL Jira]navigera till ett problem som du vill länka till manuellt [!DNL Workfront] objekt.
1. I [!DNL Workfront] höger panel, klistra in **URL** eller **[!UICONTROL Reference Number]** i [!DNL Workfront] objekt som du vill länka till.

1. Klicka på **[!UICONTROL Link]**.

   De två objekten blir länkade och [!DNL Workfront] den högra panelen fylls i med information från [!DNL Workfront] objekt.

   Följande [!DNL Workfront] fält visas i [!DNL Jira]som standard finns i [!DNL Workfront] höger panel:

   * The **[!UICONTROL Name]** för artikeln: Du kommer åt [!DNL Workfront] genom att klicka på namnet på panelen.
   * **[!UICONTROL Project Name]**
   * The **[!UICONTROL Status]** för artikeln
   * The **[!UICONTROL Priority]** för artikeln
   * Det datum då den skapades i [!DNL Workfront]
   * The **[!UICONTROL Planned Hours]** för artikeln
   * The **[!UICONTROL Reference Number]**: Du kommer åt [!DNL Workfront] genom att klicka på [!UICONTROL Reference Number] på panelen.

Mer information om hur du aktiverar ytterligare fält som ska visas på den högra panelen finns i [Konfigurera fältsynkronisering mellan [!DNL Jira] och [!DNL Workfront] Objekt](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) avsnitt i [Konfigurera [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). En kommentar från [!DNL Workfront] administratör som är associerad med integreringen är registrerad i **[!DNL Workfront]** -fliken i [!DNL Jira] bekräfta att en ny [!DNL Jira] objektet har skapats. Kommentaren innehåller en länk till [!DNL Jira] problem.

## Bryt länken mellan objekt [!DNL Jira] och [!DNL Workfront]

Länkade objekt mellan [!DNL Jira] och [!DNL Workfront] kan brytas länken manuellt från [!DNL Jira].\
Du kan inte bryta länken till en [!DNL Workfront] objekt från sina [!DNL Jira] motpart i [!DNL Workfront].

Du behöver följande åtkomst för att bryta länken till manuellt länkade objekt:

* Du är den användare som manuellt länkade objekten
* Du är [!DNL Jira] systemadministratör

Endast en [!DNL Workfront] kan du bryta länken mellan objekt som har länkats automatiskt.

Så här bryter du länken till en [!DNL Jira] utgåva från en [!DNL Workfront] objekt:

1. I [!DNL Jira], navigera till ett problem som är länkat till ett [!DNL Workfront] aktivitet eller problem.
1. Gå till [!DNL Workfront] den högra panelen och klicka på **[!UICONTROL Unlink]** ikonen och klicka sedan på **[!UICONTROL Unlink]**.

   Tidigare länkade [!DNL Jira] och [!DNL Workfront] objekt är nu olänkade. Eventuella fält, kommentarer eller dokument som kan uppdateras individuellt i framtiden uppdateras inte på den tidigare motsvarigheten i det andra programmet.
