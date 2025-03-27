---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Enkel inloggning i  [!DNL Workfront Proof]: AD FS-konfiguration'
description: Om du är administratör på AD-servern kan du installera och konfigurera AD FS.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: 690b0817dfe4ff200982ffe8d67ad93e563e30ac
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 0%

---

# Enkel inloggning i [!DNL Workfront Proof]: AD FS-konfiguration

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om du är administratör på AD-servern kan du installera och konfigurera AD FS.

## Installera och konfigurera AD FS

1. Hämta Microsoft AD FS 2.0 till datorn.
1. Öppna den hämtade filen AdfsSetup.exe för att starta installationsguiden för ADFS (Active Directory Federation Services).
1. På skärmen Serverroll väljer du ett av alternativen (du behöver minst en federationsserver).
1. Om du inte vill visa IIS på AD-servern för Internet (portarna 80 och 443 för HTTP och HTTPS), kan du först konfigurera en federationsserver bakom brandväggen och sedan skapa en andra federationsserverproxy som skickar begäranden genom brandväggen till federationsservern.
1. När du har slutfört AD FS-konfigurationen väljer du **[!UICONTROL Start the AD FS 2.0 Management snap-in]** och klickar sedan på **[!UICONTROL Finish]**. När detta är klart öppnas AD FS 2.0-hanteringsfönstret med en gång. Annars kan du öppna den från **[!UICONTROL Start]** > **[!UICONTROL Administrative Tools]** > **[!UICONTROL AD FS 2.0 Management]**. Detta är huvudprogrammet för AD FS-kontroll.

1. Börja med att klicka på konfigurationsguiden för AD FS 2.0-federationsserver.
Detta hjälper dig att konfigurera AD FS och ansluta det till både Internet via IIS och till AD.
1. Om du konfigurerar en ny AD FS-server väljer du **[!UICONTROL Create a new Federation Service]**.
1. Välj **[!UICONTROL Stand-alone federation server]** (för testnings- och utvärderingssyften).

1. Klicka på Ny federationsservergrupp för hög tillgänglighet och belastningsutjämning.
1. Ange federationstjänstens namn.
Som standard hämtar konfigurationsguiden det SSL-certifikat som är bundet till standardwebbplatsen i IIS och använder ämnesnamnet som anges där. Om du använder ett jokertecken måste du ange namnet på federationstjänsten.
Om inget SSL-certifikat har konfigurerats i IIS söker konfigurationsguiden i det lokala datorns certifikatarkiv efter giltiga certifikat. De här visningarna visas i listrutan för SSL-certifikat. Om det inte finns några certifikat kan du använda Server Certificate Generator i IIS för att skapa ett.

1. Fortsätt med konfigurationen och klicka på **[!UICONTROL Close]** när den är klar.

## Konfigurerar [!DNL Workfront Proof] enkel inloggning

Om du är [!DNL Workfront Proof]-administratör kan du konfigurera enkel inloggning på [!DNL Workfront Proof]-sidan. Mer information finns i [enkel inloggning i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** och öppna sedan fliken **[!UICONTROL Single sign-on]**.

1. Klistra in ditt enhets-ID i rutan **SSO-URL** .
Följande är ett exempel på ett enhets-ID:
http://*&lt;adfs.your-company.com>*/adfs/services/trust
Ditt enhets-ID finns i din Federationsmetadatas XML-fil.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. Federationsmetadata finns i snapin-modulen AD FS 2.0 > Service > Endpoints-mappen. I avsnittet Metadata letar du reda på den som har typen Federationsmetadata. Klistra in slutpunkten i webbläsaren om du vill visa metadata. Du kan också gå till den här länken direkt: https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml när du har ersatt {adfs.your-company.com} med dina egna uppgifter.
1. Klistra in din SSO-inloggning i rutan **[!UICONTROL Login URL]**.
1. Följande är ett exempel på en SSO-inloggning:
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. Länken finns i XML-filen för federationsmetadata.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. Ange länken i rutan **[!UICONTROL Logout URL]** och spara.
Följande är ett exempel på en URL för utloggning:
https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. Gå till AD FS-hanteraren > Lita på relationer > Förlitande partsförtroenden - Korrekturegenskaper.
   1. Klicka på [!UICONTROL Add and entry] under slutpunkterna med följande information:

      * Slutpunktstyp = SAML-utloggning
      * Bindning = POST
      * URL = https://*&lt;adfs.your-company.com*>/adfs/ls/?wa=wsignout1.0
      * Det här steget kan slutföras när du har konfigurerat förlitande part-förtroendet (se nedan) i din AD FS.
   1. Ange data från ditt certifikat i rutan **[!UICONTROL Certificate fingerprint]**.
   1. Gå till snapin-modulen ADFS 2.0 och navigera till Service > Certifikat > Tokensignering.
   1. Högerklicka på den här posten för att visa certifikatet.
   1. Kopiera tumavtrycket från fliken [!UICONTROL Certificate Details] och klistra in det på konfigurationsfliken **[!UICONTROL Workfront Proof Single Sign-On]**.

   1. Fingeravtryckstecknen kan separeras med kolon eller mellanslag, men vi rekommenderar att du tar bort dessa. Om du har problem med konfigurationen för enkel inloggning kontaktar du kundsupport.


## Lägga till ett förlitande part-förtroende

När konfigurationen är klar måste du arbeta i avsnittet Förlitande partsförtroenden i din AD FS.

1. Navigera till mappen **[!UICONTROL Trust Relationships]** > **[!UICONTROL Relying Party Trusts]** och klicka sedan på **[!UICONTROL Add a Relying Party Trust]** för att starta konfigurationsguiden.

1. Välj datakälla.
Alla metadata för ditt [!DNL ProofHQ]-konto finns under en länk som den här:
https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq
Detta konfigurerar merparten av förlitande part-förtroendet.

   >[!NOTE]
   >
   >* Om du har problem med att upprätta anslutningen från URL:en sparar du metadata som en fil och väljer att importera data från en fil.
   >* När du har konfigurerat en fullständig anpassad domän (t.ex. www.your-proofing.com) på ditt [!DNL ProofHQ]-konto ersätter du hela delen {yoursubdomain}.proofhq.com med din egen domän för att skapa din [!DNL ProofHQ]-metadatalänk.


## Konfigurera anspråksregler

När konfigurationen av förlitande part-förtroende är klar kan du konfigurera anspråksreglerna så att konfigurationen slutförs. Du konfigurerar två anspråksregler för Korrektur för huvudkontor: E-post och Namn-ID.

1. Öppna dialogrutan **[!UICONTROL Edit Claim Rules]**.
1. Gå till **[!UICONTROL ProofHQ Relying Party Trust]** och klicka sedan på **[!UICONTROL Edit Claim Rules]** (1).\
   Popup-fönstret bör öppnas automatiskt om du har valt det här alternativet när du har konfigurerat förtroendet.

1. Klicka på **[!UICONTROL Add Rule]** (2) för att öppna anspråkskonfigurationsfönstret.

   * E-post (Skicka LDAP-attribut som anspråksregelmall)
   * NameID (transformera en regelmall för inkommande anspråk)
