---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Generera korrektur i  [!DNL Workfront Proof]
description: Med Workfront Proof kan du skapa korrektur av dokument eller webbplatser och dela dessa med andra.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 1443551b605dac6e53531c5d445b89517384fe11
workflow-type: tm+mt
source-wordcount: '1818'
ht-degree: 0%

---

# Generera korrektur i [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>Den här artikeln hänvisar till funktionalitet i den fristående produkten [!DNL Workfront Proof]. Mer information om korrektur i [!DNL Adobe Workfront] finns i [Korrektur](../../../review-and-approve-work/proofing/proofing.md).

Med [!DNL Workfront Proof] kan du skapa korrektur från dokument eller webbplatser och dela dessa korrektur med andra. Följande steg beskriver de olika konfigurationsalternativ som är tillgängliga:

## Generera ett korrektur från ett dokument

1. Öppna sidan **[!UICONTROL New Proof]** genom att göra något av följande:

   * Klicka på knappen **[!UICONTROL New proof]** i det övre vänstra hörnet på en sida.
   * Skicka via Dropzone (Enterprise-funktionen).

1. Om du vill korrekturgranska ett eller flera dokument lägger du till dokument som ska korrektur på något av följande sätt (upprepa den här processen om du vill lägga till flera dokument):

   * Dra ett dokument från filsystemet till dra och släpp-området i **[!UICONTROL Add Files]**-området.
   * Klicka på länken **bläddra** i området **[!UICONTROL Add Files]** för att hitta och välja det dokument som du vill överföra från filsystemet på arbetsstationen.

     ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Om du vill korrekturgranska en webbplats anger du webbplatsens URL i området **[!UICONTROL Add Files]** och trycker sedan på **[!UICONTROL Enter]**. Upprepa det här steget om du vill lägga till flera webbplatser i korrektur.

   Mer information om korrekturwebbplatser finns i [Skapa ett korrektur för en URL](#generate-a-proof-for-a-url).

   ![Korrekturwebbplats](assets/proof-website-350x65.png)

1. (Valfritt) Ändra filnamnen för överförda filer:

   1. Håll markören över dokumentnamnet som du vill ändra i dokumentlistan och klicka sedan på ikonen **[!UICONTROL Edit]**.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. Ange ett nytt namn i fältet **[!UICONTROL Proof name]** och klicka sedan på **[!UICONTROL Done]**.

   1. (Valfritt) Om du vill ta bort filer som inte ska överföras håller du pekaren över dokumentet som du vill ta bort i dokumentlistan och klickar sedan på ikonen **[!UICONTROL Delete]**.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Valfritt) Aktivera alternativet **[!UICONTROL Combine all compatible files into single proof]**.

      **När det här alternativet är aktiverat:** Alla statiska filer och webbplatser är tillgängliga i ett enda korrektur och du kan överföra upp till 50 filer vid en given tidpunkt.

      >[!NOTE]
      >
      >Interaktiva filer, inklusive videor och interaktiva webbplatser, kan inte kombineras till ett enda korrektur.

      **När det här alternativet är inaktiverat:** Alla dokument och webbplatser genereras som individuella korrektur och du kan överföra upp till 20 filer vid en given tidpunkt.

      Så här kombinerar du alla överförda filer och webbplatser till ett enda korrektur:

      1. Aktivera alternativet **[!UICONTROL Combine all compatible files into single proof]**.
      1. I fältet **[!UICONTROL Proof name]** anger du ett nytt namn för det kombinerade korrekturet.
      1. I området **[!UICONTROL Add Files]** ändrar du ordningen på de inkluderade filerna genom att dra en fil till önskad ordning. Filernas ordning är sidordningen för det kombinerade korrekturet. Mer information om hur du skapar kombinerade korrektur finns i [Skapa ett flersidigt korrektur](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Valfritt) Om du vill använda ett automatiskt arbetsflöde som innehåller flera steg väljer du bland följande alternativ i avsnittet **[!UICONTROL Workflow]**:

   * **Grundläggande:** Välj det här alternativet om du vill ange vilka användare som ska ha tillgång till korrekturet omedelbart efter att det har skapats. Du kan dela korrekturet med flera användare.

     Mer information om att dela ett korrektur finns i [Dela ett korrektur inom [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatiserad:** Välj det här alternativet om du vill hantera granskning och godkännande av innehåll när du har komplexa granskningsprocesser, eller om du skickar innehåll för granskning till samma grupper av personer regelbundet. Med ett automatiserat arbetsflöde går korrekturet från scen till scen tills det är slutgiltigt godkänt. De berörda användarna meddelas när som helst om att de måste göra ett godkännande.

     Mer information om hur du skapar ett automatiserat arbetsflöde finns i [Konfigurera ett korrektur med ett automatiserat arbetsflöde i [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Välj om du vill skicka e-postmeddelanden och ett anpassat meddelande till de användare som du valde i föregående steg:

   * **Meddela mottagarna om det här korrekturet:** Välj det här alternativet om du vill skicka ett e-postmeddelande till användarna. När **[!UICONTROL Basic sharing]** har valts i avsnittet **[!UICONTROL Workflow]** skickas ett e-postmeddelande när korrekturet skapas. När **[!UICONTROL Automated workflow]** har valts i avsnittet **[!UICONTROL Workflow]** skickas ett e-postmeddelande när korrekturet kommer in i det automatiserade arbetsflöde som användaren är kopplad till.

   * **Lägg till anpassat meddelande:** Välj det här alternativet om du vill inkludera ett anpassat meddelande i meddelandet. Du kan ange ämne och meddelandetext. Meddelandetexten kan innehålla formaterad text, t.ex. fet stil, punkter och hyperlänkar.

1. Välj någon av följande korrekturinställningar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Kräv inloggning. Detta korrektur kan inte delas med andra användare</td> 
      <td> <p>När det här alternativet är markerat:</p> 
       <ul> 
        <li>Användarna kan inte logga in på korrekturet för att visa det om de inte har lagts till i det.</li> 
        <li>Det går inte att aktivera prenumerationer.</li> 
       </ul> 
       <p>Det här alternativet är inaktiverat som standard.</p> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kräv att beslut signeras elektroniskt</td> 
      <td><p>När det här alternativet är markerat måste användarna ange sitt användarnamn och lösenord när de fattar ett beslut om ett korrektur.</p>
      <p>Det här alternativet är inaktiverat som standard.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lås korrektur när alla nödvändiga beslut har fattats</td> 
      <td> <p>När den här inställningen är aktiverad låses korrekturläget när alla beslut har fattats. Läget ändras automatiskt från olåst till låst när den slutliga godkännaren fattar sitt beslut.</p> 
      <p>Det här alternativet är inaktiverat som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt hämtning av originalfilen</td> 
      <td> <p><strong></strong> När det här alternativet är markerat kan granskarna hämta originalfilen som korrekturet skapades från.</p> <p>När det här alternativet är avmarkerat visas inte längre ikonen Hämta.</p>
      <p>Det här alternativet är aktiverat som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt delning av korrektur via offentlig URL eller inbäddningskod</td> 
      <td><p>När det här alternativet är markerat kan korrekturet delas via en offentlig URL eller inbäddningskod.</p>
       <p>Det här alternativet är aktiverat som standard.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt att prenumerera på korrektur via en offentlig URL eller inbäddningskod</td> 
      <td> <p>När det här alternativet är markerat kan personer som inte har lagts till i korrekturet prenumerera på korrekturet. Den person som prenumererar på beviset får rollen och e-postadressen som du anger i följande inställningar:</p> 
       <ul> 
        <li><strong>Prenumerantroll</strong>: Standardkorrekturrollen som tilldelas alla granskare som prenumererar på korrekturet.</li> 
        <li><strong>E-postaviseringsinställningar för prenumeranter</strong>: Standardaviseringen för e-post som tilldelas alla granskare som prenumererar på korrekturet.</li> 
        <li> <p><strong>Åtkomst via e-postlänk krävs för</strong>: Konfigurera om prenumeranten får ett e-postmeddelande med en länk till korrekturet. Du kan välja <strong>Inget e-postmeddelande</strong> (e-postlänk krävs inte för att få åtkomst till korrekturet), <strong>E-postmeddelande för korrektur endast</strong> (prenumeranten får en länk till korrekturet via e-post utan någon verifiering) eller <strong>E-postmeddelanden för validering och korrekturrundor</strong> (prenumeranten får en länk till beviset via e-post och måste klicka på länken för att få åtkomst. Syftet med det här alternativet är att se till att personen har angett en korrekt e-postadress som han/hon har tillgång till).</p> <p>Obs! Om korrekturet har ett automatiserat arbetsflöde, kommer alla prenumerationer att generera bekräftelsemeddelanden till korrekturägaren så att de kan bestämma i vilken fas personen ska läggas till.</p> </li> 
       </ul> 
        <p>Det här alternativet är inaktiverat som standard.</p>
       </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Create Proof]**. Workfront genererar ett korrektur av de valda dokumenten eller webbplatserna.

   Hur lång tid det tar att överföra ett dokument varierar beroende på filstorlek och typ. Det tar längre tid att generera större filer. Du kan navigera bort från sidan när Workfront fortsätter att generera filen. Den maximala filöverföringsstorleken är 4 GB.

## Generera ett statiskt korrektur med en URL {#generate-a-proof-for-a-url}

Du kan generera ett statiskt korrektur med en webb-URL.

>[!NOTE]
>
>Du kan bara generera ett interaktivt korrektur för en URL om din [!DNL Workfront]-miljö är integrerad med ett [!DNL Workfront Proof] Premium-konto. Kontakta Workfront-administratören om du inte kan använda korrektur som beskrivs i det här avsnittet.

1. Öppna sidan **[!UICONTROL New Proof]** genom att göra något av följande:

   * Klicka på knappen **[!UICONTROL New proof]** i det övre vänstra hörnet på en sida.
   * Skicka via Dropzone (Enterprise-funktionen).

1. På sidan **Nytt korrektur** anger du webbadressen till webbplatsen som du vill skapa ett korrektur från i området **[!UICONTROL Add Files]** och trycker sedan på **[!UICONTROL Enter]** eller **[!UICONTROL Return]** på tangentbordet.

1. (Valfritt) Upprepa den här processen om du vill lägga till flera webbplatser till korrekturet.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Klicka på ikonen **Redigera** till höger om URL:en i området **[!UICONTROL Add Files]** för att öppna korrekturinformation för webbplatsen.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Ange **[!UICONTROL Proof name]**. Som standard är korrekturnamnet samma som URL:en för webbplatsen.

1. Välj något av följande **[!UICONTROL Handle site contents]**-alternativ:

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
      <td> <p>Skapar ett korrektur som gör att granskarna kan navigera på webbplatsen, visa HTML5-bilder, Flash-element osv.</p> <p>Om du vill skapa ett interaktivt korrektur måste webbplatsen ha ett säkert protokoll (https). Dessutom kan webbplatser som inte kan bäddas in i en iframe inte genereras som ett interaktivt korrektur (begränsningar för iframe-inbäddning styrs av den webbplats som du försöker bädda in).</p> <p>När det inledande korrekturet har skapats kan den här inställningen inte ändras när efterföljande versioner skapas.</p> <p>Mer information om interaktiv korrektur finns i <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Skapa ett korrektur för interaktivt innehåll</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Skärmbildupplösning</td> 
      <td> <p>(Det här alternativet är inte tillgängligt för interaktiva korrektur.) Du kan justera upplösningen som innehållet visas i eller välja flera upplösningar.</p> <p>På så sätt kan användare granska korrekturet för att se hur innehållet kommer att se ut på olika enheter, till exempel olika storlekar för telefoner, surfplattor och bildskärmar.</p> <p>Om du väljer flera upplösningar skapas ett separat korrektur för varje upplösning som du väljer.</p> <p>När användare kommenterar korrekturet visas den aktuella skärmupplösningen automatiskt i kommentaren så att andra användare vet vilken upplösning kommentaren är kopplad till.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Leta efter undersidor</td> 
      <td>(Det här alternativet är inte tillgängligt för interaktiva korrektur.) Välj det här alternativet om du vill navigera på webbplatsens sidor. Du kan expandera webbplatsen upp till två nivåer från huvudsidan. Hovra över en sida för att visa sidans URL-adress och markera endast de sidor som du vill korrekturgranska. Varje sida som du väljer skapas som ett enskilt korrektur som standard. Du kan också aktivera alternativet <strong>Kombinera alla kompatibla filer till ett enda korrektur</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Konfigurera eventuella avancerade alternativ för korrektur, som att dela korrektur, lägga till ett automatiserat arbetsflöde eller ställa in åtkomst- och prenumerationsinställningar. Mer information om de här alternativen finns i följande artiklar:

   * [Dela ett korrektur inom [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Konfigurera ett korrektur med ett automatiserat arbetsflöde i  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Konfigurera åtkomst- och prenumerationsinställningar för ett bevis](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Klicka på **[!UICONTROL Done]**.

1. Klicka på **[!UICONTROL Create Proof]**.

## Generera ett korrektur för interaktivt innehåll {#generate-a-proof-for-interactive-content}

<!--A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).-->

Mer information om interaktivt innehåll finns i [Översikt över interaktiva innehållskorrektur](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Lägga till interaktivt innehåll som en URL](#add-interactive-content-as-a-url)
* [Lägga till interaktivt innehåll som en ZIP-fil](#add-interactive-content-as-a-zip-file)

### Lägga till interaktivt innehåll som en URL {#add-interactive-content-as-a-url}

Mer information om hur du lägger till ett interaktivt URL-korrektur finns i [Skapa ett korrektur för en URL](#generate-a-proof-for-a-url).

### Lägga till interaktivt innehåll som en ZIP-fil {#add-interactive-content-as-a-zip-file}

1. Förbered innehållet genom att skapa en paketerad ZIP-fil.

   Mer information om specifikationer för paketerade ZIP-filer finns i [Översikt över korrektur av interaktivt innehåll](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Öppna sidan **[!UICONTROL New Proof]** genom att göra något av följande:

   * Klicka på knappen **[!UICONTROL New proof]** i det övre vänstra hörnet på en sida.
   * Skicka via Dropzone (Enterprise-funktionen).

1. På sidan **[!UICONTROL New proof]** drar och släpper du det interaktiva ZIP-paketet i området **[!UICONTROL Add files]**.

1. (Valfritt) Konfigurera eventuella avancerade alternativ för korrektur, som att dela korrekturet, lägga till ett automatiskt arbetsflöde eller ställa in åtkomst- och prenumerationsinställningar. Mer information om de här alternativen finns i följande artiklar:

   * [Dela ett korrektur inom [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Konfigurera åtkomst- och prenumerationsinställningar för ett bevis](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Klicka på **[!UICONTROL Create Proof]**. Workfront genererar ett korrektur av zip-filen.

   Hur lång tid det tar att överföra ett dokument varierar beroende på storleken på ZIP-filen. Du kan navigera bort från sidan när Workfront fortsätter att generera filen. Den maximala filöverföringsstorleken är 4 GB.
