---
title: Skapa och ändra anpassade åtkomstnivåer
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Som Adobe Workfront-administratör kan du skapa anpassade åtkomstnivåer och använda dem för användare.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 0f2923851230e830eb647d422f2862a0c5d5472b
workflow-type: tm+mt
source-wordcount: '1468'
ht-degree: 0%

---

# Skapa och ändra anpassade åtkomstnivåer

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

Som Adobe Workfront-administratör kan du skapa anpassade åtkomstnivåer och använda dem för användare. När du arbetar med åtkomstnivåer är det viktigt att förstå hur de fungerar tillsammans med objektbehörigheterna som användarna ger när de delar objekt med varandra. Mer information om åtkomstnivåer finns i:

* [Översikt över nya åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>Vi rekommenderar att du låter de inbyggda åtkomstnivåerna vara oförändrade så att du kan referera till dem när du har konfigurerat användarna. Om du vill anpassa en åtkomstnivå kopierar du standardåtkomstnivån och ändrar kopian. Du kan göra detta för alla åtkomstnivåer förutom systemadministratör och extern användare.

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
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa eller redigera en anpassad åtkomstnivå

{{step-1-to-setup}}

1. Klicka på **Åtkomstnivåer** i den vänstra panelen.
1. Välj den åtkomstnivå som du vill kopiera och anpassa och klicka sedan på ikonen **Kopiera** ![Kopiera](assets/copy-icon.png) .

   eller

   Om du redigerar en befintlig åtkomstnivå markerar du åtkomstnivån genom att klicka i rutan till vänster om åtkomstnivån och klickar sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) .

1. I rutan som visas gör du något av följande för att börja konfigurera den anpassade åtkomstnivån:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Namn</td> 
      <td> <p>Ange ett namn för åtkomstnivån. </p> <p>Om du precis har kopierat en åtkomstnivå för att skapa en ny är standardnamnet Åtkomstnivånamn (kopia), där åtkomstnivånamnet är den åtkomstnivå du kopierade.</p> <p><strong>Tips</strong>: Vi rekommenderar att du inkluderar det ursprungliga namnet på åtkomstnivån i kopians namn. På ACME-företaget kan till exempel en kopia av åtkomstnivån Standard heta ACME Standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning </td> 
      <td>Ange en beskrivning för åtkomstnivån. Det är praktiskt att här ange vad en användare med den här åtkomstnivån kan komma åt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Licenstyp</td> 
      <td>Se till att den licens som valts här är den som är mest kopplad till den typ av åtkomstnivå som du skapar eller redigerar. Den valda licensen avgör vilka inställningar som är tillgängliga för åtkomstnivån. Mer information finns i <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Översikt över nya licenser</a> eller <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Översikt över licenser</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Villkorligt) Om **Standard** eller **Plan** har valts i rutan **Licenstyp** bläddrar du till avsnittet **Tillåt administrativ åtkomst för** och väljer administratörsbehörighet för de som ska ha den här åtkomstnivån.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Godkännandeprocesser</td> 
      <td>Skapa och hantera godkännandeprocesser som kan användas i hela systemet och för specifika grupper.<p>Utan den här åtkomsten kan användare bara skapa ad hoc-godkännandeprocesser för objekt som de har åtkomst till att hantera.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Företag</td> 
      <td>Lägg till nya och redigera befintliga företag i Workfront.<br><p>Utan den här åtkomsten kan användare bara visa befintliga företag.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Egna formulär</td> 
      <td>Skapa och hantera alla anpassade formulär i gruppen. <br><p>Utan den här åtkomsten kan användare bara bifoga befintliga formulär till objekt som de har åtkomst till för att bidra eller hantera.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Växelkurser</td> 
      <td> Lägg till ny valuta i Workfront. <p>Utan den här åtkomsten kan användaren bara lägga till en befintlig valuta i ett projekt som han/hon skapar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Utgifter</td> 
      <td>Visa alla utgifter för objekt i Workfront.<p>Utan den här åtkomsten kan användaren bara visa följande:</p>
       <ul>
        <li>Utgifter för projekt, uppgifter eller ärenden som de hanterar</li>
        <li>Deras egna utgifter</li>
        <li>Utgifter för underordnade</li>
       </ul><p><b>Obs!</b>: Detta innebär inte att användaren kan skapa nya utgiftstyper.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Jobbroller</td> 
      <td> Med den här åtkomsten kan användaren göra följande: 
       <ul> 
        <li>Visa och redigera befintliga jobbroller</li> 
        <li>Lägg till nya jobbroller</li> 
        <li>Redigera rollfakturering och kostnadstariffer</li> 
       </ul> 
       <p>Viktig information om åtkomst till ekonomiska data som är tillgängliga för en Standard- eller Planering-användare med administrativ åtkomst till jobbroller finns i <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">Standard- eller Planeringsanvändare med administrativ åtkomst till jobbroller</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Milstolpar i min grupp</td> 
      <td>Visa alla milstolpesökvägar i systemet under menyn Milstolpbanor i Konfigurera. Användare kan också redigera eller ta bort alla milstolpbanor som tillhör någon av deras grupper. Användare kan inte hantera (redigera eller ta bort) milstolpesökvägar som inte är tilldelade till deras grupper.<p>Utan den här åtkomsten kan användare bara visa befintliga milstolpbanor och använda dem i projekt som de har tillgång till för att hantera.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Påminnelsemeddelanden</td> 
      <td>Skapa och hantera påminnelsemeddelanden i Workfront.<p>Utan den här åtkomsten begränsas användarna till att ta emot och visa meddelanden.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tidrapporter och timmar</td> 
      <td> Gruppadministratörer kan tilldela tidrapportprofiler till användare i de grupper och undergrupper som de hanterar. <p>Om det här alternativet inte är aktiverat kan gruppadministratörer inte tilldela andra användare i de grupper och undergrupper som de hanterar tidrapportprofiler, även om de kan skapa dem.</p> <p>Alla andra användare som har en Standard- eller Plan-licens kan visa alla timmar och tidrapporter i Workfront.</p> <p>Om det här alternativet inte är aktiverat kan användare bara visa timmar på:</p> 
       <ul> 
        <li>Projekt, uppgifter eller problem som de hanterar</li> 
        <li>Deras egen tidrapport</li> 
        <li>En tidrapport med någon som rapporterar till dem</li> 
        <li>En tidrapport som de godkänner</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Ange ytterligare begränsningar** och ange sedan någon av följande begränsningar för åtkomstnivån.

   >[!IMPORTANT]
   >
   >För externa användare som leverantörer (alla som inte finns i organisationen) rekommenderar vi att du begränsar åtkomsten till uppgifter, projekt, uppdateringar, meddelanden, andra företag, team och grupper.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ge aldrig åtkomst till hela projektet när det tilldelas till en uppgift eller ett ärende</td> 
      <td> Förhindrar att användare som har tilldelats till uppgifter eller problem också får behörighet till det överordnade projektet, även om projektbehörigheterna tillåter det.<p>Mer information om hur du konfigurerar behörigheter för ett projekt finns i avsnittet <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> i artikeln <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Redigera projekt</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ärv aldrig dokumentåtkomst från projekt, uppgifter, ärenden osv.</td> 
      <td>Förhindrar att dokument ärver de behörigheter som angetts för deras överordnade objekt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa endast uppdateringar som de har inkluderats i konversationen</td> 
      <td> Gör det möjligt för användare att endast se kommentarer där deras namn eller teamets namn har inkluderats. <p> <p><b>OBS!</b>: Detta förhindrar användare från att prenumerera på objekt i Workfront. Mer information om att prenumerera på objekt finns i <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Prenumerera på objekt i Adobe Workfront</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt aldrig användare att ta bort kommentarer </td> 
      <td> Hindrar användare från att ta bort kommentarer om objekt.  <p><b>Obs!</b> Ingen kan ta bort kommentarer från andra användare.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa endast företag, grupper och team som de tillhör</td> 
      <td>Tillåter användare att endast visa och dela objekt med företag, grupper och team som de tillhör.<p><strong>Obs!</strong>: Användare med beställar- eller medverkarlicenser kan inte visa företag som de inte tillhör, även om det här alternativet har valts.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt aldrig synlighet för planerade timmar eller faktiska timmar</td> 
      <td>Hindrar användare från att se de planerade och faktiska timmarna av arbetsobjekt de har tillgång till. De kan dock se faktiska timmar som de loggar sig själva eller timmar som loggas av någon som rapporterar till dem.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt aldrig användare att ta bort meddelanden</td> 
      <td>Förhindrar att användare tar bort meddelanden i meddelandecentret. Mer information finns i <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Skicka meddelanden</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Villkorligt och valfritt) Om ditt Workfront-system är konfigurerat för användare som tillhör flera företag kan du begränsa synligheten till andra användare baserat på vilket företag de tillhör i avsnittet **Personer i andra företag bör endast visa användare från**.

   Du kan begränsa användarna så att de bara kan se användare från det egna företaget eller från det företag som du har angett som primärt företag. Det primära företaget representerar vanligtvis ditt Workfront-konto där de flesta av dina användare arbetar. Mer information om det primära företaget finns i [Skapa och redigera företag](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Om två användare tillhör två olika företag, men båda kan se användare från det primära företaget, kan de se uppdateringsområdet som är associerat med det primära företaget.

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med en av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till aktiviteter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) och [Bevilja åtkomst till ekonomiska data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Klicka på **Spara**.

   När åtkomstnivån har skapats kan du tilldela den till en användare (om det inte är en åtkomstnivå för systemadministratörer).

   Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Mer information om hur en Adobe-administratör tilldelar en systemadministratörsåtkomstnivå till en användare finns i [Bevilja en användare fullständig administrativ åtkomst](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Standard- eller planeringsläsare med administrativ åtkomst till jobbroller {#planner-users}

Om du ger en Standard- eller Planering-användare administrativ åtkomst till jobbroller aktiveras inställningen Redigera rollfakturering och kostnadstariffer automatiskt för användaren.

Om du senare inaktiverar administrativ åtkomst till jobbroller för användaren, visas jobbrollerna fortfarande för användaren eftersom inställningen Redigera rollfakturering och kostnadstariffer fortfarande är aktiverad.

Om detta inträffar och du måste ta bort användarens åtkomst för att kunna visa jobbroller, måste du inaktivera användarens behörighetsinställning Redigera rollfakturering och kostnadstariffer. Instruktioner finns i [Bevilja åtkomst till ekonomiska data](grant-access-financial.md).



