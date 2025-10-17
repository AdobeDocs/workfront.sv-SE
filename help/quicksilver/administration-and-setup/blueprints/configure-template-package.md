---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Konfigurera en utkast
description: Du kan konfigurera information om projektmallen eller organisationsstrukturen innan du installerar planen.
author: Jenny
feature: System Setup and Administration
role: Admin
exl-id: df10bc8f-b980-4c61-ae6d-bcea03103738
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1749'
ht-degree: 0%

---

# Konfigurera en plan

Du kan konfigurera information om en plan innan du installerar den. Plantyper för projektmallar och organisationsstrukturer kräver vanligtvis att vissa inställningar ställs in och att vissa egenskaper mappas. Andra typer av utkast kanske inte kräver konfiguration och du installerar dem som de är. Mer information om installation finns i [Installera en plan](/help/quicksilver/administration-and-setup/blueprints/blueprints-install.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Workfront-administratör </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera en projektmallsplan

1. Hitta den plan du vill använda.
1. Klicka på **[!UICONTROL Install]** och välj sedan en miljö:

   <table style="table-layout:auto">
        <tr>
        <td><strong>Produktion</strong></td>
        <td>Produktionen är er livemiljö.</td>
    </tr>
    <tr>
        <td><strong>Förhandsgranska sandlåda</strong></td>
        <td>Sandbox Preview är en testmiljö som fungerar som en kopia av din livemiljö och uppdateras varje helg av Workfront.</td>
    </tr>
    <tr>
        <td><strong>Sandbox 1 &amp; 2</strong></td>
        <td>Sandlådan för anpassad uppdatering är en separat testmiljö som uppdateras manuellt av dig. Det finns en extra kostnad för att hämta den anpassade uppdateringssandlådan.</td>
    </tr>
   </table>

1. Fortsätt med följande avsnitt:

   * [[!UICONTROL Template preferences]](#template-preferences)
   * [[!UICONTROL Role mapping]](#role-mapping)
   * [[!UICONTROL Team mapping]](#team-mapping)
   * [[!UICONTROL Company mappin]g](#company-mapping)
   * [[!UICONTROL Group mapping]](#group-mapping)

## [!UICONTROL Template preferences] {#template-preferences}

Välj hur du vill installera mallen.

Du kan också ange mallägandeskap innan du installerar ritningen. Du kan ändra de här fälten när mallen har installerats. Mer information finns i [Redigera projektmallar](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

![[!UICONTROL Template Preferences] avsnitt &#x200B;](assets/Blueprints_TemplatePreferences.png)

1. Ange ett nytt mallnamn i avsnittet [!UICONTROL Template Preferences].
1. Ange följande:

   <table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Template owner]<strong></td>
        <td>Den här personen får [!UICONTROL Manage] behörigheter i mallen och blir projektägare när mallen används för att skapa ett projekt.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Template sponsor]</strong></td>
        <td>Personen är vanligtvis en chef, en chef eller en intressent som behöver veta vad som händer med projektet. Projektsponsorn får ingen ytterligare åtkomst till projektet, men läggs till i e-postmeddelandena för projektet.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Portfolio]</strong></td>
        <td>Det här är portföljen som projektet hör till när det skapas.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Program]</strong></td>
        <td>Detta är det program som projektet hör till när det skapas.</td>
    </tr>
   </table>

1. Välj om mallen ska installeras som aktiv eller inaktiv.
1. Välj om du vill använda de definierade inställningarna för nya utgåvor, om det finns några inställningar.

   Klicka på **[!UICONTROL See issue preferences]** om du vill granska de inställningar som ska installeras med planen. Projekt som skapas från den importerade mallen använder de här inställningarna för nya utgåvor som läggs till i avsnittet [!UICONTROL Issues].

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Köa ämnesgrupper</strong></td> 
      <td> <p>Köämnesgrupper definierar den högsta nivån av kategorier för utgåvor och förfrågningar. Användarna visar ämnesgrupper som menyalternativ när de väljer var förfrågningar ska skickas. En ämnesgrupp kan innehålla flera köämnen. Mer information finns i <a href="../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Skapa ämnesgrupper</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Köämnen</strong></td> 
      <td> <p>Köämnen fungerar tillsammans med routningsregler för att tilldela ärenden eller förfrågningar. Det här är de menyalternativ som användarna väljer när de anger ett problem eller en förfrågan, efter att ha valt en ämnesgrupp. Mer information finns i <a href="../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Skapa köämnen</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Cirkulationsregler</strong></td> 
      <td>Routningsregler skickar ärenden eller förfrågningar till specifika jobbroller, användare eller team. De kan också skicka förfrågningar till specifika projekt, utöver det som är associerat med begärandekön. Mer information finns i <a href="../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Skapa routningsregler</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!INFO]
   >
   >**Exempel:** De nya utgåvsinställningarna i den här planen innehåller fyra köämnen. Användaren väljer ett av dessa ämnen när han/hon skapar ett problem. (Eftersom det bara finns en ämnesgrupp används den automatiskt och användaren behöver inte markera den.) När användaren har slutfört och skickat problemet avgör routningsreglerna vilken jobbroll eller vilket team det är tilldelat.
   >![Exempelinställningar för nya utgåvor](assets/Blueprints_IssuePrefsDetails.png)
   >![Köämnen för nya utgåvor](assets/blueprints-newissueqtopicsexample-350x204.png)
   >![Utfärdandet har vidarebefordrats till jobbrollen](assets/Blueprints_ProjectShowsIssueAssignment.png)

   >[!TIP]
   >
   >* Genom att använda inställningarna för problem kan du skapa ett konsekvent sätt att hantera nya utgåvor eller förfrågningar i dina projekt.
   >* När du anger de här inställningarna konverteras inte projekt som skapas från mallen automatiskt till begärandeköer. Mer information om hur du konfigurerar en begärandekö finns i [Skapa en begärandekö](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   >* Alla utkast innehåller inte nya inställningar för utgåvor.


## [!UICONTROL Role mapping] {#role-mapping}

>[!NOTE]
>
>Det här avsnittet kanske inte visas i vissa ritningar.

Vissa mallar innehåller förskrivna jobbroller. Med jobbroller kan du tilldela rätt personer när mallen konverteras till ett projekt. Du kan anpassa hur roller mappas innan du installerar ritningen. Klicka på **[!UICONTROL See role descriptions]** om du vill veta mer om de roller som är tillgängliga i planen.

Planen söker efter rollnamnet för att se om några befintliga roller matchar. Sökningen är skiftlägeskänslig, så namnen måste vara en exakt matchning. Om inga befintliga roller matchar kan du skapa dem i en plan.

![[!UICONTROL Role Mapping] avsnitt &#x200B;](assets/Blueprints_RoleMapping.png)

1. Om det finns en roll kan du välja något av följande alternativ:

   1. Skapa en ny roll med ett annat namn och skriv namnet i textrutan.
   1. Använd en befintlig roll och välj sedan en roll i valrutan.
   1. Använd inte mappad roll. Det här alternativet rekommenderas inte eftersom vissa uppgifter inte har tilldelats några roller.

1. Om en roll inte finns kan du välja något av följande alternativ:

   1. Skapa en ny roll. Med det här alternativet skapas rollen som modellen rekommenderar.
   1. Skapa en ny roll med ett annat namn och skriv namnet i textrutan.
   1. Använd en befintlig roll och välj sedan en roll i valrutan.
   1. Använd inte mappad roll. Det här alternativet rekommenderas inte eftersom vissa uppgifter inte har tilldelats några roller.

>[!NOTE]
>
>Installationsprocessen använder inte roller för specifika personer. Du bör verifiera personerna i dessa roller efter att du har installerat lösningen för utkast och tilldela personer om det behövs. Mer information finns i [Åtgärder som ska vidtas efter att en plan har installerats](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Mer information om jobbroller i [!DNL Workfront] finns i [Skapa och hantera jobbroller](../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## [!UICONTROL Team mapping] {#team-mapping}

>[!NOTE]
>
>Det här avsnittet kanske inte visas i vissa ritningar.

Vissa mallar innehåller förskrivna team. Arbetet som tilldelats ett team kan utföras av alla medlemmar i teamet. Du kan anpassa hur team mappas innan du installerar planen. Klicka på **[!UICONTROL See team descriptions]** om du vill veta mer om vilka team som finns tillgängliga i planen.

Planen söker efter teamets namn för att se om några befintliga team matchar. Sökningen är skiftlägeskänslig, så namnen måste vara en exakt matchning. Om inga befintliga team matchar kan du skapa dem i en plan.

![[!UICONTROL Team Mapping] avsnitt &#x200B;](assets/Blueprints_TeamMapping.png)

1. Om ett team finns kan du välja något av följande alternativ:

   1. Skapa ett nytt team med ett annat namn och skriv namnet i textrutan.
   1. Använd [!UICONTROL existing team] och välj sedan ett team i valrutan.
   1. Använd inte mappat team. Det här alternativet rekommenderas inte eftersom vissa uppgifter inte har tilldelats några team.

1. Om ett team inte finns kan du välja något av följande alternativ:

   1. Skapa ett nytt team. Med det här alternativet skapas teamet som vi rekommenderar.
   1. Skapa ett nytt team med ett annat namn och skriv namnet i textrutan.
   1. Använd [!UICONTROL existing team] och välj sedan ett team i valrutan.
   1. Använd inte mappat team. Det här alternativet rekommenderas inte eftersom vissa uppgifter inte har tilldelats några team.

>[!NOTE]
>
>Installationsprocessen lägger inte till personer i teamen. Du bör verifiera personerna i teamet efter att du har installerat lösningen för utkast och tilldela personer om det behövs. Mer information finns i [Åtgärder som ska vidtas efter att en plan har installerats](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Mer information om hur team fungerar i [!DNL Workfront] finns i [Skapa och hantera team](../../people-teams-and-groups/create-and-manage-teams/create-and-mange-teams.md).

## Företagsmappning {#company-mapping}

>[!NOTE]
>
>Det här avsnittet kanske inte visas i vissa ritningar.

Vissa ritningar innehåller förskrivna företag. Ett företag är en organisationsenhet som kan representera din organisation, en avdelning inom organisationen eller en kund som du arbetar med. Du kan anpassa hur företag mappas innan du installerar ritningen. Klicka på **[!UICONTROL See company descriptions]** om du vill veta mer om de företag som finns i planen.

Planen söker efter företagsnamnet för att se om några befintliga företag matchar. Sökningen är skiftlägeskänslig, så namnen måste vara en exakt matchning. Om inga befintliga företag matchar kan du skapa en plan för dem. Det primära företaget i planen mappas till det primära företaget i din miljö, även om de inte har samma namn.

![[!UICONTROL Company Mapping] avsnitt &#x200B;](assets/Blueprints_CompanyMapping.png)

1. Om det finns ett företag kan du välja något av följande alternativ:

   1. Skapa ett nytt företag med ett annat namn och skriv namnet i textrutan.
   1. Använd ett befintligt företag och välj sedan ett företag i valrutan.\

      Det primära företaget i planen mappas till det primära företaget i din miljö, även om de inte har samma namn.
   1. Använd inte mappat företag. Det här alternativet rekommenderas inte eftersom företagsreferenserna i andra objekt kommer att vara tomma.

1. Om ett företag inte finns kan du välja något av följande alternativ:

   1. Skapa ett nytt företag. Med det här alternativet skapas det företag som planen rekommenderar.
   1. Skapa ett nytt företag med ett annat namn och skriv namnet i textrutan.
   1. Använd ett befintligt företag och välj sedan ett företag i valrutan.
   1. Använd inte mappat företag. Det här alternativet rekommenderas inte eftersom företagsreferenserna i andra objekt kommer att vara tomma.

>[!NOTE]
>
>Mer information om hur du konfigurerar företagen efter att du har installerat ritningen finns i [Åtgärder som ska vidtas efter att en plan har installerats](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Mer information om hur du associerar en mall med ett företag finns i [Redigera projektmallar](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Mer information om hur företag fungerar i [!DNL Workfront] finns i [Skapa och redigera företag](../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## [!UICONTROL Group mapping] {#group-mapping}

>[!NOTE]
>
>Det här avsnittet kanske inte visas i vissa ritningar.

Vissa utkast innehåller förskrivna grupper. En grupp är en grupp användare som sammanfaller med avdelningsstrukturen. Grupper liknar, men skiljer sig från, team och företag i Workfront. Du kan anpassa hur grupper mappas innan du installerar ritningen. Klicka på **[!UICONTROL See group descriptions]** om du vill veta mer om de grupper som är tillgängliga i planen.

Planen söker efter gruppnamnet för att se om några befintliga grupper matchar. Sökningen är skiftlägeskänslig, så namnen måste vara en exakt matchning. Om inga befintliga grupper matchar kan du skapa dem i planen.

![[!UICONTROL Group Mapping] avsnitt &#x200B;](assets/Blueprints_GroupMapping.png)

1. Om det finns en grupp kan du markera **[!UICONTROL Remap Group]** och välja något av följande alternativ:

   1. **[!UICONTROL Create a new group with a different name]** och skriv sedan det namn som ska tilldelas den här gruppen. Referenser till gruppen i definitionen av utkast kopplas i stället till den nya gruppen.
   1. **[!UICONTROL Replace with an existing group]**, sök efter och markera en grupp i markeringsrutan.

      >[!NOTE]
      >
      >Du kan inte byta namn på en befintlig grupp.

1. Om en grupp inte finns kan du:

   1. Ändra det föreslagna gruppnamnet genom att skriva det i textrutan.
   1. Markera **[!UICONTROL Remap Group]** och välj [!UICONTROL Replace with an existing group]. Sök efter och markera sedan en grupp i markeringsrutan.
   1. Markera **[!UICONTROL Remap Group]** och välj **[!UICONTROL Insert under an existing group]**. Sök efter och markera sedan en grupp i markeringsrutan. Med det här alternativet skapas en ny undergrupp under den befintliga gruppen.

>[!NOTE]
>
>Information om hur du konfigurerar grupperna efter att du har installerat ritningen finns i [Åtgärder som ska vidtas efter att du har installerat en ritning](../../administration-and-setup/blueprints/best-next-actions-after-install.md).

Mer information om hur du använder grupper i [!DNL Workfront] finns i [Översikt över grupper](../../administration-and-setup/manage-groups/groups-overview/groups.md).
