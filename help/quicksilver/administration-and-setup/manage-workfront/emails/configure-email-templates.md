---
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: emails-administration
title: Konfigurera e-postmallar
description: Som Adobe Workfront-administratör kan du konfigurera e-postmallar som har stöd för påminnelsemeddelanden.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2ebc3be5-2734-4012-9277-86176c070137
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 0%

---

# Konfigurera e-postmallar

Som Adobe Workfront-administratör kan du konfigurera e-postmallar som har stöd för påminnelsemeddelanden.

E-postmallar innehåller meddelandet som skickas till användarna när ett påminnelsemeddelande initieras.\
Utan en e-postmall levereras påminnelsemeddelandet som tomt innehåll i e-postmeddelandets brödtext.

E-postmallar kan associeras med påminnelsemeddelanden för problem, uppgifter, projekt och tidrapporter. När du skapar e-postmallar kan Workfront-administratören tillhandahålla innehåll för e-postmeddelandet och en ämnesrad.

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
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td><p>Aktuell: Planera</p>
   eller
   <p>Nytt: Standard</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivåkonfiguration</td> 
   <td> <p>Systemadministratör</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information om åtkomstkrav finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en e-postmall {#create-an-email-template}

{{step-1-to-setup}}

1. Klicka på **E-post** > **Meddelanden**> **E-postmallar** i den vänstra panelen.

   ![](assets/email-templates-tab-under-setup-email-notifications-area.png)

1. Klicka på **Ny e-postmall**.

1. Ange följande information i rutan **Ny e-postmall**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td>Lägg till en rubrik för e-postmallen. Detta är ett obligatoriskt fält.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Objekttyp</td> 
      <td>Ange den objekttyp som du vill associera mallen med. Välj bland följande objekt:
      <ul>
      <li>Projekt</li>
      <li>Uppgift</li>
      <li>Problem</li>
      <li>Tidrapport</li> </ul>

   Detta är ett obligatoriskt fält och det är som standard inställt på Projekt.</td>
   </tr>
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Lägg till mer information om e-postmallen, dess syfte och avsedd målgrupp.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Ämne </td> 
      <td>Lägg till texten som visas på ärenderaden i e-postmeddelandet när e-postmeddelandet som genereras av mallen skickas. Detta är ett obligatoriskt fält.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Brödtext </td> 
      <td> <p>Lägg till texten för e-postmeddelandets innehåll.</p> <p>Du kan använda HTML-formatering för e-postinnehållet, vilket beskrivs i avsnittet <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">Lägg till HTML i en e-postmall</a> i den här artikeln.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Spara**.

## Lägga till HTML-formatering i en e-postmall {#add-html-formatting-to-an-email-template}

Du kan lägga till HTML-taggar i e-postmallar för att skapa anpassade meddelanden.\
Börja skapa e-postmallen enligt beskrivningen i [Skapa en ny e-postmall](#create-a-new-email-template).

HTML kan förbättra e-postmallarna, vilket visas i följande avsnitt.

* [Länka till Workfront-objekt](#link-to-workfront-objects)
* [Länka till anpassade fält med HTML](#link-to-custom-fields-with-html)
* [HTML e-postexempel](#html-email-examples)

### Länka till Workfront-objekt {#link-to-workfront-objects}

Du kan inkludera länkar till Workfront-fält genom att använda jokertecknet `$$` för att tala om för e-postgeneratorn att söka efter värden från databasen som är associerad med ett visst objekt.

Innehållet i e-postmeddelandet för ett meddelande som varnar den som tilldelats uppgiften att uppgiften ska starta kan följa den här strukturen:

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b><strong>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td></tr>
</table>
</html>
```

Om du vill hämta jokertecknet för ett objekt gör du något av följande:

* Gå till API-utforskaren och välj namnen på objekten på fliken Fält för ett objekt. Mer information om API-utforskaren finns i [API-utforskaren](/help/quicksilver/wf-api/general/api-explorer.md).

* Använd det `valuefield`-värde som du hittar i en rapportvy i textläge. Mer information om värden för textläge finns i [Översikt över textläge](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Värdet `heading` kan vara objektets namn, så som du vill att det ska visas i e-postbrödtexten.

### Länka till anpassade fält med HTML {#link-to-custom-fields-with-html}

Du kan inkludera länkar till användare och anpassade fält genom att använda jokertecknet `$$` för att tala om för e-postgeneratorn att söka efter värden från den databas som är associerad med objektet. De måste finnas på båda sidor om databasattributreferensen.

Om du till exempel lägger till följande text som HTML skulle den tilldelade användarens förnamn läggas till i påminnelsemeddelandet som är kopplat till en uppgift:

`assignedTo:firstName`

Om du vill lägga till anpassade fält med samma formatering kan du lägga till följande i e-postmeddelandet:

`DE:Custom Field As It Appears in Workfront`

Det här är till exempel en e-postmall som innehåller en referens till ett anpassat fält med namnet Leveransdatum, och det förutsätts att fältet Leveransdatum tillhör en uppgift.

Ersätt `<your domain>` med ditt företags Workfront-domän, utan hakparenteser:

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which has a Delivery Date of $$DE:Task:Delivery Date$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
<tr>
<td><b>Description:</b></td>
<td>$$description$$</td>
<tr>
<td><b>Estimated Effort:</b></td>
<td>$$work$$ hours</td>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
<td><b>Delivery Date:</b></td>
<td>$$DE:Task:Delivery Date$$</td>
</tr>
</table>
</html>
```

>[!NOTE]
>
>Om fältet tillhör ett projekt ersätter du aktiviteten med projektet:
>
>`DE:Project:Delivery Date`

### HTML e-postexempel {#html-email-examples}

* [Påminnelsemeddelande för sent projekt (exempel)](#late-project-reminder-notification-example)
* [Påminnelse om aktivitet eller problem att starta (exempel)](#task-or-issue-about-to-start-reminder-example)

#### Påminnelsemeddelande för sent projekt (exempel) {#late-project-reminder-notification-example}

Om du vill redigera en e-postmall för en påminnelse om ett sent projekt bör du ta hänsyn till den här informationen för fälten Ämne och Innehåll.

Ersätt `<your domain>` med ditt företags Workfront-domän, utan hakparenteser.

**Ämne:**

Ett projekt som du hanterar har blivit försenat

**Innehåll:**

```html
<html>
<p>The <b><a href="https://<your domain>.my.workfront.com/project/view?ID=$$ID$$">$$name$$</a></b> project you are assigned as the owner of just became late.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
</tr>
</table>
<p>Please review the task plan and bring it up to date to reflect the progress made so far. If it is necessary to update the plan to bring it reflect reality going forward, be sure to speak to $$sponsor:name$$ for approval before make these changes to the work breakdown structure.</p>
</html>
```

Detta skapar ett e-postmeddelande som liknar följande:

![](assets/project-became-late-email.png)

#### Påminnelse om aktivitet eller problem att starta {#task-or-issue-about-to-start-reminder-example}

Du kan också skapa en påminnelseavisering för en kommande uppgift eller ett kommande problem.

Följande kod kan inkluderas i en e-postmall som används för uppgifter och för att skicka påminnelsemeddelanden som skickas ett valfritt antal dagar före det planerade startdatumet för uppgiften eller utgåvan.

Ersätt `<your domain>` med ditt företags Workfront-domän, utan hakparenteser.

Om du vill använda det här för ett e-postmeddelande för ett problem ändrar du värdet `/task/view.` i länken till arbetsobjektet till `/issue/view`.

**Ämne:**

`$$name$$ to start on $$plannedStartDate$$`

**Innehåll:**

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><ahref=https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<tablewidth=350"style=font-size:12px;">
<tr>
<td><b>Task Name:</b></td>
<td>$$name$$</td>
</tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<td><b>Created on:</b></td>
<td>$$entryDate$$</td>
</tr>
<tr>
<td><b>Project Manager:</b></td>
<td>$$project:owner:name$$</td>
<tr>
<td><b>Priority:</b></td>
<td>$$priority$$</td>
</tr>
<tr>
<td><b>Who is assigned to:</b></td>
<td>$$assignedTo:name$$</td>
</tr>
<tr>
<td><b>When it's due:</b></td>
<td>$$estCompletionDate$$</td>
</tr>
</table>
</html>
```

![email_template_delivery.png](assets/email-template-delivered.png)

När en e-postmall har skapats kan användare associera den med påminnelsemeddelanden, vilket beskrivs i [Konfigurera påminnelsemeddelanden](../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
