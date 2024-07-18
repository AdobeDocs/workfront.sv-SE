---
filename: troubleshooting-proof-creation-failures
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: use-the-desktop-proofing-viewer
title: Felsöka fel vid korrekturskapande
description: Processen för att skapa korrektur innefattar både import- och korrekturgenerering. När du skapar ett korrektur kan det hända att en fil inte kan importeras eller att korrekturet inte kan genereras när filen har importerats.
author: Courtney
source-git-commit: de30bd970bda06c706e5156d5195e8568558e593
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---


# Felsöka fel vid korrekturskapande

Processen för att skapa korrektur innefattar både import- och korrekturgenerering. När du skapar ett korrektur kan det hända att en fil inte kan importeras eller att korrekturet inte kan genereras när filen har importerats.

>[!NOTE]
>
> Om det dokument du försöker bestyrka inte uppfyller något av villkoren i detta avsnitt kan du kontakta Adobe Workfront Support för ytterligare frågor.

## Orsaker till importfel

* Du har skapat ett kombinerat korrektur som innehåller över 50 filer.

## Orsaker till fel vid bevisgenerering

* Filtypen stöds inte.\
  En lista över filtyper som stöds finns i [Översikt över filtyper och storleksbegränsningar som stöds](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

* Filstrukturen är inte en standardstruktur för filtypen.
* Filen skyddas av ett lösenord eller så har innehållskopiering inaktiverat.

  Till skillnad från andra typer av filer kan PDF-filer genereras i korrektur om säkerhetsinställningen för kopiering av innehåll är inställd på Tillåt på PDF.

* Sidlängden eller sidantalet överskrider gränsen.

  Den högsta tillåtna sidlängden är 195 tum efter rastrering. Det högsta tillåtna sidantalet är 1 000 sidor för ett enda korrektur.

* Filen är skadad.
* Arbetsflödets deadline för en ny korrekturversion har redan inträffat.

  Detta inträffar när du skapar en ny korrekturversion med en snabbkorrekturmetod och **automatiskt genererar korrektur när du överför dokument** väljs. Den nya korrekturversionen försöker ta arbetsflödets deadlines från det tidigare genererade korrekturet. Korrekturgenerering misslyckas om den här tidsgränsen redan har nåtts. Du kan åtgärda detta genom att ange arbetsflödets deadlines för den föregående versionen i framtiden eller skapa en ny korrekturversion. Om du genererar en ny version använder du **Mer > Ny version > Korrektur** och väljer **Arbetsflödets slutdatum i framtiden**.

* Vid korrektur av PDF-filer kan orsaken till fel vid korrekturgenerering vara:

   * Teckensnitt och bilder länkas från externa källor (t.ex. från det lokala filsystemet)

     Teckensnitt och bilder måste vara inbäddade i filen PDF för att kunna visas på en annan dator eller i Workfront Proof.

   * Filen PDF innehåller tomma lager eller genomskinliga eller överlappande fält.

     Om du inte kan avgöra vilket lager eller objekt som orsakar detta exporterar du designen/dokumentet som en optimerad PDF (då tas alla oönskade element bort).

