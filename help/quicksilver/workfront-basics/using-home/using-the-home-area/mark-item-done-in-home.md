---
product-area: projects
navigation-topic: use-the-home-area
title: Markera ett objekt som färdigt i hemområdet
description: Du kan markera en uppgift eller ett problem som Klar om du är den som tilldelats uppgiften eller utgåvan. När du markerar en uppgift eller ett problem som Klar ändras aktivitetens eller problemets status till Fullständig.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: 4c3638aa-5ee3-422a-9fee-41c4749fe48b
source-git-commit: 073e6c7d4e830dfd2b8920a20e1490c5524d71bd
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# Markera ett objekt som [!UICONTROL Done] i [!UICONTROL Home] area

Du kan markera en uppgift eller ett problem som Klar om du är den som tilldelats uppgiften eller utgåvan. När du markerar en uppgift eller ett problem som [!UICONTROL Done], statusen för uppgiften eller utgåvan ändras till [!UICONTROL Complete].

>[!NOTE]
>
>Du ser inte [!UICONTROL Done] om du inte är en av de resurser som tilldelats uppgiften eller problemet.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Work] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL Edit] tillgång till uppgifter och ärenden</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Contribute-behörigheter eller högre för de uppgifter och ärenden du behöver arbeta med</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Markera en aktivitet eller ett problem som [!UICONTROL Done]

Endast användaren som är tilldelad uppgiften eller utgåvan kan markera den som [!UICONTROL Done].

1. Klicka på **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) i det övre högra hörnet och klicka sedan på **[!UICONTROL Home]**.
1. I **[!UICONTROL Work List]**, letar du reda på objekten som du vill arbeta med.
1. Gör något av följande:

* Klicka **[!UICONTROL Done]** på arbetsuppgiften.\
   Se [Förstå alternativen i [!UICONTROL Done] knapp](#understand-the-options-of-the-done-button) om du vill ha mer detaljerad information om hur knappen kan visas.

* Markera objektet som du vill markera som färdigt och klicka sedan på **[!UICONTROL Update Status]**&#x200B;ändrar du sedan status för objektet till en status som motsvarar [!UICONTROL Complete] eller [!UICONTROL Closed].

## Förstå alternativen i [!UICONTROL Done] knapp

Som standard klickar du på [!UICONTROL Done] på en arbetsuppgift ändrar objektets status till [!UICONTROL Complete] (för uppgifter) eller [!UICONTROL Resolved] (för problem).

Dina [!DNL Adobe Workfront] kan administratören anpassa vilka statusvärden som är kopplade till [!UICONTROL Done] och tillämpa anpassningarna på ditt Home Team.

Beroende på hur många statusvärden som är associerade med [!UICONTROL Done] eller hur många resurser som tilldelats aktiviteten eller problemet, utseendet på [!UICONTROL Done] kan ändras.

* [[!UICONTROL Done] knapp som är associerad med en status](#done-button-associated-with-one-status)
* [[!UICONTROL Done] knapp som är associerad med flera statusar](#done-button-associated-with-multiple-statuses)
* [[!UICONTROL Done] knapp för artiklar som tilldelats flera resurser](#done-button-for-items-assigned-to-multiple-resources)

### [!UICONTROL Done] knapp som är associerad med en status

När [!UICONTROL Done] är associerad med en status och arbetsuppgiften är endast tilldelad dig, knappen läser **[!UICONTROL Done]**. När du klickar på den ändras aktivitetens eller problemets status till den status som är associerad med [!UICONTROL Done] -knappen.

![Knappen Klar](assets/Done.png)

För att förstå vilken status som är associerad med [!UICONTROL Done] knappen, kontrollera [!UICONTROL Team Settings] i ditt hemteam för [!UICONTROL Done Button] -sektion, enligt beskrivning i [Redigera teaminställningar](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).

Om du inte är tilldelad något hemteam väljs standardstatus när du klickar på [!UICONTROL Done], enligt beskrivningen ovan i [Förstå alternativen i [!UICONTROL Done] knapp](#understand-the-options-of-the-done-button).

### [!UICONTROL Done] knapp som är associerad med flera statusar

När [!UICONTROL Done] är associerad med mer än en status, knappen visar ordet **[!UICONTROL Done]** som följs av en nedrullningsbar meny. I det här scenariot kan du inte bara klicka [!UICONTROL Done]. Du måste välja en status i listrutan. Välj den status som bäst passar för slutförandet av arbetsuppgiften. Genom att göra detta ändrar du status för arbetsobjektet.

För att förstå hur du kan associera flera statusvärden med [!UICONTROL Done] knapp, se [Konfigurera [!UICONTROL Done] knapp för uppgifter](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md) och [Konfigurera [!UICONTROL Done] knapp för problem](../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

<!--
<img src="assets/marking-an-item-done-multiple-statuses-350x171.png" style="width: 350;height: 171;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
-->

### [!UICONTROL Done] knapp för artiklar som tilldelats flera resurser

När aktiviteten eller problemet tilldelas till mer än en resurs visas ordet **[!UICONTROL Done]** som följs av en nedrullningsbar meny. I listrutan kan du välja mellan **[!UICONTROL Done with my part]** (som talar om för teammedlemmarna att du är klar med din del av uppgiften), eller den status som är associerad med [!UICONTROL Done] -knapp (som slutför objektet). När du har valt **[!UICONTROL Done with my part]**, tas arbetsuppgiften bort från din arbetslista, men finns kvar i arbetslistan för de som fortfarande är tilldelade arbetsuppgiften.\
Om Klar-knappen är kopplad till flera statusar visas de under **Klar med min del**.

>[!NOTE]
>
>När det gäller en uppgift eller ett problem med flera tilldelningar är varje användare ansvarig för att ange att deras egen tilldelning av uppgiften eller utgåvan har slutförts. Därför måste varje tilldelad klicka [!UICONTROL Done] för att visa att de har slutfört det arbete som tilldelats dem för artikeln.

![](assets/marking-an-item-done-with-my-part-grop-by-drop-down-nwe-350x266.png)
