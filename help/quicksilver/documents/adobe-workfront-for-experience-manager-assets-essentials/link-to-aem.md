---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Länka innehåll och mappar med Content Advisor från Experience Manager Assets
description: Du kan använda Content Advisor för att länka innehåll eller mappar från Experience Manager Assets till alla Adobe Workfront-objekt som stöder dokument. Content Advisor ger intelligent, sammanhangsberoende identifiering direkt i Workfront, vilket hjälper dig att snabbt hitta relevant, godkänt innehåll.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: ab868314aef0924906ca69e82a10ece130484ba7
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 0%

---

# Länka innehåll och mappar med Experience Manager Assets Content Advisor

Content Advisor ger intelligent, sammanhangsberoende identifiering direkt i Workfront, vilket hjälper dig att snabbt hitta relevant, godkänt innehåll baserat på sammanhang. Med funktioner som smarta förslag, dynamiska medieåtergivningar och detaljerade metadata kan ni effektivt utvärdera och återanvända innehåll utan att lämna Workfront, vilket snabbar upp framtagningen av innehåll samtidigt som varumärkets enhetlighet bibehålls.

Du kan använda Content Advisor för att länka innehåll och mappar från Experience Manager Assets till Workfront. När länken är länkad kan du visa och hantera innehållet i Workfront, och alla ändringar som görs i innehållet i Experience Manager Assets återspeglas i Workfront.

>[!IMPORTANT]
>
>Om din organisation inte godkänner GenAI Rider-avtalet kan du fortfarande använda Content Advisor för att välja resurser och mappar i Experience Manager Assets, men du har inte tillgång till AI-baserade funktioner som AI-sökning, smarta förslag eller analys av kampanjinformation.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser</td> 
   <td> 
   <p>Medarbetare eller högre</p> 
   <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ytterligare produkter</td> 
   <td>Du måste ha Experience Manager as a Cloud Service eller Assets Essentials, och du måste läggas till i produkten som användare i Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager-behörigheter</td> 
    <td>Du måste ha skrivåtkomst till mappen.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till dokument</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar:

* Din Workfront-administratör måste konfigurera en Experience Manager-integrering. Mer information finns i [Konfigurera integreringen med Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

* Om du vill använda smarta förslag eller Campaign Brief-funktionen måste du signera ett GenAI-tillägg. Mer information finns i [Använd Content Advisor för att få åtkomst till AEM-innehåll i Adobe-program](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).



## Länka innehåll från Experience Manager Assets med Content Advisor

Nu kan du använda Content Advisor för att länka innehåll från Experience Manager Assets direkt i Workfront. Content Advisor är inte tillgängligt för Assets Essentials.

Så här länkar du innehåll:

1. Gå till området **Dokument** i Workfront där du vill lägga till dokumentet.
1. Välj **Lägg till ny** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Experience Manager Assets.

1. Med Content Advisor kan du


   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Sök efter resurser med hjälp av AI-sökning.</strong> Använd en AI-baserad sökning som förstår innebörd och återgivning i frågor och stöder flera språk, typografi och synonymer.</td>
         <td>Mer information finns i <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">AI-sökning efter smartare resursidentifiering</a>.</td>
      </tr>
      <tr>
         <td><strong>Visa smarta förslag baserat på sammanhang och avsikt.</strong> Identifiera resurser som är anpassade till ditt innehåll med hjälp av kontextmedvetna rekommendationer från Adobe-värdprogrammet.</td>
         <td>Mer information finns i <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Smarta förslag baserade på sammanhang och avsikt</a>.</td>
      </tr>
      <tr>
         <td><strong>Ladda upp en kampanjsammanfattning för att identifiera relevanta resurser.</strong> Överför ett kort kampanjdokument för PDF, DOCX eller TXT så att Content Advisor kan analysera det och rekommendera relevanta resurser.</td>
         <td>Mer information finns i <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Kampanjinformation för att identifiera relevanta resurser</a>.</td>
      </tr>
      <tr>
         <td><strong>Visa och välj återgivningar av dynamiska mediefiler.</strong> Bläddra bland kanaloptimerade återgivningar som bildförinställningar, smarta beskärningar och formattyper och använd dynamiska mediemodifieringar för att förhandsgranska justeringar i realtid.</td>
         <td>Mer information finns i <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Återgivningar av dynamiska mediefiler som kan användas</a>.</td>
      </tr>
      <tr>
         <td><strong>Använd dynamiska mediemodifierare på återgivningar.</strong> Lägg till modifierare för att omvandla resursrenderingar i realtid och förhandsgranska resultatet innan du väljer en rendering för värdprogrammet.</td>
         <td>Mer information finns i <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Återgivningar av dynamiska mediefiler som kan användas</a>.</td>
      </tr>
      <tr>
         <td><strong>Identifiera och bläddra bland innehållsfragment.</strong> Sök bland innehållsfragment, visa förhandsvisningar av miniatyrbilder i realtid, kontrollera status (utkast, ändrad eller publicerad) och granska detaljerade egenskaper, referenser och variationer.</td>
         <td>Mer information finns i <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Identifiering av innehållsfragment</a>.</td>
      </tr>
      <tr>
         <td><strong>Få åtkomst till metadata för resurser.</strong> Granska resursegenskaper som titel, beskrivning, format, storlek och andra metadataflikar (produkt, kampanj, taggar) som är kompatibla med Assets-vyn.</td>
         <td>Mer information finns i <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Åtkomst till resursmetadata i enlighet med Assets-vyn</a>.</td>
      </tr>
      <tr>
         <td><strong>Filtrera resurser med fördefinierade filter.</strong> Förfina resursens resultat med filter som filtyp, filformat, resursstatus, filstorlek, bildbredd, bildhöjd, ändringsdatum och Skapad den.</td>
         <td>Mer information finns i <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Åtkomstfilter som är konsekventa med Assets-vyn</a>.</td>
      </tr>
      <tr>
         <td><strong>Spara och återanvänd sökningar.</strong> Skapa sparade sökningar genom att ange en sökterm och filteralternativ och sedan återanvända dem i Experience Manager Assets och andra Adobe-program.</td>
         <td>Mer information finns i <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Åtkomst till och återanvändning av senaste och sparade sökningar</a>.</td>
      </tr>
      <tr>
         <td><strong>Sök efter resurser i och mellan samlingar.</strong> Sök efter resurser eller samlingar i alla samlingar, eller begränsa sökningen till en viss samling.</td>
         <td>Mer information finns i <a href="https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Söka efter resurser i och mellan samlingar</a>.</td>
      </tr>
   </tbody>
   </table>


### Länka en ny version från Experience Manager Assets med Content Advisor

Du kan hämta nytt innehåll från Experience Manager Assets eller Assets Essentials och lägga till det i en befintlig resurs som en ny version. Om dokumentet redan är länkat och en ny version har lagts till i Experience Manager Assets eller Resurser Essentials, visas den nya versionen automatiskt i Workfront.

Länka en ny version:

1. Gå till området **Dokument** i Workfront där du vill lägga till dokumentet.
1. Markera den resurs som du vill ersätta med en ny version. Du kan inte skapa en ny version av en resurs i en länkad mapp.
1. Välj **Lägg till ny** > **Version** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Experience Manager Assets.

1. Markera innehållet som du vill länka:

   * Välj fliken Assets för att bläddra bland resurser, mappar och samlingar i Experience Manager Assets eller Resurser Essentials.

     ![Innehållsrådgivare](assets/content-advisor-full.png)

   * Innehållsfragment stöder inte versioner. Om du väljer ett innehållsfragment ersätter den nya versionen det befintliga innehållsfragmentet i stället för att skapa en ny version.

1. Klicka på **Markera**.

## Länka en mapp från Experience Manager Assets med Content Advisor

Behörigheter att visa enskilda resurser i en mapp kräver Experience Manager Assets-behörigheter.

Så här länkar du en mapp:

1. Gå till området **Dokument** i Workfront där du vill ha mappen.
1. Välj **Lägg till ny** och välj sedan den Experience Manager-integrering som administratören har konfigurerat.

   >[!NOTE]
   >
   >Workfront-administratören kan välja vilket namn som helst för integreringen, så det kanske inte uttryckligen anger Experience Manager Assets.

1. Klicka på **Assets** > **Filer och mappar**.

1. Klicka på ikonen **Filter** och välj sedan **Mappar** i avsnittet **Resurstyp**.

1. Markera mappen som du vill länka.

1. Klicka på **Markera**.

## Överväganden

* Funktionen Content Advisor är inte tillgänglig för objekt som använder Adobe Enterprise Storage. Om din organisation använder Adobe Enterprise Storage kan du fortfarande länka resurser och mappar från Experience Manager Assets eller Assets Essentials, men du har inte tillgång till Content Advisor-funktioner som AI Search, smarta förslag eller Dynamic Media-renderingar. Mer information finns i [Använda Adobe Experience Manager med Frame.io-integrering](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* Funktionen Content Advisor är inte tillgänglig för Assets Essentials. Mer information om hur du länkar resurser och mappar från Resurser Essentials finns i [Länka resurser och mappar från Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem-essentials.md).

* Metadatafält mappas först när du skickar en resurs från Workfront till Experience Manager Assets. Om Workfront-administratören har aktiverat synkronisering av objektmetadata, förblir fälten aktuella om de ändras i något av programmen.
