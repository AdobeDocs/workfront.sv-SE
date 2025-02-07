---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Hantera tillgängliga licenser i systemet
description: Som Adobe Workfront-administratör har du tillgång till information om ditt Workfront-konto, inklusive antalet licenser som köpts för din organisation, samt antalet licenser som används för närvarande.
author: Lisa, Becky
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '1216'
ht-degree: 0%

---

# Hantera tillgängliga licenser i ditt system

<!-- Audited: 12/2023 -->

Som Adobe Workfront-administratör har du tillgång till information om ditt Workfront-konto, inklusive antalet licenser som köpts för din organisation, samt antalet licenser som används för närvarande.

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
   <td>
    <p>Nytt: Standard</p>
    <p>eller</p>
    <p>Aktuell: Planera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara systemadministratör eller gruppadministratör. Gruppadministratören har en begränsad vy över licensinformationen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

>[!NOTE]
>
>Följande programsatser gäller endast för nya planer.
>
>För Select-planen:
>
>1. Systemadministratörer kan inte ange gränser för hemgrupper.
>2. Systemadministratörer kan endast se det totala antalet licenser som används i alla hemgrupper.
>3. Gruppadministratörer har inte tillgång till licenssidan alls.
>
>För Prime och Ultimate:
>
>1. Systemadministratörer kan lägga till hemgrupper på sidan Licenser för att visa användningen av licenser i dessa grupper, och de kan också ange licensbegränsningar.
>2. Gruppadministratörer har tillgång till sidan Licenser och kan visa hur licenserna i de grupper de hanterar har utnyttjats och som har lagts till på sidan Licenser av systemadministratörer.
>3. Gruppadministratörer kan inte visa information för andra hemgrupper eller lägga till maximumvärden.

+++

## Visa organisationens licenser

Antalet licenser som används uppdateras automatiskt när du tilldelar åtkomstnivåer till användare som du lägger till i Workfront. Mer information finns i [Lägg till användare](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Så här visar du licensinformation i ditt system:

{{step-1-to-setup}}

1. Klicka på **System** > **Licenser** längst ned på den vänstra panelen.

   Mer information om licenserna på den här sidan finns i [Licensöversikt](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Korrekturlicenser är endast tillgängliga för kunder som har köpt det betalda Workfront Proof-tillägget utöver sin Workfront-licens. Mer information om det här tillägget finns i [Workfront Proof: artikelindex](../../workfront-proof/workfront-proof.md).

1. (Villkorligt) Om du ser meddelandet **Om du vill ange ett maximum måste du lägga till en hemgrupp**, lägga till en hemgrupp i systemet enligt anvisningarna i avsnittet [Lägg till eller ta bort en hemgrupp på sidan Licenser](#add-or-remove-a-home-group-to-the-licenses-page) i den här artikeln.

   >[!NOTE]
   >
   >För de nya planerna tillåter Select-planen inte att administratörer visar licenser per hemgrupp. Du kan bara se det totala antalet använda licenser. Med Prime- och Ultimate-planerna kan du ange maximalt antal licenser per hemgrupp.

## Visa information om licenser för Workfront-tillägg

Om ditt företag har det betalda Workfront Proof-tillägget visas antalet använda licenser och antalet tillgängliga licenser. Till exempel visar **5 av 10 korrekturlicenser** att organisationen för närvarande använder 5 av de 10 Workfront Proof-licenser som de har köpt.

![Licens för Workfront-tillägg](assets/updated-licenses-page.png)

Om din organisation har köpt Workfront-mål visas även licensinformationen för den här produkten här. I så fall kan du visa följande information:

* Det totala antalet Workfront Goals-licenser som ditt företag har köpt
* Antalet Workfront Goals-licenser som är kopplade till användare. Det här är antalet användare som ska ha beviljat minst Visa åtkomst till mål på åtkomstnivå.

Mer information om Workfront-mål finns i [Översikt över Adobe Workfront-mål](../../workfront-goals/goal-management/wf-goals-overview.md). Mer information om åtkomst till Workfront-mål finns i [Bevilja åtkomst till Adobe Workfront-mål](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

>[!NOTE]
>
>Med Workfront kan du tilldela fler licenser för Workfront Goals som du har köpt. Om du tilldelar fler licenser än vad som tillåts enligt Workfront Goals-avtalet kontaktar en Workfront-kontoansvarig dig för att tala om att du har överskridit ditt avtalsnummer.
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>Användare utan administrativ åtkomst kan använda en grupprapport för att visa licensantal. Skapa en ny grupprapport på fliken Rapport och lägg till följande kolumner:
>
>* Begränsning av licenstyp: Worker-gräns
>* Gräns för licenstyp: Planeringsgräns
>
>Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Visa information om månatliga korrektur- och dokumentavrop

>[!IMPORTANT]
>
>Gränserna för korrektur och dokumentbeslut gäller endast användare av de nya licenserna. Mer information finns i [Översikt över nya licenser](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

Handläggningsbeslut och dokumentbeslut är begränsade för alla obetalda Workfront-licenser. Begränsningar som återställs per användare och månad.

Beslutsgränsen för respektive licens varierar beroende på vilken plan du har. Du kan visa din månadstilldelning i Inställningar > Licenser.

Mer information om beslutsgränser för korrektur och dokument finns i [Översikt över begränsade dokument och korrekturrundor för obetalda användare](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![Månadsvis beslutstilldelning](assets/monthly-decision-allotment.png)

## Lägga till eller ta bort en hemgrupp på sidan Licenser {#add-or-remove-a-home-group-to-the-licenses-page}

<!--A Business or Enterprise Workfront Plan is required to use this feature. For more information about the various plans available, see [Workfront Plans.](https://www.workfront.com/plans)-->

Varje användare kan endast tilldelas en hemgrupp. Workfront tillhandahåller ett grupporienterat licensantal genom att beräkna hur många licenser som tilldelas och används i respektive hemgrupp.

Om du ser meddelandet **Om du vill ange ett maxvärde måste du lägga till en hemgrupp** på sidan Licenser. Du måste lägga till minst en hemgrupp på sidan Licenser.

>[!IMPORTANT]
>
>* För att effektivt hantera licenser med hemgrupper rekommenderar vi att du skapar specifika hemgrupper för affärsenheter innan du uppdaterar det högsta antalet licenser. Mer information finns i [Översikt över hemgrupper](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* Du kan bara lägga till grupper på den översta nivån som hemgrupper, inte undergrupper. Om en användare har en undergrupp tilldelad som sin hemgrupp läggs hans/hennes licens till i antalet licenser för den översta gruppen ovanför den undergruppen.
>

Så här lägger du till eller tar bort en hemgrupp på sidan Licenser:

{{step-1-to-setup}}

1. Klicka på **System** > **Licenser** längst ned på den vänstra panelen.

1. Klicka på **Hantera grupplista**.
1. Börja skriva gruppnamnet på den översta nivån i rutan **Hemgrupper**.
1. Om du vill lägga till gruppen klickar du på dess namn när den visas.

   eller

   Om du vill ta bort gruppen klickar du på X-ikonen till höger om dess namn.

1. Klicka på **Spara**.

Som Workfront-administratör kan du ange högsta antal licenser för hemgrupperna för att förhindra att en affärsenhet använder Workfront-licenser som köpts för andra affärsenheter. Instruktioner finns i [Ange maximalt antal licenser för en hemgrupp](#set-the-maximum-license-count-for-a-home-group) i den här artikeln.

## Ange högsta antal licenser för en hemgrupp {#set-the-maximum-license-count-for-a-home-group}

Som Workfront-administratör kan du ange högsta antal licenser för de översta hemgrupperna i ditt system. På så sätt kan ni förhindra att en affärsenhet använder Workfront-licenser som köpts för andra affärsenheter inom organisationen.

Som standard är det högsta antalet licenser inställt på Ej tillämpligt, vilket innebär att det inte finns någon gräns.

Gruppadministratörer kan visa antalet licenser som tilldelats och använts i en hemgrupp som de hanterar. Mer information finns i [Visa antalet licenser som allokerats och använts i en grupp](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

Så här anger du det maximala antalet licenser för en hemgrupp:

{{step-1-to-setup}}

1. Klicka på **System** > **Licenser** längst ned på den vänstra panelen.

1. Leta reda på hemgruppen i listan.
1. I kolumnen **Max** i gruppen klickar du på det värde som du vill ange ett maxvärde för.
1. Ange det maximala antalet och tryck sedan på Retur.

   ![Maximalt antal licenser för gruppen](assets/updated-max.png)

   >[!NOTE]
   >
   >Ange inte 0 om du vill återställa en grupps maximala licensvärde till standardvärdet. Ta i stället bort numret i rutan. Om det maximala licensvärdet anges till 0 betyder det att det inte finns några tilldelade licenser för den gruppen.
