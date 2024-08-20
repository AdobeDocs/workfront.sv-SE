---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Konfigurera korrekturinställningar för din organisation
description: Som Adobe Workfront-administratör eller Workfront Proof-administratör kan du anpassa korrekturinställningarna för din organisation. De här inställningarna innehåller standarddelningsalternativ, branding med mera.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 29405172-c3dd-431f-a242-fd38b53a307d
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '1221'
ht-degree: 0%

---

# Konfigurera korrekturinställningar för din organisation

Som Adobe Workfront-administratör eller Workfront Proof-administratör kan du anpassa korrekturinställningarna för din organisation. De här inställningarna innehåller standarddelningsalternativ, branding med mera.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Premium eller Select</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administratör måste väljas i din behörighetsprofil för korrektur. Mer information finns i <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Konfigurera en användares språkkontroll</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

+++

## Konfigurera åtgärder

Mer information om hur du använder åtgärder i korrekturläsaren finns i [Använda åtgärder på korrekturkommentarer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md).

Du kan konfigurera åtgärder för din organisation på följande sätt:

* [Lägg till eller byta namn på en åtgärd](#add-or-rename-an-action)
* [Inaktivera eller återaktivera en åtgärd](#deactivate-or-reactivate-an-action)
* [Ordna om funktionsmakron](#reorder-actions)

### Lägga till eller byta namn på en åtgärd {#add-or-rename-an-action}

{{step1-to-proofing}}

1. Klicka på **Inställningar** > **Kontoinställningar** i det övre högra hörnet av Workfront Proof-gränssnittet och klicka sedan på fliken **Inställningar** .

1. Gör något av följande:

   * Om du vill skapa en ny åtgärd klickar du på **Ny åtgärd** i avsnittet **Åtgärder**.

     Det finns ingen gräns för hur många åtgärder du kan konfigurera på ditt konto.

   * Om du vill byta namn på en befintlig åtgärd klickar du på **Inställningar** bredvid åtgärden.

1. Skriv ett namn för åtgärden och klicka sedan på **Spara**.
1. Klicka på **Spara.**

### Inaktivera eller återaktivera en åtgärd {#deactivate-or-reactivate-an-action}

{{step1-to-proofing}}

1. Klicka på **Inställningar** > **Kontoinställningar** i det övre högra hörnet av Workfront Proof-gränssnittet och klicka sedan på fliken **Inställningar** .

1. Klicka på **Konfigurera** bredvid den åtgärd som du vill inaktivera eller återaktivera.
1. Välj **Aktivera** eller **Inaktivera** och klicka sedan på **Spara**.

### Ordna om funktionsmakron {#reorder-actions}

{{step1-to-proofing}}

1. Klicka på **Inställningar** > **Kontoinställningar** i det övre högra hörnet av Workfront Proof-gränssnittet och klicka sedan på fliken **Inställningar** .

1. Klicka på den blå upp- och nedpilen bredvid **Inställningar** för att ordna om åtgärderna.

   ![Ändra ordning_åtgärder.png](assets/re-order-actions-350x103.png)

## Konfigurera anpassade enheter för korrektur

Du kan lägga till anpassade enheter i systemet, så att användarna kan granska interaktivt innehåll och simulera hur innehållet ser ut på en viss enhet.

Mer information om hur användare kan välja enheter när de granskar interaktivt innehåll finns i [Ändra interaktiv korrekturupplösning i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)

Så här lägger du till en anpassad enhet:

{{step1-to-proofing}}

1. Klicka på **Inställningar** > **Kontoinställningar** i det övre högra hörnet av Workfront Proof-gränssnittet och klicka sedan på fliken **Inställningar** .

1. Klicka på **Lägg till ny enhet** i avsnittet **Anpassade enheter för korrektur**.

1. Ange följande information i rutan **Lägg till ny enhet** som visas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td>Det namn som användarna ser när de väljer enheten i Desktop Proofing Viewer, enligt beskrivningen i <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">Ändra interaktiv korrekturupplösning i korrekturläsaren</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensioner</td> 
      <td>Ange måtten som ska användas för den här enheten. Användarna ser dimensionerna som visas under enhetsnamnet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Förhållande</td> 
      <td>Ange enhetens proportioner.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Typ</td> 
      <td>Ange om enheten är en mobil, bärbar eller stationär dator.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Användaragentsträng</td> 
      <td>Ange användaragenten för enheten för att ange information som får programmet att köras och visas som avsett för enheten.<p>Du kan hämta användaragenten genom att gå till <a href="https://www.whatismybrowser.com/detect/what-is-my-user-agent">https://www.whatismybrowser.com/detect/what-is-my-user-agent</a> från enheten.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Handikappade</td> 
      <td>Om det här alternativet är markerat är enheten inte tillgänglig för användare att välja när de granskar interaktiva korrektur.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Skapa**.

## Konfigurera popup-meddelanden för korrektur

Du kan konfigurera popup-meddelanden på korrektur för att kommunicera allmän information till alla granskare i organisationen.

Du kan konfigurera meddelanden så att de visas i följande situationer:

* **Vid inläsning av meddelande**: Visas när korrekturet öppnas första gången. Användbart för att förklara för användarna hur man granskar ett bevis eller lämnar en ansvarsfriskrivning eller annan juridisk text.
* **Ett beslutsmeddelande**: Visar när en användare väljer ett beslut om ett korrektur. Användbar för att ge användarna checklistor för exempelvis varumärken eller regelefterlevnad. Information om beslut finns i [Ta beslut om ett korrektur i korrekturläsaren](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

* **Bekräfta knapptext**: Den etikett som visas på knappen i popup-meddelandet Vid inläsning som förklaras ovan.

Så här skapar du popup-meddelanden för korrektur:

1. Klicka på **Redigera** till höger om meddelandet som du vill anpassa.
1. Ange ett meddelande och inkludera lämplig formatering och klicka sedan på **Spara**.
1. (Valfritt) Om du anpassade meddelandet Vid inläsning och även vill anpassa bekräftelseknappetiketten klickar du på **Redigera** till höger om **Bekräfta knapptext**, anger en etikett och klickar sedan på **Spara**.

## Konfigurera korrekturinställningar

Mer information om hur du konfigurerar korrekturinställningar för din organisation finns i [Konfigurera standardkorrekturinställningar](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).


## Konfigurera standardinställningar för delning

Du kan ange vilka korrektur som din organisation kan dela med sig av, vilka versioner som är tillgängliga för granskare och när korrektur med ett automatiserat arbetsflöde visas för användare som är kopplade till en viss fas.

Mer detaljerad information om delningsinställningar i Workfront Proof finns i [Konfigurera delningsinställningar för dina användare](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md).

## Varumärk Workfront Proof webbplats

Om du använder Workfront Proof kan du konfigurera branding för följande delar av webbplatsen:

* Den välkomstsida som visas när korrekturet läses in
* Logga in och logga ut skärmar
* E-postaviseringar

Mer information om varumärket finns på Workfront Proof webbplats [Varumärket på Workfront Proof webbplats](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).

## Konfigurera avancerade lösenordsinställningar

>[!IMPORTANT]
>
>Det här alternativet är endast tillgängligt för äldre Workfront-planer. Om du har en Pro-, Business- eller Enterprise Workfront-plan kan du inte längre konfigurera avancerade lösenordsinställningar.

Under **Avancerade lösenordsinställningar** kan du förbättra lösenordssäkerheten för dina användare.

1. Klicka på **Konfigurera** till höger om den inställning du vill konfigurera:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Minsta lösenordslängd</td> 
      <td>Standardlängden för Workfront Proof-lösenord är sex tecken. Du kanske vill öka antalet beroende på organisationens regler.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Teckenblandning</strong> </td> 
      <td>Du kan tvinga användarna att använda en blandning av gemener, versaler, siffror och symboler i sina lösenord. Du bestämmer hur många tecken lösenordet ska innehålla.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Maximalt antal tecken som upprepas</strong> </td> 
      <td>Du kan ange hur många tecken som ska upprepas i varje användares lösenord.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatisk lösenordshantering</td> 
      <td>Tvingar användare att regelbundet ändra sitt lösenord. Du bestämmer hur ofta de ska göra det.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Antal upprepningar av lösenord tillåts inte</strong> </td> 
      <td>Konfigurera antalet upprepningar av lösenord som inte tillåts i ditt konto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Profilutelåsning</strong> </td> 
      <td>Låser ut dina användare från kontot efter ett antal misslyckade inloggningsförsök som du anger. Du kan även ange hur länge de ska vänta innan de kan komma åt sitt konto igen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lås användare om lösenordet inte har återställts efter 30 dagar</td> 
      <td>Om din användare inte ändrar sitt första lösenord inom 30 dagar efter att profilen aktiverats, kommer de att låsas ut från kontot.<br><p>Kontoadministratörer kan låsa upp (återaktivera) användare som automatiskt låses av systemet. Detta ger dem ytterligare sju dagar för att ändra sitt lösenord.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lås användarkontot om det är inaktivt i 120 dagar</td> 
      <td>Om din användare inte loggar in på Workfront Proof eller ett inloggningsbevis som krävs i 120 dagar, kommer de att låsas ut från kontot.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ändra lösenord efter första inloggningen</strong> </td> 
      <td>Kräver att användare ändrar sitt tillfälliga lösenord efter den första inloggningen.<p>Kontoadministratörer kan låsa upp (återaktivera) användare som automatiskt är låsta av systemet.</p><p>Mer lösenordsinformation finns i <a href="../../../workfront-proof/wp-getstarted/faqs/log-in-change-password.md" class="MCXref xref">Logga in och ändra ditt lösenord och din e-postadress för Workfront Proof</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>
