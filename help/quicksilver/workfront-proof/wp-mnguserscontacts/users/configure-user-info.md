---
product-previous: workfront-proof
product-area: documents;system-administration;user-management;setup
navigation-topic: users-workfront-proof
title: Konfigurera användarinformation med  [!DNL Workfront Proof]
description: Konfigurera användarinformation med  [!DNL Workfront Proof]
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ae8d3a96-ebf1-48ee-a7b7-50d69bffbd36
source-git-commit: f776fb88000ea6044b88cba88d0cb7198c205d05
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# Konfigurera användarinformation med [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

1. Börja skapa eller redigera en användare enligt beskrivningen i [Skapa användare med  [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/users/create-users.md).
1. Ange följande information:

   * I avsnittet **[!UICONTROL Personal Details]**:

      * **E-postadress:** Användarens e-postadress.
      * **Förnamn:** Användarens förnamn.
      * **Efternamn:** Användarens efternamn.
      * **Position:** Användarens position i företaget.
      * **Behörighetsprofil:** Användarens behörigheter på korrekturkontot.
      * **Språk:** Användarens primära språk.
      * **Tidszon:** Välj användarens tidszon.
      * **Datumformat:** Välj användarens önskade datumformat.
      * **Anmäl dig - produkt- och marknadsföringsmeddelanden:** Välj om du vill anmäla användaren till produkt- och marknadsföringsmeddelanden.
      * **Endast API:** Tillåter användaren att logga in endast via API:t.

   * I avsnittet **[!UICONTROL User Details]** anger du användarens kontaktinformation, till exempel gatuadress och telefonnummer.
   * Konfigurera inställningarna som påverkar hur användaren skapar eller arbetar med korrektur i avsnittet **[!UICONTROL Default proof settings]**.

      * **Standardkorrekturroll:** Välj en standardkorrekturroll för användaren. Rollalternativen är **[!UICONTROL Read only]**, **[!UICONTROL Reviewer]**, **[!UICONTROL Approver]**, **[!UICONTROL Reviewer & Approver]**, **[!UICONTROL Author]** eller **[!UICONTROL Moderator]**.

        Mer information om korrekturroller finns i [Hantera korrekturroller i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

      * **Lås korrekturet när alla beslut fattas:** Lås automatiskt korrekturet från ytterligare ändringar när alla beslut om korrekturet har fattats.
      * **Inloggning krävs. Korrektur kan bara delas med andra användare:** Gör korrekturet tillgängligt endast för användare med inloggningsuppgifter för [!DNL Workfront Proof].
      * **Endast ett beslut krävs:** Endast ett beslut krävs för ett bevis.
      * **Hämta originalfilen:** Används för att hämta originalfilen för ett korrektur. Det här alternativet är aktiverat som standard.

        Mer information om hur du hämtar originalfiler finns i [Hämta filer lagrade i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).

        <!--      
        <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Public sharing. The proof can be shared via a public URL or embedded code:</strong>Enables the user to share proofs via a public URL or embed code.<br>This option is enabled by default but is not available if the&nbsp;<strong>Login required</strong>option is selected.<br>For more information on sharing proofs, see "<a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md" class="MCXref xref" xrefformat="{para}">Share the Public URL in Workfront Proof</a>."</li>      
        -->

      * **Prenumeration. Användarna kan registrera sig för korrekturet via den offentliga URL:en eller inbäddningskoden** Tillåter granskare utanför organisationen att registrera sig för korrekturet via den offentliga URL:en eller inbäddningskoden.

        När det här alternativet är markerat måste **prenumeranten klicka på en länk i ett e-postmeddelande för att få tillgång till ett bevis** är också tillgängligt. Välj det här alternativet om du vill att den externa granskaren ska klicka på en länk i e-postmeddelandet för att få åtkomst till korrekturet.
Det här alternativet är aktiverat som standard om alternativet **Offentlig delning** är markerat.

      * **Standardroll för nya gästgranskare:** Välj en standardkorrekturroll för gästgranskare. Alternativen är desamma som de i **Standardkorrekturrollen**, med undantag för Moderator och Författare.

   * I avsnittet **[!UICONTROL Default email alert settings]**:

      * **Standardvarning för e-post:** Ange hur ofta användaren får e-postuppdateringar. Välj **Alla aktiviteter, Svara på mina kommentarer, Beslut, Slutligt beslut, Sammanfattning varje timme, Sammanfattning varje dag,** eller **Inaktiverad**.

        Mer information om standardalternativ för e-postavisering finns i [Konfigurera e-postaviseringsinställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md)

      * **Standardmeddelande för nya gästgranskare:** Ange hur ofta gästgranskare ska få e-postuppdateringar. Alternativen är desamma som för **Standardavisering via e-post.**

      * **Skicka en e-postbekräftelse när korrektur är klara:** Välj att automatiskt skicka en bekräftelse via e-post när korrektur är klara.
      * **Format för e-post som skickas till den här användaren:** Välj **[!UICONTROL HTML]** eller **[!UICONTROL Plain text]** som standardformat för e-post som skickas till användaren.

   * I avsnittet **[!UICONTROL Custom message settings]**: Skapa inställningar för korrekturmallar.

     Mer information om mallar finns i:

      * **Ämnesmall för korrektur:** Skapa en mall för ett korrekturämne.
      * **Mallen för korrekturmeddelanden:** Skapa en mall för ett korrekturmeddelande och dess format.
