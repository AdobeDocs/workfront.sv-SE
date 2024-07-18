---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: Hantera korrekturroller i  [!DNL Workfront Proof]
description: Korrekturroller gör att du kan bevilja behörigheter till användare som begränsas av den behörighetsprofil som är konfigurerad för deras användarprofil.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 6e24b9c717ecedd6efbdf62ec01e53ac98079cfe
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 0%

---

# Hantera korrekturroller i [!DNL Workfront Proof]

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Korrekturroller gör att du kan bevilja behörigheter till användare som begränsas av den behörighetsprofil som är konfigurerad för deras användarprofil. (Mer information om behörighetsprofiler finns i [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

Korrekturroller skiljer sig från kontoprofiler. Din kontoprofil gäller den övergripande behörighetsnivå som du har på ditt konto och påverkar de rättigheter som du har för alla korrektur i ditt konto, även de som inte har delats med dig.

Mer information finns i [Korrekturbehörighetsprofiler i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Om korrekturroller

Följande korrekturroller ges till användare för ett enskilt korrektur när användaren blir inbjuden att granska beviset:

* [Skrivskyddad](#read-only)
* [Granskare](#reviewer)
* [Godkännare](#approver)
* [Granskare och godkännare](#reviewer-approver)
* [Upphovsman](#author)
* [Moderator](#moderator)

Korrekturrollen definierar vilka åtgärder en granskare kan vidta i förhållande till det specifika korrekturet.

Om du till exempel är en granskare blir du ombedd att granska korrekturet genom att lägga till markeringar och kommentarer. Om du är granskare och godkännare blir du ombedd att granska och även fatta ett beslut om beviset.

Vissa korrekturroller ger en granskare redigeringsbehörighet för korrekturet (även om deras kontoprofil inte tillåter det) och låter dem använda ytterligare funktioner som att lägga till åtgärder i kommentarer, skapa nya versioner och lägga till fler granskare till korrekturet.

Mer information finns i följande artiklar:

* [Använda funktionsmakron för korrekturkommentarer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [Dela ett korrektur i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### Skrivskyddad

{#read-only}

![cleaner.png](assets/cleaner.png) Kan visa ett korrektur

![no.png](assets/no.png) Det går inte att lägga till markeringar

![no.png](assets/no.png) Det går inte att lägga till kommentarer

![no.png](assets/no.png) Det går inte att fatta ett beslut

![no.png](assets/no.png) Det går inte att ta bort kommentarer som gjorts av andra

![no.png](assets/no.png) Har inte redigeringsbehörighet för korrekturet

>[!NOTE]
>
>Om en mapp delas med en användare av [!DNL Workfront Proof] får de automatiskt skrivskyddad behörighet till alla befintliga och efterföljande objekt i mappen.

Mer information finns i [Dela mappar i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### Granskare {#reviewer}

![cleaner.png](assets/cleaner.png) Kan visa ett korrektur

![cleaner.png](assets/cleaner.png) Kan lägga till markeringar

![cleaner.png](assets/cleaner.png) Kan lägga till kommentarer

![[!DNL cleaner].png](assets/cleaner.png) Kan redigera egna kommentarer om det inte finns några svar

![no.png](assets/no.png) Det går inte att fatta ett beslut

![no.png](assets/no.png) Det går inte att redigera eller ta bort kommentarer som gjorts av andra

![no.png](assets/no.png) Har inte redigeringsbehörighet för korrekturet

### Godkännare {#approver}

![cleaner.png](assets/cleaner.png) Kan visa ett korrektur

![cleaner.png](assets/cleaner.png) Kan fatta ett beslut

![no.png](assets/no.png) Det går inte att lägga till markeringar

![no.png](assets/no.png) Det går inte att lägga till kommentarer

![no.png](assets/no.png) Det går inte att redigera eller ta bort kommentarer som gjorts av andra

![no.png](assets/no.png) Har inte redigeringsbehörighet för korrekturet

### Granskare och godkännare {#reviewer-approver}

![cleaner.png](assets/cleaner.png) Kan visa ett korrektur

![cleaner.png](assets/cleaner.png) Kan lägga till markeringar

![cleaner.png](assets/cleaner.png) Kan lägga till kommentarer

![[!DNL cleaner].png](assets/cleaner.png) Kan redigera egna kommentarer om det inte finns några svar

![cleaner.png](assets/cleaner.png) Kan fatta ett beslut

![no.png](assets/no.png) Det går inte att redigera eller ta bort kommentarer som gjorts av andra

![no.png](assets/no.png) Har inte redigeringsbehörighet för korrekturet

### Upphovsman {#author}

![cleaner.png](assets/cleaner.png) Kan lägga till markeringar

![cleaner.png](assets/cleaner.png) Kan lägga till kommentarer

![[!DNL cleaner].png](assets/cleaner.png) Kan redigera egna kommentarer om det inte finns några svar

![cleaner.png](assets/cleaner.png) Kan fatta ett beslut

![cleaner.png](assets/cleaner.png) Kan skicka nya versioner

![cleaner.png](assets/cleaner.png) Kan skapa en kopia av korrekturet

![cleaner.png](assets/cleaner.png) Kan dela korrekturet med andra

![cleaner.png](assets/cleaner.png) Kan använda åtgärder på kommentarer

![cleaner.png](assets/cleaner.png) Kan lösa kommentarer

![no.png](assets/no.png) Det går inte att redigera eller ta bort kommentarer som gjorts av andra

>[!NOTE]
>
>Den här rollen kan endast tilldelas användare av [!DNL Workfront Proof].

### Moderator {#moderator}

![cleaner.png](assets/cleaner.png) Kan lägga till markeringar

![cleaner.png](assets/cleaner.png) Kan lägga till kommentarer

![[!DNL cleaner].png](assets/cleaner.png) Kan redigera egna kommentarer om det inte finns några svar

![cleaner.png](assets/cleaner.png) Kan fatta ett beslut

![cleaner.png](assets/cleaner.png) Kan skicka nya versioner

![cleaner.png](assets/cleaner.png) Kan lägga till nya granskare

![cleaner.png](assets/cleaner.png) Kan använda åtgärder på kommentarer

![cleaner.png](assets/cleaner.png) Kan lösa kommentarer

![cleaner.png](assets/cleaner.png) Kan ta bort kommentarer och svar på korrekturet (görs av sig själv eller av andra)

* Om du tar bort den första kommentaren i en kommentarstråd tas hela tråden bort
* Om du tar bort svar i kommentarstråden tas endast det svaret bort

![no.png](assets/no.png) Det går inte att redigera kommentarer som gjorts av andra

Med den här rollen kan man hantera och moderera korrekturkommentarerna, så att de bara kan behålla relevanta kommentarer på beviset och ta bort icke-relevanta kommentarer.

>[!NOTE]
>
>Den här rollen kan endast tilldelas användare av [!DNL Workfront Proof].

## Tilldela korrekturroller

Du kan tilldela korrekturroller när du skapar nya korrektur, skapar nya versioner av befintliga korrektur eller på befintliga korrektur.

### Nya korrektur {#new-proofs}

Bevisroller kan tilldelas granskare på sidan [!UICONTROL New proof] när korrektur skapas (1).

![Korrektur_roles_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### Nya versioner {#new-versions}

När du skapar en ny version av ett korrektur visas granskarna från den tidigare versionen automatiskt (med samma roll som den föregående versionen).

Du kan redigera korrekturrollerna som tillämpas på granskarna när du skapar den nya versionen (1).

![Proof_roles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### Befintliga korrektur {#existing-proofs}

Om du vill ändra en persons roll för ett befintligt korrektur kan du göra det på sidan [!UICONTROL Proof details] genom att redigera personens roll i arbetsflödesavsnittet (1).

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## Kontrollera roller i korrekturläsaren

Du kan kontrollera rollen som granskare direkt i korrekturläsaren (1) och redigera den (2) om det behövs.

![Proof_roles_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## Roller för standardkorrektur

Du kan ange din standardkorrekturroll på sidan [!DNL Proofing Defaults] i dina personliga inställningar. Det innebär att när du läggs till i ett korrektur fylls din standardkorrekturroll i automatiskt. Observera att den här rollen kan ändras på korrekturnivå av en användare med redigeringsbehörighet för ett korrektur.

>[!NOTE]
>
>Endast användare med administratörs- eller faktureringsadministratörsprofiler kan ändra standardinställningarna för korrektur för andra användare i sina konton.

Mer information finns i [Personliga inställningar i [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## Skapare och ägare

Skapare och ägare har fullständig redigeringsbehörighet för korrekturet.

### Skapare {#creators}

Bevisskaparen är den person som överför korrekturet i första instansen. Den som skapar korrekturet visas automatiskt i personlistan för korrekturet (i sin standardroll).

På sidan [!UICONTROL New proof] kan du tilldela en annan korrekturroll till korrekturförfattaren (utöver deras standardroll).

Det går inte att ändra eller ta bort korrekturläsaren från ett korrektur.

### Ägare {#owners}

Som standard är skaparen även ägare av korrekturet, men skaparen kan göra någon annan till korrekturägare när korrekturet skapas (på sidan [!UICONTROL New proof]).

Så här ändrar du ägare på sidan Nytt korrektur:

1. Klicka på den ändringslänk som visas bredvid skaparens namn.
1. Välj den nya ägaren i listrutan. (2)

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

När beviset har skapats går det fortfarande att ändra ägare. Alla som har redigeringsbehörighet för korrekturet kan ändra korrekturägarskapet till en annan användare via sidan [!UICONTROL Proof details] (se nedan).

Möjligheten att ändra ägare av ett korrektur är särskilt användbar när det gäller arbetsflödeshantering. Det gör att den person som ansvarar för projektet kan ta över ägarskapet av korrektur och ge dem redigeringsbehörighet för korrektur och möjlighet att visa dem i vyn [!UICONTROL My proofs].

Så här ändrar du korrekturets ägare via sidan [!UICONTROL Proof details]:

* Klicka på Åtgärder-menyn bredvid namnet på den person som du vill göra ägare.
* Välj [!UICONTROL **Skapa ägare**] i listrutan.
* Du kan också klicka i fältet [!UICONTROL **Ägare**] bredvid korrekturbilden och välja den nya ägaren i listrutan som visas.

När detta är klart visas ordet &quot;Ägare&quot; bredvid den personens namn.

>[!NOTE]
>
>Endast en användare från samma konto eller ett partnerkonto kan göras ägare av ett bevis. En användare på ett partnerkonto kan endast göras till ägare av ett bevis när:
>
>* Det finns en befintlig partnerrelation mellan kontona. Mer information finns i [Partnerkonton i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* Det finns inga anpassade fält på sidan [!UICONTROL New proof].
>* Korrektet har inte tilldelats någon mapp.
>* Inga taggar har lagts till i korrekturet.

Information om hur du tillfälligt delegerar korrekturägarskap inom [!DNL Workfront Proof] finns i [Ange tillfälliga korrekturägare i [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
