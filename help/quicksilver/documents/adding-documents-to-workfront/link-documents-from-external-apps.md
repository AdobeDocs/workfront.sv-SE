---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Länka dokument från externa program
description: Du kan länka dokument och mappar till Adobe Workfront från externa källor.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '2620'
ht-degree: 0%

---

# Länka dokument från externa program

<!-- Audited: 01/2024 -->

Du kan länka dokument och mappar till Adobe Workfront från följande källor:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Befintliga dokumentleverantörer i molnet från tredje part</td> 
   <td>Bland dessa finns följande: 
    <ul> 
     <li>Box</li> 
     <li>Dropbox</li> 
     <li>Dropbox Business</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Microsoft SharePoint</li> 
     <li>Google Drive</li> 
     <li>Snabbhet</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof </td> 
   <td>Du kan göra korrektur som ursprungligen skapades i Workfront Proof tillgängliga i Workfront. För de aktuella licenserna krävs en Pro Workfront-plan eller högre för att den här funktionen ska kunna användas. För de nya licenserna innehåller alla planer den här funktionen. Mer information om olika tillgängliga planer finns i <a href="https://business.adobe.com/products/workfront/pricing.html">Workfront-planer</a>.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>Du kan länka dokument till Workfront från Experience Manager Assets Essentials. Mer information finns i <a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref"> Adobe Workfront for Experience Manager Assets Essentials</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">WORKFRONT DAM </td> 
   <td>Detta kräver ett extra inköp. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Andra dokumentleverantörer (via anpassade dokumentintegreringar)</td> 
   <td> <p class="workfront_plans">För de aktuella licenserna krävs en Pro Workfront-plan eller högre för att den här funktionen ska kunna användas. För de nya licenserna innehåller alla planer den här funktionen. Mer information om olika tillgängliga planer finns i <a href="https://business.adobe.com/products/workfront/pricing.html">Workfront-planer</a>.</p> </td>
  </tr> 
 </tbody> 
</table>

Innan du länkar dokument eller mappar måste Workfront-administratören aktivera den här funktionen för varje dokumentleverantör eller för en anpassad dokumentintegrering, enligt beskrivningen i [Konfigurera dokumentintegreringar](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

Du kan granska och godkänna dokument som är länkade till en extern molnleverantör på samma sätt som du gör med dokument som överförs direkt till Workfront.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td>
   <td> <p> Alla</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td>
   <td><p>Nytt: Medarbetare eller högre</p>
    <p>eller</p>
    <p>Aktuell: Begäran eller senare</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dokumentlagring

Dokument som är länkade till Workfront från ett externt program lagras hos den externa molnleverantören, inte inom Workfront.

Följande undantag gäller:

* När de tillhandahålls av dokumenttjänsten kan miniatyrbilder och förhandsvisningsbilder lagras på Workfront-servrar.
* När du använder korrektur i Workfront kopieras dokumentet och läggs till på korrekturservrarna.

## Länka ett dokument från ett externt program till Workfront

Du kan länka befintliga dokument till en extern molnleverantör. Detta inkluderar alla delade dokument.

### Förutsättningar {#prerequisites}

Innan du länkar dokument eller mappar måste Workfront-administratören aktivera den här funktionen för varje dokumentleverantör eller för en anpassad dokumentintegrering, enligt beskrivningen i [Konfigurera dokumentintegreringar](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

### Länka ett externt dokument till Workfront {#link-an-external-document-to-workfront}

Du kan länka dokument till Workfront från ett externt program som Google och Microsoft OneDrive.

>[!IMPORTANT]
>
>Dropbox lagrar dokument baserat på filsökvägen. Det innebär att om en fil som är länkad från Dropbox flyttas, byter namn eller tas bort blir den inte tillgänglig i Workfront.

1. Gå till området **Dokument** i Workfront där du vill ha dokumentet.
1. Klicka på **Lägg till ny** och klicka sedan på den externa dokumentleverantören där du vill länka dokument till Workfront.

   Om du till exempel vill länka dokument från Dropbox klickar du på **Från Dropbox**.

   Externa leverantörer som du redan har auktoriserat visas högst upp i listan.

1. (Villkorligt) Om du uppmanas att logga in på den externa tjänsten anger du dina inloggningsuppgifter för tjänsten i rutan som visas och klickar sedan på **Logga in**.
1. (Villkorligt) Om du uppmanas att auktorisera det externa programmet klickar du på knappen **Auktorisera** .

   Du behöver bara göra detta en gång.

1. I sökrutan i rutan **Länka externa filer och mappar** som visas skriver du namnet på det objekt som du vill söka efter och trycker sedan på **Retur** för att se alla resultat från det externa programmet, oavsett i vilken mapp de lagras.

   eller

   Bläddra till och markera de dokument som du vill länka.

   Även om du kan markera flera dokument är bara de dokument som är markerade i den aktuella vyn länkade. Om du t.ex. markerar ett dokument och sedan går till en mapp, är det dokument som du ursprungligen markerade inte länkat.

1. (Villkorligt) Om du använder Workfront DAM klickar du på ikonen **Miniatyrbild** för att visa filer som miniatyrbilder.

   >[!NOTE]
   >
   >Workfront DAM-kunder kan visa miniatyrer när de länkar dokument från Workfront DAM. Miniatyrbilder kan också visas för Workfront DAM-kunder för andra tjänster som Dropbox och Box. Det går inte att visa miniatyrbilder för andra tjänster än Workfront DAM i Workfront, och miniatyrbilder visas aldrig när du länkar dokument från SharePoint eller Google Drive.

1. Klicka på **Länk**.

   I Workfront visas molnleverantörens ikon bredvid dokumenten.

   >[!NOTE]
   >
   >* Om den hämtnings-URL som används för att länka dokumentet överskrider 2 048 tecken kan filen inte länka.
   >* För dokument som är länkade till Box visas inte länken till dokumentet i Box förrän du uppdaterar sidan.

### Lägga till en ny version av ett länkat dokument {#add-a-new-version-of-a-linked-document}

Du kan lägga till en ny version av ett dokument som är länkat till Workfront från ett externt program.

1. Gå till området **Dokument** där dokumentet är länkat och markera sedan det länkade dokumentet.

   >[!IMPORTANT]
   >
   >Dokumentet måste finnas utanför en länkad mapp för att du ska kunna skapa en ny version.

1. Klicka på **Lägg till ny** > **Version** och klicka sedan på den externa dokumentleverantören.

   Om du till exempel vill länka en ny version av ett dokument från Dropbox klickar du på **Från Dropbox**.

   Externa leverantörer som du redan har auktoriserat visas högst upp i listan.

1. (Villkorligt) Om du uppmanas att logga in på den externa tjänsten anger du dina inloggningsuppgifter för tjänsten i rutan som visas och klickar sedan på **Logga in**.
1. (Villkorligt) Om du uppmanas att auktorisera det externa programmet klickar du på **Auktorisera**.

   Du behöver bara göra detta en gång.

1. I sökrutan i rutan **Länka externa filer och mappar** som visas skriver du namnet på det objekt som du vill söka efter och trycker sedan på **Retur** för att se alla resultat från det externa programmet, oavsett i vilken mapp de lagras.

   eller

   Bläddra till och markera de dokument som du vill länka.

   Du kan markera flera dokument, men bara dokument som är markerade i den aktuella vyn är länkade. Om du t.ex. markerar ett dokument och sedan går till en mapp, är det dokument som du ursprungligen markerade inte länkat.

1. (Villkorligt) Om du använder Workfront DAM klickar du på ikonen **Miniatyrbild** för att visa filer som miniatyrbilder.

   >[!NOTE]
   >
   >Workfront DAM-kunder kan visa miniatyrer när de länkar dokument från Workfront DAM. Miniatyrbilder kan också visas för Workfront DAM-kunder för andra tjänster som Dropbox och Box. Det går inte att visa miniatyrbilder för andra tjänster än Workfront DAM i Workfront, och miniatyrbilder visas aldrig när du länkar dokument från SharePoint eller Google Drive.

1. Klicka på **Länk**.

   I Workfront visas molnleverantörens ikon bredvid dokumenten, vilket anger att de är länkade till den externa molnleverantören.

   >[!NOTE]
   >
   >För dokument som är länkade till Box visas inte länken till dokumentet i Box förrän du uppdaterar sidan.

Mer information om hur du lägger till en ny version av ett dokument som du har överfört till Workfront från filsystemet finns i [Lägg till dokument i Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#add-documents-to-workfront) i [Lägg till dokument i Adobe Workfront från filsystemet](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### Länka Workfront Proof-dokument {#link-workfront-proof-documents}

Du kan länka korrektur till Workfront som ursprungligen fanns i Workfront Proof. När du länkar ett korrektur från Workfront Proof är alla kommentarer och andra metadata som är kopplade till korrekturet tillgängliga i Workfront.

Du kan bara länka de korrektur som du har åtkomst till Visa i Workfront Proof.

1. Gå till området **Dokument** i Workfront där du vill ha dokumentet.
1. Klicka på **Lägg till ny** och sedan på **Från Workfront Proof**.

   >[!NOTE]
   >
   >Alternativen på den här menyn kan variera beroende på vilka tredjepartsleverantörer som är konfigurerade i din miljö.

1. I rutan **Länkkorrektur från Workfront Proof** som visas börjar du skriva namnet på det korrektur som du vill göra tillgängligt i Workfront.

   Listan filtreras när du skriver.

1. Välj upp till 10 korrektur att länka till.

   Ett nedtonat korrekturnamn går inte att länka eftersom korrekturet redan är kopplat till ett dokument i Workfront.

1. Klicka på **Länk**.

   Den senaste versionen av korrekturet är länkad till Workfront. När du öppnar korrekturet är alla versioner tillgängliga i korrekturläsaren.

### Skapa ett Google-dokument i Workfront {#create-a-google-document-from-within-workfront}

Du kan skapa ett nytt Google-dokument i Workfront. Du kan inte skapa nya dokument från Workfront för andra molnleverantörer.

1. Gå till området **Dokument** i Workfront där du vill ha dokumentet.
1. Klicka på **Lägg till ny** > **Google-fil** och välj sedan den typ av Google-dokument som du vill skapa.
1. Om rutan **Lägg till Google Drive-konto** visas klickar du på **Auktorisera Google Drive**.

   Ett Google-dokument läggs till på fliken **Dokument**.

   >[!NOTE]
   >
   > Min enhet och Delad med mig visar två olika resultat. Om du inte kan hitta en fil på Min enhet checkar du in mappen Delad med mig.

## Överföra och länka ett dokument från Workfront till en extern molnleverantör

Du kan överföra och länka ett dokument från Workfront till en extern molnleverantör. Detta flyttar lagringen av dokumentet från Workfront till den externa molnleverantören. När dokumentet ändras i det externa programmet uppdateras det automatiskt i Workfront.

>[!NOTE]
>
>När du skickar en resurs till en extern dokumentleverantör skapas en ny version av resursen.

Användare utan Workfront-åtkomst kan se dokumentet i det externa programmet om de har tillgång till programmet.

1. Markera ett dokument som har överförts till Workfront.
1. Klicka på **Mer** >**Skicka till** och välj sedan den molnleverantör som du vill lagra det länkade dokumentet hos.

   Du kan också använda menyn Mer ![Mer](assets/more-icon.png) på sidan Dokumentinformation för att göra detta.

1. Markera den mapp i providerns program där du vill lagra dokumentet.

   Detta kan vara vilken mapp som helst i providerns program, inklusive en delad mapp.

1. Klicka på **Spara**.

   Den externa leverantörens logotyp visas bredvid dokumentnamnet för att ange att dokumentet nu är länkat till Workfront och lagrat av den externa molnleverantören.

   ![doc_with_google_drive_link_highlight_1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## Länka mappar

När du länkar en mapp mellan Workfront och en extern molnleverantör länkas mappen och allt dess innehåll. Om användare utan Workfront-åtkomst lägger till, tar bort och ändrar filer från det externa dokumentprogrammet synkroniseras deras ändringar med Workfront.

### Mappåtkomsträttigheter {#folder-access-rights}

När du synkroniserar mappinnehåll från ett externt dokumentprogram använder Workfront inloggningsuppgifterna för den användare som ursprungligen länkade mappen. Detta ger följande användarupplevelse:

* Om användare inte har åtkomst till att visa filer och mappar i det externa programmet, men har åtkomst till att visa den länkade mappen via Workfront, kan de bara visa namnen på filerna och mapparna i Workfront, inte deras innehåll.
* När någon öppnar innehåll i en länkad mapp i Workfront (t.ex. en undermapp i en länkad mapp) som en annan användare har länkat till Workfront, synkroniseras innehållet med Workfront med inloggningsuppgifterna för Workfront för den användare som ursprungligen länkade mappen, inte inloggningsuppgifterna för den användare som har åtkomst till innehållet.

>[!IMPORTANT]
>
>* Om den användare som ursprungligen länkade mappen tas bort från Workfront-systemet kan användarna inte längre komma åt innehåll i den länkade mappen via Workfront. I så fall måste mappen länkas om av en aktiv Workfront-användare som har behörighet till mappen i det externa programmet.
>* Om den användare som har länkat en mapp inte längre har åtkomst till det externa programmet kan Workfront inte längre komma åt innehållet i mappen. Detta kan till exempel inträffa om användaren som ursprungligen länkade mappen lämnar företaget. För att säkerställa fortsatt åtkomst måste en användare med åtkomst till mappen länka om mappen.

### Länka en eller flera externa mappar {#link-one-or-more-external-folders}

1. Gå till det område i Workfront där du vill ha mappen och klicka sedan på ikonen **Dokument** ![Dokument](assets/document-icon.png) i den vänstra panelen.

1. Klicka på **Lägg till ny** och klicka sedan på den externa dokumentleverantör som du vill länka en mapp från till Workfront.
1. (Villkorligt) Om du ännu inte har auktoriserat den externa tjänsten anger du dina inloggningsuppgifter för den externa leverantören och klickar sedan på **Logga in**.

   Externa leverantörer som du redan har auktoriserat visas högst upp i listan.

1. I rutan **Länka externa filer och mappar** som visas bläddrar du till och markerar de mappar som du vill länka.

   eller

   Skriv namnet på mappen som du vill söka efter och tryck sedan på **Retur**.

   Du kan markera flera mappar, men bara de mappar som är markerade i den aktuella vyn är länkade. Om du t.ex. markerar en mapp och sedan går till en mapp, länkas inte den mapp som du ursprungligen markerade.

   >[!NOTE]
   >
   >När du länkar mappar från Google Drive kan du bara länka mappar som finns på din personliga enhet (Min enhet) och Team Drive. Du kan inte länka mappar från området Delat med mig.

1. Klicka på **Länk**.

   I Workfront visas molnleverantörens logotyp bredvid mappen, vilket anger att den är länkad till den externa molnleverantören.

1. (Valfritt) Om du vill byta namn på mappen så att mappnamnet i Workfront skiljer sig från mappnamnet i det externa dokumentprogrammet, markerar du mappen i avsnittet **Mappar**, klickar på menyn Mer ![Mer](assets/more-icon.png) som visas bredvid mappnamnet och klickar sedan på **Byt namn**.

   ![Byt namn på mapp](assets/documents-folderlink-rename-nwe-350x154.png)

Det här ändrar inte namnet på mappen i det externa programmet.

### Lägga till undermappar i en länkad mapp  {#add-subfolders-to-a-linked-folder}

Du kan skapa en ny mapp i en befintlig länkad mapp. Du kan också dra en annan mapp till en befintlig länkad mapp.

1. Om du vill skapa en ny mapp i en befintlig länkad mapp går du till den befintliga mappen och skapar sedan den nya mappen enligt beskrivningen i [Skapa dokumentmappar](../../documents/organizing-documents/create-documents-folder.md).

   eller

   Om du vill dra en befintlig mapp till en befintlig länkad mapp går du till området Dokument där du vill ha undermappen och drar den till den länkade mappen.

   ![Dra till den länkade mappen](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   >
   >Följande begränsningar gäller när du drar en befintlig Workfront-mapp till en länkad mapp:
   >
   >* Mappen som du drar kan inte redan vara länkad och kan inte innehålla innehåll som redan är länkat.
   >* Mappen (inklusive dess innehåll) som du drar får inte överstiga 50 MB.

## Lägga till ett dokument i en länkad mapp

När du lägger till ett dokument i en länkad mapp via Workfront, läggs det automatiskt till som ett länkat dokument.

1. Markera den länkade mapp där du vill ha dokumentet, klicka på **Lägg till nytt > Dokument**, bläddra sedan till dokumentet och lägg till det i mappen.

   eller

   Dra dokumentet till en länkad mapp i området **Dokument** där du vill ha dokumentet.

   En ny version av dokumentet skapas automatiskt i det externa programmet och länkas till Workfront.

>[!NOTE]
>
> * Dokumentalternativen är inte tillgängliga när dokumentet håller på att flyttas.
>
> * När ett dokument har flyttats till Experience Manager Assets visas det inte längre i dokumentlistan i Workfront.
>
> * De åtgärder eller redigeringar du gör i ett dokument när det flyttas visas inte i dokumentet i Experience Manager Assets och kommer därför att gå förlorade.

## Ta bort ett länkat dokument eller en länkad mapp

När du tar bort ett länkat dokument eller en länkad mapp från det externa programmet förblir dokumentet eller mappen kvar i Workfront-systemet tills du också tar bort den från Workfront.

1. Markera det länkade dokumentet eller den länkade mappen och klicka sedan på **Ta bort**.
1. Klicka på **Ja, bryt länken** i bekräftelserutan som visas.

   Dokumentet är inte länkat från Workfront webbplats. Den påverkas inte i det externa programmet.

## Om att byta namn på länkade dokument och mappar

När du byter namn på ett länkat dokument eller en länkad mapp visas ändringen bara i det program där du gör den. Om du t.ex. byter namn på ett länkat dokument i Workfront visas det nya namnet bara i Workfront.

Om du vill att namnet ska matcha i Workfront och det externa programmet måste du byta namn på det på båda platserna.

>[!IMPORTANT]
>
>Byt inte namn på ett dokument i Workfront som är länkat till Dropbox. Om du gör det blir filen i Workfront otillgänglig. Byt i stället namn på filen i Dropbox och synkronisera sedan filen igen.
