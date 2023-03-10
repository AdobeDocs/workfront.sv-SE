---
product-area: projects
navigation-topic: convert-issues
title: Konvertera ett problem till ett projekt i Adobe Workfront
description: Konvertera ett problem till ett projekt i Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1292'
ht-degree: 0%

---

# Konvertera ett problem till ett projekt i Adobe Workfront

Om mer arbete behöver göras för att slutföra ett problem efter att utgåvan har skickats kan du konvertera utgåvan till ett projekt.

Du kan konvertera ett ärende till ett nytt projekt eller konvertera det till ett projekt med hjälp av en mall. I den här artikeln beskrivs båda sätten att konvertera problem till projekt.

Allmän information om hur du konverterar problem finns i [Översikt över konverteringsproblem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till problem, uppgifter och projekt</p> <p>Redigera åtkomst till finansiella data för att uppdatera finansiell information för en prognos som konverterats från utgåvan</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa behörigheter för utgåvan</p> <p>Du får behörigheten Hantera för projektet när problemet har konverterats</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Konvertera ett ärende till ett projekt

Du kan konvertera en utgåva till ett tomt projekt eller konvertera en utgåva till ett projekt med hjälp av en mall.

1. Gå till ett projekt och klicka på **[!UICONTROL Issues]** i den vänstra panelen.
1. Gör något av följande i listan med problem som visas:

   * Om du vill konvertera en utgåva till ett tomt projekt klickar du på problemets namn och klickar på knappen **[!UICONTROL More]** meny ![](assets/more-icon.png) till höger om problemnamnet och klicka sedan på **[!UICONTROL Convert to a blank project]**.


      eller

      Välj ett problem i listan över problem och klicka på **[!UICONTROL More]** meny ![](assets/more-icon.png) överst i listan klickar du på **[!UICONTROL Convert to a blank project]**.

      >[!IMPORTANT]
      >
      >Alternativet Konvertera till ett tomt projekt visas bara när din system- eller gruppadministratör har aktiverat alternativet [!UICONTROL Allow users to create projects without using a template] i [!UICONTROL Setup] område. Mer information finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


      Du måste lägga till uppgifter manuellt i projektet eller bifoga en mall till projektet när du har konverterat utgåvan.

      Fortsätt med steg 3e nedan.

      <!--
     Is this accurate?
     -->

      >[!TIP]
      >   
      >* Om problemet skapades med en frågekö ärver det nya projektet gruppen för begärandekön.
      >* Om problemet skapades genom att det lades till i avsnittet Problem i projektet ärver det nya projektet gruppen om problemet uppstod.


   * Gör något av följande om du vill konvertera ett ärende till ett projekt med en mall:

      * Klicka på namnet på ett problem och klicka sedan på [!UICONTROL **Mer**] meny ![](assets/more-icon.png) till höger om problemets namn

         ![](assets/issue-more-menu-expanded-with-convert-to-project-options-nwe-350x213.png)

         eller

      * Välj problemet i listan med problem, i en rapport eller på en kontrollpanel, klicka på **Mer** meny ![](assets/more-icon.png) överst i listan klickar du på **Konvertera till projekt från mall** och börja skriva namnet på en mall i **Sökmall** och sedan klicka på mallens namn när den visas i listan. Fortsätt med steg 3.

         <!--      
        (is this accurate?)      
        -->
      >[!TIP]
      >
      >Om du har lagt till mallar i favoritlistan kan du föra musen över [!UICONTROL **Favoritmallar**] och klicka på mallen som du vill använda.

      Rutan Nytt projekt från mall visas.

      ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

      >[!TIP]
      >
      >Om problemet är kopplat till en godkännandeprocess eller om det redan är kopplat till ett matchande objekt, visas en varning högst upp i rutan Konvertera till projekt för att meddela dig att godkännandet kommer att tas bort eller att det matchande objektet kommer att skrivas över under konverteringen. Mer information finns i [Översikt över konverteringsproblem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).


1. (Villkorligt) Om du valde att konvertera utgåvan till ett projekt med hjälp av en mall fortsätter du med följande steg:

   1. Granska mallinformation till höger.

      Mallinformationen innehåller följande:

      * Mallvaraktighet
      * Mallägare
      * Antalet uppgifter på den översta nivån som innehåller namnen på de tre viktigaste uppgifterna
      * Antalet uppgifter i mallen
      * Namnen på de anpassade mallformulären
   1. (Valfritt) För muspekaren över namnet på en mall och klicka på ikonen Favoriter ![](assets/favorites-icon-small.png) för att markera den som en favorit för framtida bruk.

      >[!TIP]
      >
      >Du kan ha upp till 40 Workfront-objekt markerade som favoriter. Detta inkluderar mallar och andra objekt.

   1. Klicka [!UICONTROL **Använd mall**] för att välja en mall.

      The [!UICONTROL Convert to Project] öppnas.

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. Om ett fält redan är ifyllt i mallen fylls fältet i automatiskt i [!UICONTROL Convert to project] box. Du kan redigera de förifyllda värdena så att de bättre matchar ditt projekt. Mer information finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* Systemadministratören eller gruppadministratören kan lägga till eller ta bort fält i [!UICONTROL Convert to Project box] genom att uppdatera projektinformationen i [!UICONTROL Layout Template].
      >
      >* Så här uppdaterar du fält i [!UICONTROL Finance] i [!UICONTROL Convert to Project] ruta som du måste ha [!UICONTROL Edit] behörighet till [!UICONTROL Financial Data] på din åtkomstnivå. Om du har [!UICONTROL View] behörighet till [!UICONTROL Financial Data] på din åtkomstnivå överför all ekonomisk information från mallen till det nya projektet och du kan inte redigera den medan du konverterar problemet. Mer information finns i [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) och [Dela en mall](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).


   1. (Valfritt och villkorligt) Klicka på [!UICONTROL **Alternativ**] i den vänstra panelen väljer du bland de tillgängliga alternativen:

      * [!UICONTROL **Behåll det ursprungliga problemet och knyt lösningen till det här projektet**]

         När du avmarkerar det här alternativet tas den ursprungliga utgåvan bort.

         >[!NOTE]
         >
         >Användare som saknar åtkomst eller behörighet att ta bort problem kan inte ta bort problemet eftersom de konverterar det, oavsett status för den här inställningen. Mer information om åtkomst och behörigheter till problem finns i:
         >
         >* [Bevilja åtkomst till utleveranser](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
         > 
         >* [Dela ett ärende](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


      * [!UICONTROL **Tillåt (användarnamn) åtkomst till det här projektet**]

         Om alternativet inte är markerat är problemet [!UICONTROL Primary Contact] har inte åtkomst till den nya uppgiften.

         >[!NOTE]
         >
         >Vilka alternativ som är tillgängliga här beror på hur Workfront-administratören har konfigurerat dem för alla i systemet eller för din grupp. Mer information finns i [Konfigurera inställningar för uppgifter och problem i hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
         >
         >
         >Eller, om de översta grupperna i din organisation konfigurerade dem separat, beror alternativen här på vilken grupp du valde för det nya projektet i steg 6. Mer information finns i [Konfigurera inställningar för aktiviteter och utgåvor för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).
   1. Klicka [!UICONTROL **Anpassad Forms**] och gör något av följande:

      * Granska de anpassade formulär som är kopplade till mallen. De kommer att överföras till det nya projektet.
      * Kontrollera att alla obligatoriska fält har giltig information.
      * Ändra ordning på de anpassade formulären genom att dra dem ![](assets/drag-object-icon.png) där du vill ha dem.
      * Klicka på **x** till höger om alla formulär som du inte vill överföra till projektet.
      * Om det behövs kan du överföra anpassad formulärinformation från ärendet till projektet.

         >[!TIP]
         >
         >* Om ett anpassat formulär med flera objekt som är kopplat till utgåvan är konfigurerat för användning med både utgåvor och projekt behålls all information som sparas i formuläret när du konverterar.
         >
         >* Om du använder en mall för konverteringen och ett anpassat formulär som är kopplat till mallen innehåller ett anpassat fält som också finns i ett anpassat formulär som är kopplat till utgåvan, används fältvärdet från utgåvan för det nya projektet. Om det anpassade fältet är tomt i utgåvan används dock värdet från mallen.

   1. Klicka [!UICONTROL **Konvertera till projekt**].

      >[!TIP]
      >
      >Om du bestämde dig för att ta bort den ursprungliga utgåvan är frågan nu ett projekt.
      >   
      >eller
      >  
      >Om du bestämde dig för att behålla den ursprungliga utgåvan är utgåvan nu kopplad till det nya projektet och den kommer att slutföras när projektet är klart.
      >
      >Vissa problemfält överförs till projektet. De flesta fält som definieras i mallen överförs automatiskt till det nya projektet om du inte ändrade dem i tidigare steg. Mer information finns i [Översikt över konverteringsproblem i Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).




1. (Valfritt) Ange ytterligare projektinformation &#x200B;(projektägare, projektdatum) och uppgifter efter behov.
1. Klicka [!UICONTROL **Konvertera till projekt**].

   Problemet konverteras nu till ett projekt.

1. Klicka [!UICONTROL **Gå till projekt**] inuti [!UICONTROL Success] i det övre högra hörnet på sidan. Projektsidan öppnas.
