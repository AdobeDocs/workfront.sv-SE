---
product-area: user-management;setup
navigation-topic: configure-your-user-profile
title: Konfigurera mina inställningar
description: Din [!DNL Adobe Workfront] profil innehåller information om dig själv (till exempel ditt namn, e-postadress, adress, telefonnummer, titel). Den innehåller även information om din interaktion med [!DNL Workfront]  och andra användare i ditt företag.
author: Lisa
feature: Get Started with Workfront
exl-id: 0199bf74-0611-48f0-9c05-da6afac85033
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '2894'
ht-degree: 0%

---

# Konfigurera mina inställningar

<!-- Audited: 01/2024 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Edit the job role FTE percentage allocation blurbs when more functionality is released: now, it says that the % is that of the user's schedule, but it will be either the user's schedule or the system schedule.</p>
-->

Din [!DNL Adobe Workfront]-profil innehåller information om dig själv (till exempel ditt namn, e-postadress, adress, telefonnummer, titel). Den innehåller även information om din interaktion med [!DNL Workfront] och andra användare i ditt företag (t.ex. dina aviseringsinställningar, flikarna som du vill visa i [!DNL Workfront] eller din jobbroll, chef samt grupp- och teammedlemskap).

Den mesta informationen har redan angetts av din [!DNL Workfront]-administratör när ditt [!DNL Workfront]-konto skapades.

Beroende på vilken åtkomstnivå du har i [!DNL Workfront] kan du redigera en del av den här informationen genom att konfigurera ditt [!UICONTROL My Settings]-område.

## Hur åtkomstnivåer påverkar redigeringen av [!UICONTROL My Settings]-området

Beroende på vilken åtkomstnivå du har kan du eventuellt redigera avsnitt i ditt [!UICONTROL My Settings]-område.

Vissa fält i redigerbara avsnitt kan inte redigeras, beroende på andra inställningar som kanske inte har konfigurerats på åtkomstnivån. Mer information om ytterligare åtkomst som behövs för att redigera vissa av fälten som du hittar i [!UICONTROL My Settings] finns i avsnitten i [Konfigurera området [!UICONTROL My Settings]](#configuring-the-my-settings-area).

Om du vill ta reda på vilken åtkomstnivå du har kontaktar du [!DNL Workfront]-administratören.

Följande rutnät visar vilka avsnitt i området [!UICONTROL My Settings] som är synliga eller redigerbara beroende på din åtkomstnivå:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>[!UICONTROL My Settings] områden </strong> </th> 
   <th><strong>Synlig eller redigerbar</strong> </th> 
   <th><strong>[!UICONTROL System Administrator]</strong> </th> 
   <th><strong>[!UICONTROL Standard] eller [!UICONTROL Planner]</strong> </th> 
   <th><strong>[!UICONTROL Worker]</strong> </th> 
   <th><strong>[!UICONTROL Light] eller [!UICONTROL Reviewer]</strong> </th> 
   <th><strong>[!UICONTROL Contributor] eller [!UICONTROL Requestor]</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2">[!UICONTROL Personal Info]</td> 
   <td> <p>Synlig</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td> <p>Redigerbar</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Preferences]</td> 
   <td> <p>Synlig</p> </td> 
   <td> <p>✔</p> </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>Redigerbar</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Notifications]</td> 
   <td> <p>Synlig</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td> <p>Redigerbar</p> </td> 
   <td> <p>✔</p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td> ✔</td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Access]</td> 
   <td>Synlig</td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Redigerbar</td> 
   <td> ✔</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Organization]</td> 
   <td>Synlig</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Redigerbar</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Resource Planning]</td> 
   <td>Synlig</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Redigerbar</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Custom Forms]</td> 
   <td>Synlig</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>Redigerbar</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td rowspan="2">[!UICONTROL Comment]</td> 
   <td>Synlig</td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td>Redigerbar</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurerar området [!UICONTROL My Settings]

{{step1-click-profile-pic}}

1. Klicka på menyn **[!UICONTROL More]** bredvid ditt namn ![Mer meny](assets/more-icon.png) och klicka sedan på **[!UICONTROL Edit]**.

1. Beroende på din åtkomstnivå kan du uppdatera följande avsnitt:

   * [Personlig information](#personal-info)
   * [Inställningar](#preferences)
   * [Meddelanden](#notifications)
   * [Åtkomst](#access)
   * [Organisation](#organization)
   * [Resursplanering](#resource-planning)
   * [Anpassad Forms](#custom-form)
   * [Kommentar](#comment)

1. Klicka på **[!UICONTROL Save]**.

### [!UICONTROL Personal Info]

Detta avsnitt innehåller följande underavsnitt:

* [Grundläggande information](#basic-info)
* [Jobbinformation](#job-info)
* [Kontaktinformation](#contact-info)

#### [!UICONTROL Basic info]

Den här informationen bör redan konfigureras av [!DNL Workfront]-administratören. Alla fält i det här underavsnittet är obligatoriska fält.

Du kan ändra något av följande i det här underavsnittet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL First Name]</strong></td> 
   <td>Uppdatera ditt förnamn. Detta är ett obligatoriskt fält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Last Name]</strong></td> 
   <td>Uppdatera ditt efternamn. Detta är ett obligatoriskt fält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Email Address]</strong></td> 
   <td> Uppdatera din e-postadress. Detta är ett obligatoriskt fält. Kom ihåg att din e-postadress även är ditt användarnamn för [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Reset password]</strong></td> 
   <td>Återställ lösenordet i det här avsnittet. Mer information om hur du återställer lösenordet finns i <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Återställ lösenordet</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Villkorlig) &lt;SSO-konfiguration&gt; [!UICONTROL Username]</strong></td> 
   <td> Om din [!DNL Workfront]-administratör har aktiverat en SSO-integrering med [!DNL Workfront] visas ditt SSO-användarnamn i det här fältet. Typen av SSO-konfiguration som är aktiverad för din [!DNL Workfront]-instans visas i det här fältet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Villkorligt) [!UICONTROL Only Allow <SSO Configuration> Authentication]</strong></td> 
   <td> <p> Om administratören för [!DNL Workfront] aktiverade en SSO-integrering med [!DNL Workfront] och har uppdaterat användare för enkel inloggning, är det här fältet markerat som standard. Typen av SSO-konfiguration som är aktiverad för din [!DNL Workfront]-instans visas i det här fältet.</p> <p>När det här fältet är markerat måste du logga in på [!DNL Workfront] med dina SSO-autentiseringsuppgifter. Om du avmarkerar den kan du logga in på [!DNL Workfront] med dina [!DNL Workfront]-inloggningsuppgifter.</p> <p>Mer information om hur du konfigurerar [!DNL Workfront] med en SSO-lösning finns i <a href="../../../administration-and-setup/add-users/single-sign-on/single-sign-on.md" class="MCXref xref">Enkel inloggning i [!DNL Workfront]: artikelindex</a>. Mer information om hur du uppdaterar användare för enkel inloggning finns i <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Uppdatera användare för enkel inloggning</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Job info]

Du kan ändra något av följande i det här underavsnittet:

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Title]</strong></td>
        <td>Ange titel. Detta är inte samma sak som din jobbroll. Titeln ingår inte i resursplaneringen, men din jobbroll är det. Din titel visas i [!DNL Workfront]-gränssnittet överallt med ditt namn och din avatarskärm. Den är synlig för alla som har tillgång till din användarprofil.</td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Talk to Me About]</strong></td>
        <td>Ange dina yrkesmässiga intressen i det här fältet.</td>
    </tr>
</table>

#### [!UICONTROL Contact info]

Du kan ändra något av följande i det här underavsnittet:

<table style="table-layout:auto">
    <tr>
        <td><strong>[!UICONTROL Phone Number]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Extension]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Mobile Number]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Address]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL City]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL State]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Postal Code]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Country]</strong></td>
        <td> </td>
    </tr>
    <tr>
        <td><strong>[!UICONTROL Profile Picture]</strong></td>
        <td>Din profilbild blir din avatar och den visas i hela [!DNL Workfront]-systemet, oavsett var ditt namn visas.</td>
    </tr>
</table>

### [!UICONTROL Preferences]

Ange vad du vill visa i ditt [!DNL Workfront]-gränssnitt i det här avsnittet.

>[!NOTE]
>
>Användare med en [!UICONTROL Contributor]- eller [!UICONTROL Requestor]-licens har inga andra vänsterpanelsobjekt tillgängliga att lägga till i sina [!UICONTROL Main Menu] utanför [!UICONTROL Requests]-området. En [!DNL Workfront]-administratör kan tilldela användare med en [!UICONTROL Contributor]- eller [!UICONTROL Requestor]-licens till en layoutmall som innehåller alla andra områden i [!UICONTROL Main Menu]. Efter det kan de markera de områden som ska visas i sina [!UICONTROL Main Menu] genom att redigera deras användarprofil.

Du kan ändra något av följande i det här underavsnittet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Time Zone]</strong> </td> 
   <td><p>Ange din tidszon. Detta styr den tid som visas i dina utgående e-postmeddelanden.</p>
       <p>Tidszonen påverkar även vad som visas i en PTO-kalenderrapport.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Email Locale]</strong> </td> 
   <td><p>Ange önskat språk här. Detta styr vilket språk, datum och nummerformat som används i utgående e-postmeddelanden.</p>
   <p><strong>Obs!</strong> När din organisation använder Adobe Unified Experience lagras språkinställningarna i din Adobe-profil och e-postspråkinställningen används inte. Mer information finns i <a href="/help/quicksilver/workfront-basics/supported-languages-in-workfront.md#change-the-adobe-experience-cloud-language">Ändra Adobe Experience Cloud-språk</a> i artikeln <a href="/help/quicksilver/workfront-basics/supported-languages-in-workfront.md">Språk som stöds i Adobe Workfront</a>.</p></td> 
  </tr>

<tr> 
   <td role="rowheader"><strong>[!UICONTROL Send work assigned to myself to my Working On tab]</strong> </td> 
   <td>Det här fältet refererar till en inaktuell funktion som har tagits bort från [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Villkorligt) Generera korrektur automatiskt när dokument överförs</strong></td> 
   <td>Markera det här fältet om du vill börja generera ett korrektur omedelbart efter att dokumentet har lästs in i [!DNL Workfront]. Det här fältet är inaktiverat som standard och kan bara uppdateras av en Workfront-administratör.<br>Det här fältet är bara tillgängligt om ditt företag har köpt Workfront Proof-komponenten för Workfront och om du har aktiverats som korrekturanvändare. Mer information om Workfront Proof finns i <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md" class="MCXref xref">Hantera korrektur i Adobe Workfront</a>.
   <p><b>Obs!</b> Dokument som överförs till en begäran genererar inte något korrektur automatiskt. </p></td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Notifications]

Ange vilka meddelanden du vill ta emot från [!DNL Workfront]. Mer information om hur du konfigurerar meddelanden finns i [Ändra dina egna e-postmeddelanden](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### [!UICONTROL Access]

Din åtkomst och andra associerade komponenter konfigureras av din [!DNL Workfront]-administratör när ditt konto är konfigurerat.

Endast en [!DNL Workfront]-administratör kan se och redigera alla fält i det här avsnittet.

Du kan ändra något av följande i det här underavsnittet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Is Active]</strong> </td> 
   <td>Det här fältet är bara synligt för en användare som också är [!DNL Workfront]-administratör och bör vara markerat som standard. Detta innebär att användaren är aktiv och kan logga in på [!DNL Workfront]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Access Level]</strong> </td> 
   <td>Det här fältet är synligt för användare med åtkomstnivån [!UICONTROL Standard], [!UICONTROL Plan] eller [!UICONTROL Workfront administrator] och kan bara redigeras av [!DNL Workfront]-administratörer. Om du är [!DNL Workfront]-administratör bör du inte ändra din åtkomstnivå till något lägre när du ändrar det här fältet. </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Layout Template]</strong> </td> 
   <td>Det här fältet är synligt för användare med åtkomstnivån [!UICONTROL Standard], [!UICONTROL Plan] eller [!UICONTROL [!DNL Workfront] administrator] och kan bara redigeras för [!UICONTROL [!DNL Workfront] administratörer] eller användare med en [!UICONTROL Standard]- eller [!UICONTROL Plan]-licens som också har administratörsbehörighet. Här väljer du en layoutmall för att uppdatera utseendet och fältet i Workfront-gränssnittet. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">Konfigurera användarnas åtkomst till att redigera användare med en anpassad åtkomstnivå</a> i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.<br>Mer information om layoutmallar och hur de påverkar gränssnittet finns i <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Skapa och hantera layoutmallar</a></td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader"><strong>Log in as</strong> </td> 
    <td> <p><strong>Add access</strong> for a Workfront administrator or group administrator (associated with a group you are in) to log in as you. Select an <strong>Access expiration date</strong> for the login. </p> <p>You can repeat this to grant login access to multiple administrators.</p> <p>The settings you choose in this section are visible only to you.
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <span class="PinkDraftNote">Add a note about this being only for the Enterprise package if they decide to do it that way. Functionality that may come in a later sprint: If you want to be notified when the administrator logs in as you, select Receive an email when this user logs in.</span> 
       </MadCap:conditionalText>
      </p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader"><strong>(Villkorligt) [!UICONTROL User can generate proofs (... out of ... proof licenses left)]</strong></td> 
   <td>Det här fältet är bara tillgängligt om ditt företag använder en äldre [!DNL Workfront]-plan och har köpt komponenten [!DNL Workfront Proof]. När det är markerat aktiveras du som korrekturanvändare. Här visas även antalet licenser som används i systemet av det totala antalet köpta korrekturlicenser. Det här fältet är bara synligt och redigerbart för användare som också är [!DNL Workfront] administratörer. Mer information om planalternativ för korrektur i [!DNL Workfront] finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md">Åtkomst till korrekturfunktioner i [!DNL Workfront]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Villkorligt) [!UICONTROL Permission Profile]</strong></td> 
   <td> <p>I det här fältet visas åtkomstnivån i [!DNL Workfront Proof]. Det är bara tillgängligt om:</p> 
    <ul> 
     <li>Ditt företag använder en äldre [!DNL Workfront]-plan och har köpt komponenten [!DNL Workfront Proof], eller så har du en [!UICONTROL Standard]-, [!UICONTROL Work]- eller [!UICONTROL Plan]-licens för en nyare [!DNL Workfront]-plan.</li> 
     <li>Du är aktiverad som korrekturanvändare.</li> 
    </ul> <p>[!DNL Workfront] administratörer kan redigera fältet för alla användare utom själva, så att alla användare ser fältet som skrivskyddat i sina egna profiler. Mer information om behörighetsprofilen finns i <a href="../../../review-and-approve-work/proofing/proofing-overview/permission-profiles.md" class="MCXref xref">Översikt över behörighetsprofiler</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Organization]

Den här informationen konfigureras vanligtvis av [!DNL Workfront]-administratören när de skapar ditt [!DNL Workfront]-konto. Du kan även uppdatera information om din organisation eller organisationsstruktur i det här avsnittet. Endast användare med åtkomstnivån [!UICONTROL Standard], [!UICONTROL Plan] eller [!UICONTROL System Administrator] kan redigera det här avsnittet.

Du kan ändra något av följande i det här underavsnittet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Company]</strong></td> 
   <td>Välj namnet på det företag du tillhör i listrutan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Villkorligt) [!UICONTROL Reports To]</strong></td> 
   <td>När du har valt en <strong>[!UICONTROL Company]</strong> för din profil kan du även ange namnet på din chef i det här fältet. Du kan bara ange ett namn här och vi rekommenderar att du anger namnet på din chef. Börja skriva sitt namn och klicka för att markera det när det visas i listan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Villkorligt) [!UICONTROL Direct Reports]</strong></td> 
   <td>När du har valt en <strong>[!UICONTROL Company]</strong> för din profil kan du även ange namnet på dina direkta rapporter i det här fältet. Du kan ange så många direktrapporter som behövs här. Börja skriva namnen och klicka för att markera dem när de visas i listan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Home Team]</strong> </td> 
   <td> <p>Välj en <strong>[!UICONTROL Home Team]</strong> i listrutan. Det här fältet är synligt för användare med en [!UICONTROL Standard]-, [!UICONTROL Plan]- eller [!UICONTROL System Administrator]-åtkomstnivå och kan bara redigeras för [!DNL Workfront] administratörer eller användare med en [!UICONTROL Standard]- eller [!UICONTROL Plan]-licens som också har administratörsbehörighet. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">Konfigurera användarnas åtkomst till att redigera användare med en anpassad åtkomstnivå</a> i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.<br></p> <p><strong>Hemteamet</strong> kan påverka utseendet på ditt [!DNL Workfront]-gränssnitt, om en layoutmall är associerad med teamet. </p> <p>Mer information om team finns i <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Teams overview</a>.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Other Teams]</strong> </td> 
   <td> <p>Du kan tillhöra fler än ett team. Ange ytterligare team som du tillhör i det här fältet genom att börja skriva namnet på ett team och sedan klicka för att markera det när det visas i listan. Tillhör för många team kan skapa förvirring om arbete som är tilldelat teamen. Mer information om team finns i <a href="../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md" class="MCXref xref">Teams overview</a>.</p> <p>Det här fältet är synligt för användare med en [!UICONTROL Standard]-, [!UICONTROL Plan]- eller [!UICONTROL System Administrator]-licens och kan bara redigeras för [!DNL Workfront]-administratörer eller användare med en [!UICONTROL Standard]- eller [!UICONTROL Plan]-licens som också har administratörsbehörighet. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">Konfigurera användarnas åtkomst till att redigera användare med en anpassad åtkomstnivå</a> i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Home Group]</strong> </td> 
   <td> <p>Välj en <strong>[!UICONTROL Home Group]</strong> i listrutan.</p> <p>Obs! Detta är ett obligatoriskt fält. Du kan inte ha en användare som inte är associerad med en grupp.<br></p> <p>Det här fältet är synligt för användare med en [!UICONTROL Standard]-, [!UICONTROL Plan]- eller [!UICONTROL System Administrator]-nivå. Mer information om vem som kan redigera fältet <strong>[!UICONTROL Home Group]</strong> finns i <a href="/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"class="MCXref xref">Redigera en användares profil</a>. <strong>[!UICONTROL Home Group]</strong> är standardgruppen för alla projekt och standardgruppen <strong>[!UICONTROL Home Group]</strong> för alla nya användare som du skapar. Alla anpassade formulär som du skapar delas med <strong>[!UICONTROL Home Group]</strong> som standard.</p> <p>Mer information om grupper finns i <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Översikt över grupper</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Other Groups]</strong> </td> 
   <td> <p>Du kan tillhöra flera grupper. Ange ytterligare grupper som du tillhör i det här fältet genom att börja skriva namnet på en grupp. Klicka för att markera den när den visas i listan. Det här fältet är synligt för användare med åtkomstnivån [!UICONTROL Standard], [!UICONTROL Plan] eller [!UICONTROL System Administrator]. Mer information om vem som kan redigera fältet <strong>[!UICONTROL Other Groups]</strong> finns i <a href="/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md"class="MCXref xref">Redigera en användares profil</a>.</p> <p>Mer information om grupper finns i <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Översikt över grupper</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Resource Planning]

Resursplaneringsinformationen påverkar tidslinjen för arbetstilldelningar, den tid du loggar, kostnader och intäkter för de projekt du är på. Normalt uppdateras det här området av [!DNL Workfront]-administratören, ett projekt eller en resurshanterare, eller av din direktansvarige.

Använd något av följande i det här avsnittet:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Schedule Deactivation]</strong></td> 
   <td>Markera den här rutan om du vill schemalägga att ditt konto ska inaktiveras efter en viss tidsperiod. I <p><strong>[!UICONTROL Scheduled Deactivation Date]</strong> anger vilket datum ditt konto ska inaktiveras. Information om hur du inaktiverar användare finns i <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation" class="MCXref xref">Schemalägg användare för inaktivering</a> i <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Inaktivera eller återaktivera en användare</a>. </p><p>Du kan redigera inaktiveringsfälten för ditt konto om du har en [!UICONTROL Standard]- eller [!UICONTROL Plan]-licens eller om du är [!DNL Workfront]-administratör. </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Primary Role]</strong></td> 
   <td> <p>Det här är den primära rollen som du kan fylla i Workfront. Alla uppgifter och utgåvor som du är tilldelad till tilldelas som standard även den här jobbrollen. Jobbroller är viktiga i resurshanteringen. Mer information om jobbroller finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.</p> <p>Du kan bara uppdatera det här fältet om du har en [!UICONTROL Standard]- eller [!UICONTROL Plan]-licens med administrativ användaråtkomst eller om du är [!DNL Workfront]-administratör. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#configure-users-access-to-edit-users-using-a-custom-access-level" class="MCXref xref">Konfigurera användarnas åtkomst till att redigera användare med en anpassad åtkomstnivå</a> i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Villkorligt) Om du valde [!UICONTROL Primary Role] visas fältet [!UICONTROL Percentage of FTE Availability].</strong></td> 
   <td>Ange hur stor procentandel av din schemalagda tid som tilldelas den här jobbrollen. Standardvärdet för [!UICONTROL Percentage of FTE Availability] för den primära rollen är 100 %.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Other Roles]</strong> </td> 
   <td> <p>Du kan ha flera jobbroller i [!DNL Workfront]. Jobbroller är viktiga i resurshanteringen. Mer information om jobbroller finns i <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Skapa och hantera jobbroller</a>.</p> <p>Du kan bara uppdatera det här fältet om du har en [!UICONTROL Standard]- eller [!UICONTROL Plan]-licens med administrativ användaråtkomst eller om du är [!DNL Workfront]-administratör. Mer information om hur du konfigurerar användare med administrativ användaråtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Konfigurera användarnas åtkomst till att redigera användare med en anpassad åtkomstnivå</a> i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Bevilja åtkomst till användare</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>(Villkorligt) Om du valde en eller flera andra roller visas fältet [!UICONTROL Percentage of FTE Availability] för varje roll.</strong></td> 
   <td> <p>Ange hur stor procentandel av den schemalagda tiden som ska tilldelas varje jobbroll. Standardvärdet för [!UICONTROL Percentage of FTE Availability] för [!UICONTROL Other Roles] är 0 %.</p> <p> <img src="assets/user-settings-roles-and-dte-boxes-rp-story--1--350x224.png" alt="user_settings_roles_and_date_boxes_rp_story__1_.png" style="width: 350;height: 224;"> </p> <p>Obs!  
     <ul> 
      <li>Om [!UICONTROL Other Roles] har 0 % FTE-tillgänglighet visas de inte i [!UICONTROL Resource Planner], såvida inte användarna har tilldelats uppgifter i de här rollerna.</li> 
      <li> <p>Summan av alla <strong>[!UICONTROL Percentages of FTE Availability]</strong> för alla roller måste vara lika med 100 %. Varje [!UICONTROL Percentage of FTE Availability] beräknar [!UICONTROL Available Hours] för varje roll per användare i [!UICONTROL Resource Planner]. </p> <p>[!UICONTROL Available Hours] för varje roll per användare beror på användarens tillgängliga tid. Den tillgängliga tiden för användaren beräknas av [!DNL Workfront] beroende på metoden som har valts av [!DNL Workfront]-administratören för att beräkna FTE i [!UICONTROL Resource Management Preferences]. Mer information om hur du beräknar tillgängligheten för användaren finns i <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Översikt över beräkning av timmar och FTE för användare och roller i resursplaneraren</a>. Mer information om hur du konfigurerar inställningar för resurshantering finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurera inställningar för resurshantering</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Schema</strong></td> 
   <td> <p>Endast [!DNL Workfront] administratörer eller användare med en [!UICONTROL Standard]- eller [!UICONTROL Plan]-licens som även har administrativ åtkomst för tidrapporter och timmar kan uppdatera det här fältet. Mer information om administrativ åtkomst för tidrapporter och timmar finns i avsnittet"Tidrapporter och timmar" i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Bevilja användare administrativ åtkomst till vissa områden</a>.</p> <p>Välj rätt tidrapport i listrutan. Detta garanterar att dina tidrapporter genereras automatiskt, i enlighet med de specifikationer som angetts av [!DNL Workfront]-administratören. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Default Hour Type]</strong> </td> 
   <td>Välj standardtimtyp. Det här är timtypen som systemet använder som standard när du loggar in i Workfront.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Available Hour Types]</strong> </td> 
   <td>Välj de timtyper som du ska kunna välja mellan när du loggar tid. Timtyperna i den här nedrullningsbara menyn är tillgängliga av administratören för [!DNL Workfront].</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Resource Pool]</strong> </td> 
   <td>Välj en resurspool som du tillhör. Detta fält är endast avsett för rapportering och information. Detta påverkar inte schemaläggning eller planering av resurser.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL FTE]</strong> </td> 
   <td> <p>Det tal som du anger här tas endast med i beräkningen av din tillgänglighet baserat på standardschemat när [!UICONTROL Resource Management Preferences] på systemnivå är inställd på <strong>[!UICONTROL The Default Schedule]</strong>.</p> <p>Om till exempel FTE-värdet är 0,5 och [!UICONTROL Default Schedule] är 40 timmar är du tillgänglig för arbete 20 timmar i veckan.</p> <p>Om [!UICONTROL Resource Management Preferences] på systemnivå är inställd på <strong>[!UICONTROL The User's Schedule]</strong> ignoreras det värde du anger här och du är tillgänglig för att arbeta enligt vad som anges i schemat. I det här fallet beräknas FTE för [!UICONTROL Resource Planner] enligt följande formel: </p> <p><code style="font-style: normal;">[!UICONTROL User Available FTE] = [!UICONTROL Hours from the Schedule of the User/ Default Schedule Hours]</code> </p> <p>Mer information om hur du beräknar FTE för användare finns i <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Översikt över beräkning av timmar och FTE för användare och roller i resursplaneraren</a>.</p> <p>Mer information om hur du skapar scheman i [!DNL Workfront] finns i <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Skapa ett schema</a>.</p> <p>Mer information om hur du konfigurerar inställningar för resurshantering finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurera inställningar för resurshantering</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Cost per Hour]</strong> </td> 
   <td>Ange kostnaden per timme för användaren. Mer information om att spåra kostnader i [!DNL Workfront] finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>. Du kan inte uppdatera den här informationen om du inte har åtkomst till ekonomiska data från din åtkomstnivå eller om du är [!DNL Workfront]-administratör. Mer information om ekonomisk åtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Bevilja åtkomst till ekonomiska data</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!UICONTROL Billing per Hour]</strong> </td> 
   <td>Ange beloppet för fakturering per timme för användaren. Mer information om att spåra fakturering och intäkter finns i <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkter</a>. Du kan inte uppdatera den här informationen om du inte har åtkomst till ekonomiska data från din åtkomstnivå eller om du är [!DNL Workfront]-administratör. Mer information om ekonomisk åtkomst finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Bevilja åtkomst till ekonomiska data</a>.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Custom Forms]

Du kan koppla ett anpassat formulär till din användarprofil. Detta gör att du kan lagra ytterligare information för användaren som annars inte kan lagras i de [!DNL Workfront] inbyggda fälten som beskrivs ovan.

Du måste ha någon av följande behörigheter eller behörigheter för att kunna koppla ett anpassat formulär till din användarprofil:

* Du är [!DNL Workfront]-administratör.
* Du är en [!UICONTROL Standard]- eller [!UICONTROL Plan]-licensanvändare och det anpassade användarformuläret delas med en av dina grupper.

Alla användare kan se anpassade formulär som har kopplats till deras profiler.

Administratören för [!DNL Workfront] måste konfigurera anpassade formulär för användarobjektet för att du ska kunna koppla ett anpassat formulär till användarprofilen. Mer information om hur du skapar anpassade formulär finns i [Designa ett formulär med formulärdesignern](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### [!UICONTROL Comment]

Du kan spela in en kommentar på din användarprofil, som lagras på profilens [!UICONTROL Updates]-flik.

Du kan klicka på ikonen [!UICONTROL people] om du vill ta med andra i uppdateringen.

Du kan klicka på ikonen [!UICONTROL lock] för att göra uppdateringen privat för användare som är i samma företag som du.
