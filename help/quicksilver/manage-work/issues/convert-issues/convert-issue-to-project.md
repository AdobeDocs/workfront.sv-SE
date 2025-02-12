---
product-area: projects
navigation-topic: convert-issues
title: Konvertera ett problem till ett projekt i Adobe Workfront
description: Konvertera ett problem till ett projekt i Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1924'
ht-degree: 0%

---

# Konvertera ett problem till ett projekt i Adobe Workfront

<!--Audited: 01/2024-->

Om mer arbete behöver göras för att slutföra ett problem efter att utgåvan har skickats kan du konvertera utgåvan till ett projekt.

Du kan konvertera ett ärende till ett nytt projekt eller konvertera det till ett projekt med hjälp av en mall. I den här artikeln beskrivs båda sätten att konvertera problem till projekt.

>[!IMPORTANT]
>
>Allmän information om konvertering av problem finns i artikeln [Översikt över konvertering av problem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

När du skapar ett projekt från ett problem fylls vissa av fälten i från andra objekt. Mer information finns i avsnittet Nya standardinställningar för projekt i artikeln [Skapa ett projekt](../../../manage-work/projects/create-projects/create-project.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard </p> 
    <p>Aktuell: Planera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till problem, uppgifter och projekt</p> <p>Redigera åtkomst till finansiella data för att uppdatera finansiell information för en prognos som konverterats från utgåvan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter för utgåvan</p> <p>Du får behörigheten Hantera för projektet när problemet har konverterats</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konvertera ett ärende till ett projekt

Du kan konvertera en utgåva till ett tomt projekt.

1. Gå till ett projekt och klicka på **[!UICONTROL Issues]** i den vänstra panelen.
1. Gör något av följande i listan med problem som visas:

   * Om du vill konvertera ett problem till ett tomt projekt klickar du på problemets namn, **[!UICONTROL More]**-menyn ![Mer-menyn](assets/more-icon.png) till höger om problemets namn och sedan på **[!UICONTROL Convert to a blank project]**.


     eller

     Välj problemet i listan med problem, klicka på **[!UICONTROL More]**-menyn ![Mer-menyn](assets/more-icon.png) överst i listan och klicka sedan på **[!UICONTROL Convert to a blank project]**.

     >[!IMPORTANT]
     >
     >Alternativet Konvertera till ett tomt projekt visas bara när system- eller gruppadministratören har aktiverat inställningen [!UICONTROL Allow users to create projects without using a template] i området [!UICONTROL Setup]. Mer information finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     Du måste lägga till uppgifter manuellt i projektet eller bifoga en mall till projektet när du har konverterat utgåvan.

     >[!TIP]
     >   
     >* Om problemet skapades med en frågekö ärver det nya projektet gruppen för begärandekön.
     >* Om problemet skapades genom att det lades till i avsnittet Problem i projektet ärver det nya projektet gruppen för problemprojektet.

     >[!TIP]
     >
     >Om problemet är kopplat till en godkännandeprocess eller om det redan är kopplat till ett matchande objekt, visas en varning högst upp i rutan Konvertera till projekt för att meddela dig att godkännandet kommer att tas bort eller att det matchande objektet kommer att skrivas över under konverteringen. Mer information finns i [Översikt över konvertering av problem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Valfritt och villkorligt) Klicka på [!UICONTROL **Alternativ**] i den vänstra panelen och välj sedan bland de tillgängliga alternativen:

   * [!UICONTROL **Behåll det ursprungliga problemet och koppla dess upplösning till det här projektet**]

     När du avmarkerar det här alternativet tas den ursprungliga utgåvan bort.

     >[!NOTE]
     >
     >Användare som saknar åtkomst eller behörighet att ta bort problem kan inte ta bort problemet eftersom de konverterar det, oavsett status för den här inställningen. Mer information om åtkomst och behörigheter till problem finns i:
     >
     >* [Bevilja åtkomst till utgåvor](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Dela ett problem](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Tillåt (användarnamn) åtkomst till det här projektet**]

     Om alternativet inte är markerat har utgåvan [!UICONTROL Primary Contact] ingen åtkomst till den nya aktiviteten.

     >[!NOTE]
     >
     >Vilka alternativ som är tillgängliga här beror på hur Workfront-administratören har konfigurerat dem för alla i systemet eller för din grupp. Mer information finns i [Konfigurera inställningar för aktiviteter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Eller, om de översta grupperna i din organisation konfigurerade dem separat, beror alternativen här på vilken grupp du valde för det nya projektet i steg 6. Mer information finns i [Konfigurera aktivitets- och probleminställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. Klicka på [!UICONTROL **Egen Forms**] och gör något av följande:

   * Granska de anpassade formulären som är kopplade till problemet. De kommer att överföras till det nya projektet om de också är skräddarsydda projektformulär.
   * Lägga till fler anpassade formulär
   * Kontrollera att alla obligatoriska fält har giltig information.
   * Ordna om de anpassade formulären genom att dra dem ![Dra ikonen](assets/drag-object-icon.png) där du vill ha dem.
   * Klicka på ikonen **x** till höger om ett formulär som du inte vill överföra till projektet. Detta tar bort formuläret från projektet.
   * Om det behövs kan du överföra anpassad formulärinformation från ärendet till projektet.

     >[!TIP]
     >
     >* Om ett anpassat formulär med flera objekt som är kopplat till utgåvan är konfigurerat för användning med både utgåvor och projekt, behålls all information som sparas i formuläret när du gör konverteringen om fälten finns både i utgåvan och i projektets anpassade formulär.
     >* Om ett anpassat formulär med flera objekt och ett beräknat fält bifogas till utgåvan och till projektet, måste utgåvan och projektet vara kompatibla med alla fält som refereras i formulärets beräknade anpassade fält. Om det finns inkompatibilitet visas ett meddelande som varnar dig om att göra ändringar. Mer information finns i avsnittet&quot;Beräknade anpassade fält i anpassade formulär med flera objekt&quot; i [Lägg till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

1. Klicka på [!UICONTROL **Konvertera till projekt**].

   >[!TIP]
   >
   >Om du bestämde dig för att ta bort den ursprungliga utgåvan är frågan nu ett projekt.
   >   
   >eller
   >  
   >Om du bestämde dig för att behålla den ursprungliga utgåvan är utgåvan nu kopplad till det nya projektet och den kommer att slutföras när projektet är klart.
   >
   >Information i vissa felfält överförs till projektet om du inte ändrade dem under konverteringen.

1. (Valfritt) Ange ytterligare projektinformation &#x200B;(projektägare, projektdatum) och uppgifter efter behov.
1. Klicka på [!UICONTROL **Konvertera till projekt**].

   Problemet konverteras nu till ett projekt. Projektsidan visas.

## Konvertera ett ärende till ett projekt med en mall

Du kan konvertera ett ärende till ett projekt med hjälp av en mall.

1. Gå till ett projekt och klicka på **[!UICONTROL Issues]** i den vänstra panelen.
1. Klicka på problemets namn i listan med problem som visas, klicka på menyn **[!UICONTROL More]** ![Mer](assets/more-icon.png) till höger om problemets namn, klicka sedan på **Konvertera till projekt från mall** och börja skriva namnet på en mall i rutan **Sökmall**. Klicka sedan på mallens namn när den visas i listan. Fortsätt med steg 3.

   >[!TIP]
   >
   >Om du har lagt till mallar i favoritlistan kan du föra musen över menyn [!UICONTROL **Favoritmallar**] och klicka på mallen som du vill använda.

   Rutan Nytt projekt från mall visas.

   ![Nytt projekt från mall](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!TIP]
   >
   >* Om problemet är kopplat till en godkännandeprocess eller om det redan är kopplat till ett matchande objekt, visas en varning högst upp i rutan Konvertera till projekt för att meddela dig att godkännandet kommer att tas bort eller att det matchande objektet kommer att skrivas över under konverteringen. Mer information finns i [Översikt över konvertering av problem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).
   >   
   >* Om problemet skapades med en frågekö ärver det nya projektet gruppen för begärandekön.
   >* Om problemet skapades genom att det lades till i avsnittet Problem i projektet ärver det nya projektet gruppen för problemprojektet.

1. Granska mallinformation till höger.

   Mallinformationen innehåller följande:

   * Mallvaraktighet
   * Mallägare
   * Antalet uppgifter på den översta nivån som innehåller namnen på de tre viktigaste uppgifterna
   * Antalet uppgifter i mallen
   * Namnen på de anpassade mallformulären

1. (Valfritt) För musen över namnet på en mall och klicka på ikonen **Favoriter** ![Favoriter](assets/favorites-icon-small.png) för att markera den som en favorit för framtida bruk.

   >[!TIP]
   >
   >Du kan ha upp till 40 Workfront-objekt markerade som favoriter. Detta inkluderar mallar och andra objekt.

1. Klicka på [!UICONTROL **Använd mall**] för att välja en mall.

   Rutan [!UICONTROL Convert to Project] öppnas.

   ![Konvertera till projekt](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

1. Om ett fält redan är ifyllt i mallen fylls fältet i automatiskt i rutan [!UICONTROL Convert to project]. Du kan redigera de förifyllda värdena så att de bättre matchar ditt projekt. Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!TIP]
   >
   >* Systemadministratören eller gruppadministratören kan lägga till eller ta bort fält i [!UICONTROL Convert to Project box] genom att uppdatera projektinformationsinformationen i [!UICONTROL Layout Template].
   >
   >* Om du vill uppdatera fält i avsnittet [!UICONTROL Finance] i rutan [!UICONTROL Convert to Project] måste du ha [!UICONTROL Edit] åtkomst till [!UICONTROL Financial Data] på åtkomstnivån. Om du har [!UICONTROL View] åtkomst till [!UICONTROL Financial Data] på åtkomstnivån överförs all ekonomisk information från mallen till det nya projektet och du kan inte redigera den medan du konverterar problemet. Mer information finns i [Bevilja åtkomst till ekonomiska data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) och [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Valfritt och villkorligt) Klicka på [!UICONTROL **Alternativ**] i den vänstra panelen och välj sedan bland de tillgängliga alternativen:

   * [!UICONTROL **Behåll det ursprungliga problemet och koppla dess upplösning till det här projektet**]

     När du avmarkerar det här alternativet tas den ursprungliga utgåvan bort.

     >[!NOTE]
     >
     >Användare som saknar åtkomst eller behörighet att ta bort problem kan inte ta bort problemet eftersom de konverterar det, oavsett status för den här inställningen. Mer information om åtkomst och behörigheter till problem finns i:
     >
     >* [Bevilja åtkomst till utgåvor](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Dela ett problem](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Tillåt (användarnamn) åtkomst till det här projektet**]

     Om alternativet inte är markerat har utgåvan [!UICONTROL Primary Contact] ingen åtkomst till den nya aktiviteten.

     >[!NOTE]
     >
     >Vilka alternativ som är tillgängliga här beror på hur Workfront-administratören har konfigurerat dem för alla i systemet eller för din grupp. Mer information finns i [Konfigurera inställningar för aktiviteter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Eller, om de översta grupperna i din organisation konfigurerade dem separat, beror alternativen här på vilken grupp du valde för det nya projektet i steg 6. Mer information finns i [Konfigurera aktivitets- och probleminställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Klicka på [!UICONTROL **Egen Forms**] och gör något av följande:

      * Granska de anpassade formulär som är kopplade till mallen. De kommer att gå över till det nya projektet.
      * Granska de anpassade formulären som är kopplade till problemet. De överförs till projektet om de också är projektformulär.
      * Kontrollera att alla obligatoriska fält har giltig information.
      * Ordna om de anpassade formulären genom att dra dem ![Dra ikonen](assets/drag-object-icon.png) där du vill ha dem.
      * Klicka på ikonen **x** till höger om ett formulär som du inte vill överföra till projektet.
      * Om det behövs kan du överföra anpassad formulärinformation från ärendet till projektet.

        >[!TIP]
        >
        >* Om ett anpassat formulär med flera objekt som är kopplat till utgåvan är konfigurerat för användning med både utgåvor och projekt, behålls all information som sparas i formuläret när du gör konverteringen om fälten finns både i utgåvan och i projektets anpassade formulär.
        >* Om ett anpassat formulär med flera objekt och ett beräknat fält bifogas till utgåvan och till projektet, måste utgåvan och projektet vara kompatibla med alla fält som refereras i formulärets beräknade anpassade fält. Om det finns inkompatibilitet visas ett meddelande som varnar dig om att göra ändringar. Mer information finns i [Lägga till beräknade fält i ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
        >* Om ett anpassat formulär som är kopplat till mallen innehåller ett anpassat fält som också finns i ett anpassat formulär som är kopplat till utgåvan, används fältvärdet från utgåvan för det nya projektet. Om det anpassade fältet är tomt i utgåvan används dock värdet från mallen.

1. (Valfritt) Ange ytterligare projektinformation &#x200B;(projektägare, projektdatum) och uppgifter efter behov.

   1. Klicka på [!UICONTROL **Konvertera till projekt**].

      >[!TIP]
      >
      >Om du bestämde dig för att ta bort den ursprungliga utgåvan är frågan nu ett projekt.
      >   
      >eller
      >  
      >Om du bestämde dig för att behålla den ursprungliga utgåvan är utgåvan nu kopplad till det nya projektet och den kommer att slutföras när projektet är klart.
      >
      >Vissa problemfält överförs till projektet. De flesta fält som definieras i mallen överförs automatiskt till det nya projektet om du inte ändrade dem i tidigare steg. Mer information finns i [Översikt över konvertering av problem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

   Problemet konverteras nu till ett projekt. Projektsidan visas.