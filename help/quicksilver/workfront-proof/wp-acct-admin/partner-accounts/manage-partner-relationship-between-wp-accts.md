---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: partner-accounts
title: Hantera en partnerrelation mellan  [!DNL Workfront Proof] konton
description: Om du samarbetar med en annan organisation som även använder en  [!DNL Workfront Proof]  (till exempel en annan avdelning i ditt företag eller en klient) kan du skapa en partnerrelation mellan de två kontona. Om du skapar en partnerrelation mellan ditt konto och en annan organisation kan du dela korrektur, filer, mappar och kontaktinformation med dina partner.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ee06c9a7-baeb-4c2b-a6c5-ec4ac542dd5a
source-git-commit: 405523606094d4f8553b0aee544d71c2b7f97d86
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Hantera en partnerrelation mellan [!DNL Workfront Proof]-konton

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om du samarbetar med en annan organisation som även använder [!DNL Workfront Proof] (till exempel en annan avdelning i ditt företag eller en klient) kan du skapa en partnerrelation mellan de två kontona. Om du skapar en partnerrelation mellan ditt konto och en annan organisation kan du dela korrektur, filer, mappar och kontaktinformation med dina partner.

Partnerrelationen upprättas mellan två organisationer i stället för mellan två användare, och båda organisationerna måste ha ett [!DNL Workfront Proof]-konto.

>[!NOTE]
>
>Användarna från partnerkontot visas som medlemmar i ditt konto och vice versa. Om din partner lägger till en ny användare i sitt konto visas den nya användaren automatiskt som medlem på din kontaktsida. När du lägger till en ny användare till ditt konto visas den nya användaren som medlem på din partners kontaktsida.

## Skicka en partnerbegäran

Endast användare med [!UICONTROL Administrator]- eller [!UICONTROL Billing Administrator]-profilbehörighet kan skicka en partnerinbjudan, eftersom åtkomst till [!UICONTROL Account settings] krävs för att utföra den här åtgärden.

Följ stegen nedan för att skicka en partnerbegäran:

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** och öppna sedan fliken **[!UICONTROL Partners]**.

1. Klicka på **[!UICONTROL Send new partner invitation]**.
1. I rutan **[!UICONTROL Send invitation]** som visas skriver du e-postadressen till en användare i din partnerorganisation.
1. Klicka på **[!UICONTROL Send]**.

## Godkänna en partnerbegäran

Alla [!DNL Workfont Proof]-administratörer kan acceptera en partnerbegäran, det behöver inte vara den användare vars e-postadress har angetts i inbjudan. Så här godkänner du partnerbegäran:

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** och öppna sedan fliken **[!UICONTROL Partners]**.

1. Klicka på **Acceptera**.**&#x200B;**

>[!NOTE]
>
>Partnerrelationen visas både i avsändare och på mottagarkonto på fliken [!UICONTROL Partners].

## Avslå en partnerbegäran

Alla [!DNL Workfont Proof]-administratörer kan avvisa en partnerbegäran. Status för inbjudan ändras till [!UICONTROL Rejected] i både mottagarens konto och avsändarens konto. Avsändaren får ett e-postmeddelande om att partnerrelationsbegäran har avvisats. Avsändaren kan inte skicka ytterligare en inbjudan till samma person om inte mottagaren tar bort relationen helt och hållet och avsändaren sedan gör samma sak. Det går dock att skicka flera partnerförfrågningar till olika användare på samma konto.

Så här avvisar du en partnerinbjudan:

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** och öppna sedan fliken **[!UICONTROL Partners]**.

1. Klicka på **[!UICONTROL Reject and ignore]**.

## Ta bort en partnerbegäran

Alla [!DNL Workfont Proof]-administratörer kan ta bort en partnerbegäran.

Om begäran tas bort på avsändarsidan visas inte längre inbjudan vare sig på avsändarens konto eller på mottagarens konto. En ny inbjudan kan skickas till samma e-postadress som den ursprungliga inbjudan.

Om mottagarorganisationen tar bort en inbjudan visas inbjudan inte längre på mottagarens konto, utan visas som [!UICONTROL Rejected] på avsändarens konto.

Så här tar du bort en partnerbegäran:

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** och öppna sedan fliken **[!UICONTROL Partners]**.

1. Klicka på nedpilen till höger om begäran.
1. Välj **[!UICONTROL Delete]**.

## Ta bort en befintlig partnerrelation

Det går att ta bort en befintlig partnerrelation om den inte längre behövs. När en partnerrelation tas bort behålls användarna från det tidigare partnerkontot på sidan [!UICONTROL Contacts], men eventuella framtida användare synkroniseras inte. Tidigare delade objekt förblir i det läget.

Så här tar du bort en partner:

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** och öppna sedan fliken **[!UICONTROL Partners]**.

1. Klicka på nedpilen till höger om partnern och klicka sedan på **[!UICONTROL Delete]** i listrutan.

Om avsändarorganisationen tar bort en partner tas partnerrelationen bort både från avsändarens och mottagarens konto. Om mottagarorganisationen tar bort en partner visas partnern inte längre i mottagarens konto, utan visas som [!UICONTROL Rejected] i avsändarens konto. Partnerrelationen kan återupprättas genom att en ny begäran skickas.
