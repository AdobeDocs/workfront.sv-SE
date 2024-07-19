---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Dela ett korrektur i Adobe Workfront
description: Du kan dela korrekturdokument i Adobe Workfront genom att dela dokumentet eller genom att lägga till användare i korrekturet.
author: Courtney
feature: Digital Content and Documents
exl-id: a5438db3-6507-4ebc-a27c-65f02c45783e
source-git-commit: 5c0cd18074cffdf0a4fe15affaf61add7314a83a
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# Dela ett korrektur i Adobe Workfront

Du kan dela korrekturdokument i Adobe Workfront genom att dela dokumentet eller genom att lägga till användare i korrekturet.

Om du delar korrekturet, enligt beskrivningen i den här artikeln, har mottagaren samma åtkomst till dokumentet och korrekturet. Dessutom kan du begära godkännande av korrekturet från mottagaren.

>[!TIP]
>
>Du kan också dela ett korrektur inifrån korrekturläsaren. Instruktioner finns i [Dela ett korrektur från korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Korrekturroll</td> 
   <td>Författare eller moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

## Dela en korrekturlänk

Genom att dela en korrekturlänk får Workfront-användare åtkomst. Användare kan kommentera korrekturet och prenumerera på e-postmeddelanden för korrekturet med hjälp av inloggningsuppgifterna för Workfront. Användare som inte är språksäkra kan kommentera och prenumerera med hjälp av en e-postadress och ett visningsnamn.

>[!IMPORTANT]
>
>Inställningen Tillåt delning av korrektur via offentlig URL eller inbäddningskod måste vara aktiverad.

1. Markera det dokument som innehåller det korrektur som du vill dela med användarna.

   Du kan bara markera ett dokument. Du kan inte dela länken för flera dokument samtidigt.

1. Klicka på **Dela** > **Korrekturlänk**.
1. Gör något av följande i rutan **Korrekturlänk** som visas:

   * Om du vill kopiera länken till Urklipp klickar du på **Kopiera länk**.

     Nu kan du distribuera länken via ett verktyg från tredje part, som en chatt eller ett e-postprogram.

   * Så här skickar du länken direkt från Adobe Workfront:

      1. I fältet **Eller e-postlänk till** börjar du skriva och väljer namnet på mottagaren. Eller ange e-postadressen till en extern användare som du vill dela med.

         >[!NOTE]
         >
         >Om du ser ett alias-e-postmeddelande när du delar ett korrektur ska du inte skapa en ny gästanvändare genom att ange det ursprungliga e-postmeddelandet om det finns ett motsvarande alias-e-postmeddelande.

      1. Välj bland följande alternativ:

         <table style="table-layout:auto">
          <col>
          <col>
          <tbody>
           <tr>
            <td role="rowheader">Skicka offentlig länk</td>
            <td><p>Inkluderar en knapp i e-postmeddelandet som dirigerar användare till korrekturet i det korrekturläsare som de använder och beviljar visningsåtkomst.</p><p>Om <strong>Prenumerera på korrektur via offentlig URL eller inbäddningskod</strong> är inaktiverat för korrekturet kan användare logga in med sina inloggningsuppgifter för Workfront för att lägga till kommentarer i korrekturet. Om det är aktiverat kan alla som anger sin e-postadress och sitt namn (inget lösenord krävs) signera och lägga till kommentarer i korrekturet.</p></td>
           </tr>
           <tr>
            <td role="rowheader">Skicka nedladdningslänk</td>
            <td>Innehåller en knapp i e-postmeddelandet som dirigerar användare till en hämtningssida med filinformation, filnamn och filstorlek, med filen textbunden. Användarna kan klicka på länken Hämta på nedladdningssidan för att hämta filen.</td>
           </tr>
           <tr>
            <td role="rowheader">Lägg till anpassat meddelande</td>
            <td>Gör att du kan ange ett eget ämne och brödtext för e-postmeddelandet.</td>
           </tr>
          </tbody>
         </table>

      1. Klicka på **Skicka**.

         Mottagarna får ett e-postmeddelande med information om det korrektur och de knappar du valt att inkludera.

         ![](assets/proof-share-email-350x87.png)

## Lägga till användare i ett korrektur

Du kan lägga till valfri Workfront-användare i korrekturet om du har redigeringsbehörighet för korrekturet. Om korrekturet har flera steg lägger du till användaren i en enskild fas

>[!WARNING]
>
>Förutom de metoder som anges i den här artikeln kan du lägga till användare i ett korrektur genom att tagga dem i en kommentar från fliken Uppdateringar i ett befintligt korrektur. Användare som läggs till i ett korrektur på det här sättet får dock inte ett e-postmeddelande om de inte taggas igen efter att de har lagts till i korrekturets arbetsflöde.
>
>Därför rekommenderar vi att du lägger till användare i ett korrektur på något av följande sätt och inte genom att tagga dem i en kommentar.
>

>[!NOTE]
>
>Tänk på följande om du använder en äldre Workfront-plan där korrektur kan aktiveras och inaktiveras för en användare:
>
>* Mottagarna behöver inte ha språkkontroll aktiverat för att kunna granska korrekturet.
>* När Automatiserat arbetsflöde är aktiverat och du lägger till en användare till korrekturet som inte har språkkontroll aktiverat i Workfront, skapas en ny fas i det automatiserade arbetsflödet. Användaren som du lägger till läggs automatiskt till på den nya scenen när han/hon visar korrekturet för första gången. (Mer information finns i [Översikt över automatiserat arbetsflöde](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).)
>

### Lägga till användare i ett befintligt korrektur från fliken Dokument

1. Markera dokumentet som innehåller det korrektur som du vill lägga till användare i.
1. Om korrekturet inte har ett automatiskt arbetsflöde (steg) klickar du på ikonen **Mer** i det övre högra hörnet av scenen 1 och sedan på **Dela** i listrutan.

   eller

   Om korrekturet har ett automatiserat arbetsflöde klickar du på ikonen **Mer** i det övre högra hörnet av scenen där du vill lägga till granskaren. Klicka sedan på **Dela** i listrutan.

1. I rutan **Dela den här versionen** som visas, under **Dela**, börjar du skriva namnet eller e-postadressen till en användare som du vill dela korrekturet med och klickar sedan på namnet som visas i listrutan.

1. (Valfritt) Upprepa det här steget om du vill lägga till flera användare till korrekturet.
1. (Valfritt) Ange en deadline för granskarna.
1. (Valfritt) Kontrollera att **Meddela personer via e-post** är markerat om du vill att granskarna ska veta att du har lagt till dem i korrekturet.
1. (Valfritt) **Lägg till ett anpassat meddelande** i e-postmeddelandet.
1. När du har lagt till alla granskare klickar du på **Dela**.

### Lägga till användare i ett befintligt korrektur från korrekturläsaren

Du kan lägga till användare i ett korrektur när du granskar ett korrektur i Web Proofing Viewer och i Desktop Proofing Viewer.

Mer information finns i [Dela ett korrektur genom att lägga till användare](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users) i artikeln [Dela ett korrektur från korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)

## Rapport om korrekturgodkännanden

Du kan skapa en rapport som rapporterar om korrekturgodkännanden som har delats inom Workfront. Den här rapporten innehåller följande bevis för godkännande i ditt system:

* Dokument som har skickats för godkännande
* Godkännarens namn
* Korrekturversion
* Korrektur-ID
* Datum för korrekturskapande

Du får åtkomst till det här godkännandet när du skapar en rapport baserad på ett objekt, vilket beskrivs i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Mer information om objektrapporten för korrekturgodkännanden finns i avsnittet [Rapport om objekt](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) i [Förstå objekt i Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)

## Godkänn ett delat korrektur

När en användare lägger till dig i ett korrektur och beviljar rollen Godkännare eller rollen Granskare och godkännare med hjälp av automatiserat arbetsflöde, visas godkännandebegäran på fliken Godkännanden i Hem eller Min arbetsyta. Sedan kan du titta på beviset och godkänna det direkt från Workfront.

Mer information om hur du fattar beslut om godkännande på arbetsytan Mitt arbete finns i [Godkänn arbete på startsidan](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-home-area) eller [Godkänna arbete](../../../review-and-approve-work/manage-approvals/approving-work.md#approving-work-from-the-my-work-area) i [Godkänna arbete](../../../review-and-approve-work/manage-approvals/approving-work.md).
