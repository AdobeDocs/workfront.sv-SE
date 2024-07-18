---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Exempel på beräknat anpassat fält: visa hanteraren för den som har skapat ett ärende i det anpassade formuläret"
description: Med hjälp av ett beräknat anpassat fält kan du visa namnet på den som har skapat ett ärende i ett anpassat formulär som har kopplats till problemet. Med samma programsats kan du skapa liknande beräkningsfält för projekt, utgåvor och andra objekt.
author: Nolan
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '413'
ht-degree: 0%

---

# Exempel på beräknat anpassat fält: visa hanteraren för den som skapat ett ärende i det anpassade formuläret

Med hjälp av ett beräknat anpassat fält kan du visa namnet på den som har skapat ett ärende i ett anpassat formulär som har kopplats till problemet. Med samma programsats kan du skapa liknande beräkningsfält för projekt, utgåvor och andra objekt.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-licens*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär<br>Mer information om att bevilja administrativ åtkomst från åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Bevilja användare administrativ åtkomst till vissa områden</a>.</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektbehörigheter</p> </td> 
   <td> <p>Contribute-åtkomst till det objekt som formuläret är kopplat till har åtkomst till Redigera det anpassade formuläret</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa den som har skapat ett ärende i det anpassade formuläret

I följande steg visas hur du kan skapa ett beräkningsfält för ett eget ärende där du kan hämta namnet på hanteraren för den användare som skapade problemet. Processen är identisk när du vill hämta namnet på den ansvarige för en användare som har skapat en uppgift, ett projekt eller en portfölj, till exempel.

1. Skapa ett eget utgivningsformulär och lägg till ett beräknat fält i det.

   Mer information om hur du skapar ett anpassat formulär och lägger till beräknade fält i det finns i följande artiklar:

   * [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [Lägga till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. Kopiera och klistra in följande textlägeskod i fältet **Beräkning** i det anpassade formuläret:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Anpassade fältberäkningar är skiftlägeskänsliga.

1. Klicka på **Klar** och sedan på **Spara + stäng**.

   Hanteraren för den användare som skapade problemet visas i beräkningsfältet när formuläret som innehåller fältet är kopplat till ett problem.
