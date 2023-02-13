---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: Flytta användare mellan konton med [!DNL Workfront Proof]
description: Om du är en [!DNL Workfront Proof] och du har ett eller flera satellitkonton anslutna till huvudkontot, kan du flytta användarna mellan alla dessa konton.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Flytta användare mellan konton med [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Om du är en [!DNL Workfront] Korrekturadministratör och du har ett eller flera satellitkonton anslutna till huvudkontot, kan du flytta användarna mellan alla dessa konton.

## Flytta användare mellan anslutna konton

1. Klicka på **[!UICONTROL Settings]** > **[!UICONTROL Account settings]**.

1. Öppna **[!UICONTROL Users]** -fliken.
1. Klicka på **[!UICONTROL Move user]** ikon (1). ![Move_user2.png](assets/move-user2-350x95.png)

1. I rutan Flytta användare som visas bekräftar du den användare som du vill flytta (1).
1. Välj ett destinationskonto i listan med anslutna konton (2).
1. Tilldela profilbehörigheten (3) som den här användaren ska ha på det nya kontot.
1. Välj en användare (4) som ska överta ägarskapet för de objekt som inte ska flyttas.
Detta inkluderar de objekt som du bestämmer dig för att lämna på det gamla kontot och de objekt som inte kan flyttas (se [Objekt som inte kan flyttas](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved) nedan).

1. Markera kryssrutorna om du vill flytta korrektur (5) och filer (6) tillsammans med användaren.
1. Skapa ett namn för mappen (7) där alla flyttade objekt placeras på det nya kontot.
1. Klicka **[!UICONTROL Move user]** (8) för att påbörja processen.
   ![Moving_users_pop-up.png](assets/moving-users-pop-up-350x380.png)

Om du väljer att flytta användaren utan sina korrektur och filer utförs den här åtgärden direkt. Om du väljer att flytta användaren tillsammans med sina korrektur och filer, kommer användarens profil att omtilldelas direkt, men korrekturen och filerna kommer gradvis att visas på målkontot eftersom den här åtgärden tar tid att överföra data.

Beroende på hur många filer och korrektur det kan ta mellan några minuter och några timmar att flytta.

>[!NOTE]
>
>Om du misstänker att processen tar längre tid än förväntat eller om de flyttade korrekturen och/eller filerna inte visas på det nya kontot kontaktar du vårt supportteam.

## Objekt som inte kan flyttas

### Mappar som har skapats eller ägs av den flyttade användaren

På grund av den typ av behörigheter som tillämpas på mappar och dess innehåll (t.ex. att de delas med andra användare och konton) kan vi inte flytta mappstrukturer med användaren.

Om en mapp ägs av den flyttade användaren överförs ägarskapet till den valda användaren (4) i popup-fönstret Flytta användare.

>[!NOTE]
>
>Om en mapp har skapats av den flyttade användaren förblir användaren skapare - endast ägarskapet överförs. Mappen är fortfarande synlig för den flyttade användaren i sidofältet för det nya kontot. Den flyttade användaren har fortfarande skrivskyddad åtkomst till de objekt som finns i mapparna.

Om du inte vill att den flyttade användaren ska behålla dessa behörigheter eller om den flyttade användaren inte vill se sina gamla mappar på det gamla &amp;kontot, är lösningen här att ta bort mapparna enligt följande:

1. Skapa en ny mapp på det gamla kontot.
1. Flytta alla objekt från den flyttade användarens mappar till den nya.
1. Ta bort alla mappar som finns kvar av den flyttade användaren.

### Versionsuppsättningar med olika ägare

Om ett bevis har ett fåtal versioner och var och en av dem ägs av en annan användare flyttas inte de versioner som ägs av den flyttade användaren. Ägarskapet för sådana versioner överförs till en annan användare enligt ditt val (4) i rutan Flytta användare. (Mer information finns i .)

>[!NOTE]
>
>En flyttad användare måste äga alla korrekturversioner i uppsättningen för att beviset ska kunna flyttas.

### Grupper

Grupper måste återskapas av den flyttade användaren på deras nya konto. Mer information finns i [Skapa korrekturgrupper med [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).

### Anpassade vyer

Personliga anpassade vyer måste återskapas av den flyttade användaren på deras nya konto. Mer information finns i [Skapa och hantera anpassade vyer i [!DNL Workfront Proof] Korrektur](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### Anpassade fält

Det går inte att flytta anpassade fält och data från anpassade fält går förlorade. Se därför till att du genererar rapporter om de nödvändiga objekten innan du flyttar dem.

### Automatiserade arbetsflödesmallar

Automatiserade arbetsflödesmallar måste återskapas på det nya kontot, men stegen behålls på de flyttade korrektur som skapats med mallarna.

### Åtgärder för kommentarer

Funktionsmakron för kommentarer finns kvar på korrekturet, men det går inte att filtrera efter dem längre. Lösningen skulle vara att skapa matchande åtgärder på det nya kontot och flagga om kommentarerna med de nya åtgärderna om det behövs.
