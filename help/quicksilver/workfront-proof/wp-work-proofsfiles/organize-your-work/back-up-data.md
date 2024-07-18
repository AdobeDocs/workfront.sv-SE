---
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Säkerhetskopiera dina [!DNL Workfront Proof] data
description: Du kan begära en säkerhetskopia av alla dina data i  [!DNL Workfront Proof] med hjälp av säkerhetskopieringsfunktionen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 3b831bb5-2d03-4d7e-ad1f-54ae95f05ccd
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1020'
ht-degree: 0%

---

# Säkerhetskopiera dina [!DNL Workfront Proof]-data

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

## Introduktion till säkerhetskopiering

Du kan begära en säkerhetskopia av alla dina data i [!DNL Workfront Proof] med hjälp av säkerhetskopieringsfunktionen.

Säkerhetskopian levereras till dig som en ZIP-fil. Den innehåller en XML-export av alla dina data (inklusive kommentarer och svar för alla versioner av alla korrektur), men inte de originalfiler som du överfört som korrektur.

Varje ZIP-fil för säkerhetskopiering som du skapar för nedladdning har ett unikt filnamn, till exempel:

9789_05_05_2011_61703.zip

Filnamnet i det här exemplet innehåller följande information:

* 9789 är din [!DNL Workfront Proof]-kontoidentifierare
* 05_05_2011 är skapandedatumet den 5 maj 2011
* 61703 är ett slumpmässigt systemtilldelat nummer

Den här namnkonventionen gör det enkelt för dig att lagra alla dina säkerhetskopierade ZIP-filer på en enda plats på datorn och att veta exakt när varje säkerhetskopia skapades åt dig.

Med funktionen [!UICONTROL Backup] kan du bestämma hur du vill använda dina resurser:

* Du kan frigöra lagringsutrymme utan att förlora aktiva eller arkiverade korrektur. Du kan begära en säkerhetskopia, ta bort korrektur och sedan tömma [Återställ och töm papperskorgen i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).
* Gör att du kan komma åt alla filer som du ursprungligen överförde till [!DNL Workfront]-korrektur. Du kan hämta dem med funktionen [!UICONTROL download original file] innan du tar bort korrektur.

>[!NOTE]
>
>Tänk på följande när du använder säkerhetskopior:
>
>* Säkerhetskopior är tillgängliga för Enterprise-planer och Obegränsat-planer. Kontakta vårt [säljteam](mailto:sales@proofhq.com) om du vill ha en offert.
>* Datakodningstypen är inställd på UTF-8 som standard och vi rekommenderar den här inställningen. Detta är den kodningstyp som oftast används av Internet-program.
>* Du kan bara begära en [!DNL backup] åt gången. När säkerhetskopian av ZIP-filen bearbetas visas inte länken Begär ny säkerhetskopiering på fliken Säkerhetskopior och meddelandet som visas ändras inte. Mer information om hur du begär en säkerhetskopiering finns i [Begär en ny säkerhetskopiering av data i [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/request-new-data-backup-in-wp.md).
>



## Säkerhetskopiera data

1. Klicka på **[!UICONTROL Account settings]** i det övre högra hörnet av [!DNL Workfront Proof]-gränssnittet. (1)
1. Klicka på fliken **[!UICONTROL Backups]**. (2)
1. Klicka på länken **[!UICONTROL Request new backup]** (3)

När säkerhetskopieringen är klar händer följande:

* Du får ett e-postmeddelande från [!DNL Workfront Proof] som meddelar dig om detta (&quot;Din [!DNL Workfront Proof]-säkerhetskopiering är klar&quot;). E-postmeddelandet innehåller en nedladdningslänk för dina säkerhetskopierade data.
* På fliken [Kontoinställningar](https://support.workfront.com/hc/en-us/sections/115000912147-Account-settings) Säkerhetskopiering visas en nedladdningslänk för dina säkerhetskopieringsdata.
* Länken Begär ny säkerhetskopiering (3) visas igen på fliken Säkerhetskopior

Dina data kommer att kunna hämtas som en zip-fil. Du kan hämta ZIP-filen för säkerhetskopiering antingen från e-postmeddelandet eller i [!UICONTROL account settings], vilket beskrivs i följande avsnitt:

* [Hämtar säkerhetskopian av ZIP-filen från e-postmeddelandet](#downloading-your-backup-zip-file-from-your-email-notification)
* [Hämtar säkerhetskopian av ZIP-filen från kontoinställningarna](#downloading-your-backup-zip-file-from-the-account-settings)

![Request_Backup.png](assets/request-backup-350x167.png)

## Hämtar säkerhetskopian av ZIP-filen från e-postmeddelandet {#downloading-your-backup-zip-file-from-your-email-notification}

När säkerhetskopian av ZIP-filen är klar att laddas ned får du ett e-postmeddelande från [!DNL Workfront Proof] med ämnesraden &quot;Säkerhetskopieringen av [!DNL Workfront Proof] är klar.&quot;

Så här hämtar du den säkerhetskopierade ZIP-filen från e-postmeddelandet:

1. Klicka på nedladdningslänken i e-postmeddelandet.\
   ![Backup_mail.png](assets/backup-mail-350x120.png)\
   Om du inte är inloggad på [!DNL Workfront Proof] öppnas ett nytt webbläsarfönster där inloggningssidan visas.

## Hämtar säkerhetskopian av ZIP-filen från kontoinställningarna {#downloading-your-backup-zip-file-from-the-account-settings}

När säkerhetskopian av ZIP-filen är klar att laddas ned visas en nedladdningslänk på fliken [!UICONTROL Backup]. Dessutom visas länken [!UICONTROL Request new backup] igen.

1. Klicka på **[!UICONTROL Account settings]** i det övre högra hörnet av [!DNL Workfront Proof]-gränssnittet. (1)
1. Klicka på fliken **[!UICONTROL Backups]**. (2)\
   Om inga användare på ditt konto har begärt några säkerhetskopior visar fliken [!UICONTROL Backups] att du inte har några säkerhetskopior. Om en användare har begärt en säkerhetskopiering visar fliken skapandedatum och hämtningslänk för den senaste säkerhetskopieringen.

1. Klicka på länken **[!UICONTROL Download backup]**. (3)\
   ![Download_Backup.png](assets/download-backup-350x167.png) Ett fönster för filhämtning visas där du tillfrågas om du vill öppna eller spara den hämtade filen.

1. Klicka på **[!UICONTROL Save]** och välj sedan den plats på datorn där du vill spara ZIP-filen för säkerhetskopian.\
   Meddelandet som identifierar datumet för den senaste säkerhetskopian visas längst ned på sidan [!UICONTROL Backup] tills nästa gång du begär en säkerhetskopiering. Länken Hämta säkerhetskopia gäller för den senaste säkerhetskopian. När länken [!UICONTROL Request new backup] visas kan du klicka på den och begära en ny säkerhetskopia.

## Förstå filerna i ZIP-filen för säkerhetskopiering

ZIP-filen för säkerhetskopian innehåller sju CSV-filer (kommaavgränsade värden eller kommaavgränsade) som innehåller information från dina aktiva och arkiverade korrektur fram till säkerhetskopieringen:

* comments.csv - innehåller kommentarer om korrektur
* comment_responses.csv - innehåller svar på kommentarer om korrektur organisation.csv - innehåller numerisk identifierare och namnet på din organisation (ditt konto)
* contact.csv - innehåller numerisk identifierare, namn och organisation för varje kontakt
* files.csv - innehåller information från sidan Korrekturinformation eller sidan Filinformation om korrektur eller filer som överförts till [!DNL Workfront Proof]
* templates.csv - innehåller numerisk identifierare, roll och beslut för varje person som angetts som granskare, granskare och godkännare, osv. när korrektur överförs för granskning den [!DNL Workfront Proof]
* users.csv - innehåller numeriska identifierare och namn för alla användare i kontot

Du kan extrahera dessa filer från ZIP-filen för säkerhetskopiering med vilket ZIP-verktyg som helst och sedan lagra dem på valfri plats på datorn. När du har sparat zip-filen och extraherat de enskilda CSV-filerna kan du ändra informationen så som du vill för den interna arkiveringen.

Varje ZIP-fil för säkerhetskopiering som skapas på din begäran har ett unikt namn som inkluderar datumet då säkerhetskopian skapades, men CSV-filerna som ingår i varje ZIP-fil för säkerhetskopiering har alltid samma namn. Du kanske vill använda någon av följande metoder för att se till att säkerhetskopieringsfilerna skiljer sig från varandra:

* Skapa en ny mapp för varje ZIP-fil för säkerhetskopiering och de CSV-filer som du extraherar från den.
* Byt namn på varje enskild CSV-fil så att den innehåller säkerhetskopieringsdatumet när du extraherar den från zip-filen.

>[!NOTE]
>
>Om [!DNL Microsoft Excel] är installerat på datorn kan extraheringsverktyget visa filtypen för de enskilda CSV-filerna som [!DNL Microsoft Office Excel] kommaseparerad värdefil. Du kan öppna en extraherad CSV-fil med [!DNL Excel] och spara filen som en [!DNL Excel]-arbetsbok (&#42;.xlsx) eller någon annan filtyp.
