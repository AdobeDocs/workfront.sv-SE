---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Generera korrektur i [!DNL Workfront Proof]
description: Med Workfront Proof kan du skapa korrektur av dokument eller webbplatser och dela dessa med andra. Följande steg beskriver de olika konfigurationsalternativ som är tillgängliga - EDIT ME.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2169'
ht-degree: 0%

---

# Generera korrektur i [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Den här artikeln handlar om funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur inuti [!DNL Adobe Workfront], se [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] Med kan du skapa korrektur av dokument eller webbplatser och dela dessa korrektur med andra. Följande steg beskriver de olika konfigurationsalternativ som är tillgängliga:

## Generera ett korrektur för ett dokument

1. Gör något av följande för att börja skapa ett nytt korrektur och visa [!UICONTROL New Proof] sida:

   * Klicka på den gröna **[!UICONTROL New proof]** i det övre vänstra hörnet på en sida.
   * I **[!UICONTROL Dashboard]** området, i **[!UICONTROL Overview]** klickar du på **[!UICONTROL New proof]** länk.

   * Skicka via Dropzone (Enterprise-funktionen).
   * The **[!UICONTROL New Proof]** visas.

1. Om du vill korrekturgranska ett eller flera dokument lägger du till dokument som ska korrektur på något av följande sätt (upprepa den här processen om du vill lägga till flera dokument som ska korrektur):

   * Dra ett dokument från filsystemet till dra-och-släpp-området i **[!UICONTROL Add Files]** område.
   * Klicka i dra-och-släpp-området i dialogrutan **[!UICONTROL Add Files]** bläddra sedan till och markera dokumentet som du vill överföra från filsystemet på din arbetsstation.

      ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Om du vill korrekturgranska en eller flera webbplatser anger du URL-adressen till den webbplats du vill korrekturgranska i dialogrutan **[!UICONTROL Add Files]** område, tryck sedan på **[!UICONTROL Enter]**.

1. (Valfritt) Upprepa den här processen om du vill lägga till flera webbplatser till korrektur.

   Mer information om korrekturwebbplatser finns i [Generera ett korrektur för en URL](#generate-a-proof-for-a-url).

   ![](assets/proof-website-350x65.png)

1. (Valfritt) Ändra filnamnen för överförda filer:

   1. För musen över dokumentnamnet som du vill ändra i dokumentlistan i dialogrutan **[!UICONTROL Add Files]** klickar du på **[!UICONTROL Edit]** ikon.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. I **[!UICONTROL Proof name]** fält, ange ett nytt namn och klicka sedan på **[!UICONTROL Done]**.

   1. (Valfritt) Om du vill ta bort filer som inte ska överföras för du musen över dokumentet som du vill ta bort i dokumentlistan i dialogrutan **[!UICONTROL Add Files]** klickar du på **[!UICONTROL Delete]** ikon.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Valfritt) Aktivera alternativet **[!UICONTROL Combine all compatible files into single proof]**.

      **När det här alternativet är aktiverat:** Alla statiska filer och webbplatser är tillgängliga i ett enda korrektur och du kan överföra upp till 50 filer vid en given tidpunkt.

      >[!NOTE]
      >
      >Interaktiva filer, inklusive videor och interaktiva webbplatser, kan inte kombineras till ett enda korrektur.

      **När det här alternativet är inaktiverat:** Alla dokument och webbplatser genereras som individuella korrektur och du kan överföra upp till 20 filer vid en viss tidpunkt.

      Så här kombinerar du alla överförda filer och webbplatser till ett enda korrektur:

      1. Aktivera alternativet **[!UICONTROL Combine all compatible files into single proof]**.
      1. I **[!UICONTROL Proof name]** anger du ett nytt namn för det kombinerade korrekturet.
      1. I **[!UICONTROL Add Files]** ändrar du ordningen på de inkluderade filerna genom att dra en fil till önskad ordning. Filernas ordning är sidordningen för det kombinerade korrekturet. Mer information om hur du skapar kombinerade korrektur finns i [Skapa ett korrektur för flera sidor](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Valfritt) Om du vill använda ett automatiserat arbetsflöde som innehåller flera steg i **[!UICONTROL Workflow]** väljer du bland följande alternativ:

   * **Grundläggande:** Välj det här alternativet om du vill ange vilka användare som ska ha tillgång till korrekturet omedelbart efter att det har skapats. Du kan dela korrekturet med flera användare.

      Mer information om hur du delar ett korrektur finns i&quot;Lägga till användare i ett korrektur&quot; i [Dela ett korrektur inom [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatiserad:** Välj det här alternativet om du vill hantera granskning och godkännande av innehåll när du har komplexa granskningsprocesser, eller om du skickar innehåll för granskning till samma grupper av personer regelbundet. Med automatiserat arbetsflöde flyttas korrekturet från scen till scen tills det är slutgiltigt godkänt. De berörda användarna meddelas när de behöver göra ett godkännande.

      Mer information om hur du skapar ett automatiskt arbetsflöde finns i [Ställ in ett korrektur med ett automatiserat arbetsflöde i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Välj om du vill skicka e-postmeddelanden och ett anpassat meddelande till de användare som du valde i föregående steg:

   * **Meddela mottagarna om detta bevis:** Välj det här alternativet om du vill skicka ett e-postmeddelande till användarna. När **[!UICONTROL Basic sharing]** är markerat i **[!UICONTROL Workflow]** skickas ett e-postmeddelande när korrekturet skapas. När **[!UICONTROL Automated workflow]** är markerat i **[!UICONTROL Workflow]** skickas ett e-postmeddelande när korrekturet kommer in i det automatiserade arbetsflöde som användaren är kopplad till.

   * **Lägg till anpassat meddelande:** Välj det här alternativet om du vill inkludera ett anpassat meddelande i meddelandet. Du kan ange ämne och meddelandetext. Meddelandetexten kan innehålla formaterad text, t.ex. fet stil, punkter och hyperlänkar.

1. Välj någon av följande korrekturinställningar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kräv inloggning - korrektur kan bara delas med andra användare</td> 
      <td> <p><strong>Kräv inloggning - korrektur kan bara delas med andra användare:</strong> När det här alternativet är markerat är det bara [!DNL Workfront Proof] -användare kan visa korrekturet.</p> <p>Det här alternativet är inaktiverat som standard. alla som har URL:en kan se korrekturet.</p> <p>När det här alternativet är markerat:</p> 
       <ul> 
        <li>Användarna kan inte logga in på korrekturet om de inte har lagts till i korrekturet.</li> 
        <li>Det går inte att aktivera prenumerationer.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Endast ett beslut krävs för det här beviset</td> 
      <td> <p>När det här alternativet har valts slutförs granskningen efter det att en av beslutsfattarna har fattat sitt beslut.</p> <p>Det här alternativet är inaktiverat som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kräv att beslut signeras elektroniskt</td> 
      <td>Användarna måste ange sitt användarnamn och lösenord när de fattar beslut om ett korrektur.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lås korrektur när alla nödvändiga beslut har fattats</td> 
      <td> <p><strong></strong> När den här inställningen är aktiverad låses korrekturläget när alla beslut har fattats. Läget ändras automatiskt från olåst till låst när den slutliga godkännaren fattar sitt beslut.</p> <p>Det här alternativet är inaktiverat som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hämta originalfil</td> 
      <td> <p><strong></strong> När det här alternativet är markerat kan granskarna hämta originalfilen som korrekturet skapades från.</p> <p>När det här alternativet är avmarkerat visas inte längre ikonen Hämta.<br>Det här alternativet är aktiverat som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dela korrektur via offentlig URL eller inbäddningskod</td> 
      <td>När det här alternativet är markerat kan korrekturet delas via en offentlig URL eller inbäddningskod.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prenumerera på korrektur via offentlig URL eller inbäddningskod</td> 
      <td> <p>När det här alternativet är markerat kan personer som inte har lagts till explicit i korrekturet prenumerera på korrekturet. Den person som prenumererar på beviset får rollen och e-postadressen som du anger i följande inställningar:</p> 
       <ul> 
        <li><strong>Abonnentroll</strong>: Standardkorrekturrollen som tilldelas alla granskare som prenumererar på korrekturet.</li> 
        <li><strong>Inställningar för e-postavisering för prenumeranter</strong>: Standardvarningsmeddelandet som tilldelas alla granskare som prenumererar på korrekturet.</li> 
        <li> <p><strong>Åtkomstbevis via e-postlänk krävs för</strong>: Konfigurera om prenumeranten får ett e-postmeddelande med en länk till beviset. Du kan välja <strong>Ingen e-post</strong> (e-postlänk krävs inte för att få åtkomst till korrekturet), <strong>Endast e-postmeddelanden med korrektur</strong> (prenumeranten får en länk till beviset via e-post utan verifiering) eller <strong>E-postmeddelanden om validering och korrektur</strong> (Prenumeranten får en länk till beviset via e-post och måste klicka på länken för att få tillgång till beviset. syftet med detta alternativ är att se till att personen har angett en korrekt e-postadress som han/hon har tillgång till).</p> <p>Obs! Om korrekturet har bifogat ett automatiserat arbetsflöde kommer alla prenumerationer att generera bekräftelsemeddelanden till korrekturägaren, så att de kan bestämma i vilken fas personen ska läggas till.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Create Proof]**.

   Workfront börjar generera ett korrektur av de valda dokumenten eller webbplatserna. Beroende på filstorlek och typ varierar fördröjningstiden för en dokumentöverföring. Ha tålamod när större filer tar längre tid att generera. Du kan navigera bort från sidan och Workfront fortsätter att generera filen. Den maximala filöverföringsstorleken är 4 GB.

   När korrekturet har skapats klickar du på **[!UICONTROL Go to proof]** för att starta korrekturverktyget.

   ![Skärmdump_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   Dokumentet visas i korrekturverktyget.

   Användare som inte har språkkontroll aktiverat på sitt konto kan fortfarande visa dokumentet och kommentera korrekturet.

## Generera ett korrektur för en URL {#generate-a-proof-for-a-url}

Du kan generera ett korrektur för en URL-adress för första gången. Du kan också generera en ny version av ett URL-korrektur där ett korrektur tidigare har genererats.

>[!NOTE]
>
>Du kan bara generera ett interaktivt korrektur för en URL om [!DNL Workfront] -miljön är integrerad med [!DNL Workfront Proof] Premiumkonto. Kontakta systemadministratören om du inte kan använda korrektur enligt beskrivningen i det här avsnittet.

Så här skapar du ett korrektur för en URL:

1. Gör något av följande för att börja skapa ett nytt korrektur och visa [!UICONTROL New Proof] sida:

   * Klicka på den gröna **[!UICONTROL New proof]** i det övre vänstra hörnet på en sida.
   * I **[!UICONTROL Dashboard]** området, i **[!UICONTROL Overview]** klickar du på **[!UICONTROL New proof]** länk.

   * Skicka via Dropzone (Enterprise-funktionen).

1. (Villkorligt) I **[!UICONTROL New proof]** sida som visas för att skapa en ny version av ett befintligt korrektur:

   1. Välj det URL-korrektur där du vill lägga till en ny version.
   1. Klicka på **[!UICONTROL New Version]** överst på sidan.

      ![Skärmdump_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. På sidan Ny korrekturversion som visas anger du webbadressen till den webbplats som du vill korrekturgranska på **[!UICONTROL Add Files]** område, tryck sedan på **[!UICONTROL Enter]**.

1. (Valfritt) Upprepa den här processen om du vill lägga till flera webbplatser till korrektur.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Klicka på webbplatsen i dokumentlistan i dialogrutan **[!UICONTROL Add Files]** område.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Ange en **[!UICONTROL Proof name]** för beviset.

   Som standard är korrekturnamnet samma som URL:en för webbplatsen.

1. Välj **[!UICONTROL Handle site contents]** alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ta skärmbild</td> 
      <td>Skapar ett korrektur av en statisk bild av URL-adressens framsida.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interaktiv</td> 
      <td> <p>Skapar ett korrektur som gör att granskarna kan navigera på webbplatsen, visa bilder i HTML5, element i Flash och så vidare.</p> <p>För att kunna skapa ett interaktivt korrektur måste webbplatsen ha ett säkert protokoll (https). Dessutom kan webbplatser som inte kan bäddas in i en iframe inte genereras som ett interaktivt korrektur (begränsningar för inbäddning av iframe styrs av den webbplats som du försöker bädda in).</p> <p>När det inledande korrekturet har skapats kan den här inställningen inte ändras när efterföljande versioner skapas.</p> <p>Mer information om interaktiv korrektur finns i <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Generera ett korrektur för interaktivt innehåll</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Skärmbildupplösning</td> 
      <td> <p>(Det här alternativet är inte tillgängligt för interaktiva korrektur.) Du kan justera upplösningen som innehållet visas i eller välja flera upplösningar.</p> <p>På så sätt kan användare granska korrekturet för att se hur innehållet kommer att se ut på olika enheter, till exempel olika storlekar för telefoner, surfplattor och bildskärmar.</p> <p>Om du väljer flera upplösningar skapas ett separat korrektur för varje upplösning som du väljer.</p> <p>När användare kommenterar korrekturet visas den aktuella skärmupplösningen automatiskt i kommentaren så att andra användare vet vilken upplösning kommentaren är kopplad till.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Leta efter undersidor</td> 
      <td>(Det här alternativet är inte tillgängligt för interaktiva korrektur.) Välj det här alternativet om du vill navigera på webbplatsens sidor. Du kan expandera webbplatsen upp till två nivåer från huvudsidan. För musen över en sida för att visa sidans URL. Markera bara de sidor som du vill korrekturgranska. Varje sida som du väljer skapas som ett enskilt korrektur som standard; eller, aktivera <strong>Kombinera till ett enda korrektur</strong> om du vill kombinera alla markerade sidor till ett enda korrektur.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Konfigurera eventuella avancerade alternativ för korrektur, som att dela korrektur, lägga till ett automatiserat arbetsflöde eller ställa in åtkomst- och prenumerationsinställningar. Mer information om dessa alternativ finns i följande artiklar:

   * [Dela ett korrektur inom [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Ställ in ett korrektur med ett automatiserat arbetsflöde i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Konfigurera åtkomst- och prenumerationsinställningar för ett bevis](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Klicka på **[!UICONTROL Done]**.

   Om du lägger till en ny version till ett befintligt URL-korrektur behålls alla alternativ som konfigurerats på det ursprungliga korrekturet eller den tidigare versionen i den här versionen. Om du lägger till en ny version till ett befintligt URL-korrektur behålls alla alternativ som konfigurerats på det ursprungliga korrekturet eller den tidigare versionen i den här versionen.

1. Klicka på **[!UICONTROL Create Proof]**.

## Generera ett korrektur för interaktivt innehåll {#generate-a-proof-for-interactive-content}

Du måste ha en Pro Workfront-plan eller senare för att kunna använda den här funktionen. Mer information om olika planer finns i [Workfront-planer](https://www.workfront.com/plans).

Mer information om interaktivt innehåll finns i [Översikt över korrektur av interaktivt material](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Lägga till interaktivt innehåll som en URL](#add-interactive-content-as-a-url)
* [Lägga till interaktivt innehåll som en ZIP-fil](#add-interactive-content-as-a-zip-file)

### Lägga till interaktivt innehåll som en URL {#add-interactive-content-as-a-url}

Mer information om hur du lägger till ett interaktivt URL-korrektur finns i  [Generera ett korrektur för en URL](#generate-a-proof-for-a-url).

### Lägga till interaktivt innehåll som en ZIP-fil {#add-interactive-content-as-a-zip-file}

1. Förbered innehållet genom att skapa en paketerad ZIP-fil.

   Mer information om paketerade ZIP-filer finns i [Förbereda interaktivt innehåll i en ZIP-fil för korrektur](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) i artikeln [Översikt över korrektur av interaktivt material](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Gör något av följande för att börja skapa ett nytt korrektur och visa [!UICONTROL New Proof] sida:

   * Klicka på den gröna **[!UICONTROL New proof]** i det övre vänstra hörnet på en sida.
   * I **[!UICONTROL Dashboard]** området, i **[!UICONTROL Overview]** klickar du på **[!UICONTROL New proof]** länk.

   * Skicka via Dropzone (Enterprise-funktionen).

1. I **[!UICONTROL New proof]** som visas drar och släpper du det interaktiva .zip-paketet i **[!UICONTROL Add files]** område.

1. (Valfritt) Konfigurera eventuella avancerade alternativ för korrektur, som att dela korrekturet, lägga till ett automatiskt arbetsflöde eller ställa in åtkomst- och prenumerationsinställningar. Mer information om dessa alternativ finns i följande artiklar:

   * [Dela ett korrektur inom [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * i artikeln
   * [Konfigurera åtkomst- och prenumerationsinställningar för ett bevis](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Klicka på **[!UICONTROL Create Proof]**.

   Workfront börjar generera ett bevis på .zip-paketet. Beroende på paketstorleken varierar fördröjningstiden för en dokumentöverföring. Det tar längre tid att generera större filer. Du kan navigera bort från sidan och Workfront fortsätter att generera filen. Den maximala filöverföringsstorleken är 4 GB.

   När korrekturet har genererats kan du klicka på **[!UICONTROL Go to proof]** som visas för att öppna korrekturet.
