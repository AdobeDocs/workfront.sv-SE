---
content-type: overview
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: manage-security-workfront-proof
title: Elektroniska signaturer i [!DNL Workfront Proof]
description: Med elektroniska signaturer kan du förbättra säkerheten på dina korrektur och följa branschstandarder som ISO.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: caff2a03-cccc-4779-9dcc-3362c527dcb9
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Elektroniska signaturer i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Med elektroniska signaturer kan du förbättra säkerheten på dina korrektur och följa branschstandarder som ISO.

Denna inställning kan göras obligatorisk eller icke-obligatorisk på kontonivå. Om det är obligatoriskt som standard aktiveras det för alla korrektur som skapas på ditt konto och kan inte inaktiveras på korrekturnivå. Om den här inställningen är icke-obligatorisk som standard kan du aktivera/inaktivera den på korrekturnivå.

Mer information finns i .

När inställningen för elektroniska signaturer är aktiverad på ett korrektur uppmanar en ruta för elektroniska signaturer alla granskare som fattar ett beslut om korrekturet att ange sin e-postadress och sitt lösenord.

![Electronic_sig_required_box.png](assets/electronic-sig-required-box.png)

## Elektroniska signaturer på [!UICONTROL Proof Details] Sida

Om en granskare fattar sitt beslut genom att välja sitt beslut [!UICONTROL Proof details] sida (1) och [!UICONTROL Electronic Signature] En popup-ruta visas där de ombeds att ange sina uppgifter (2) och bekräfta sitt beslut (3).

I popup-fönstret visas standardmeddelandeuppsättningen (om sådan finns) och granskaren måste ange e-postadress och lösenord.

The [!UICONTROL Electronic Signature] visas i korrekturläsaren och på [!UICONTROL Proof details] sida om granskaren beslutar att fatta sitt beslut från den nivån.

![Electronic_Signature_-_Proof_Details.png](assets/electronic-signature---proof-details-350x146.png)

![Electronic_Signature_-_Proof_Details_2.png](assets/electronic-signature---proof-details-2-350x148.png)

Om [!UICONTROL Single Sign-On] alternativet är aktiverat för korrekturet. E-postadressen och lösenordsinformationen visas inte i [!UICONTROL Electronic Signature] dyker upp när du fattar ett beslut.

Efter att du klickat på [!UICONTROL Confirm] (4) på den här popup-rutan kommer granskaren att omdirigeras till [!UICONTROL Single Sign-On] sida.

När granskarens inloggningsuppgifter har angetts omdirigeras granskaren automatiskt till [!UICONTROL Proof details] sida (eller tillbaka till [!UICONTROL Proof Viewer] om beslutet fattas därifrån).

![Electronic_Signature_SSO_-_Proof_Details_3.png](assets/electronic-signature-sso---proof-details-3-350x146.png)

>[!NOTE]
>
> Om beslutet undertecknas elektroniskt ska **[!UICONTROL signature icon]** (5) visas bredvid beslutet i [!UICONTROL Workflow] i [!UICONTROL Proof details] sida. Om beslutet inte ändras av granskaren utan av en annan person som har redigeringsbehörighet för beviset, kommer den personen inte att uppmanas att signera beslutet elektroniskt och det kommer inte att finnas någon signeringsikon bredvid beslutet (6).

![Electronic_Signature_icon.png](assets/electronic-signature-icon-350x52.png)Mer information om enkel inloggning finns i [Enkel inloggning i Workfront-korrektur](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

Mer information om sidan Korrekturinformation finns i [Hantera korrekturinformation i [!DNL Workfront] Korrektur](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
