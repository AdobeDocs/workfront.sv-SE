---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Bädda in en extern webbsida i en instrumentpanel
description: Du kan bädda in en extern webbsida i en instrumentpanel för att ge åtkomst till relaterad information från andra system i Adobe Workfront eller till andra Workfront-sidor.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: a8a3aec50b5538de5867ce3ba7723d92c046b50d
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Bädda in en extern webbsida i en instrumentpanel

Du kan bädda in en extern webbsida i en instrumentpanel för att ge åtkomst till relaterad information från andra system i Adobe Workfront eller till andra Workfront-sidor.

Om din organisation till exempel har en webbaserad dokumentdatabas, wiki eller något annat innehållshanteringssystem som innehåller projektinformation som du regelbundet får åtkomst till via en URL, kan du visa den informationen i Workfront genom att skapa en extern sida på en kontrollpanel.

>[!IMPORTANT]
>
>Av säkerhetsskäl kan du på vissa webbplatser inte bädda in webbsidor som en iframe. Om den webbsida som du vill bädda in i en instrumentpanel inte tillåter detta visas inte sidan i instrumentpanelen. Du kan dock fortfarande komma åt den externa sidan genom att klicka på instrumentpanelens namn.\
>![](assets/qs-empty-external-page-report-350x165.png)\
>Om du vill tillåta inbäddning för en webbplats som du äger kan du tillsammans med webbadministratören justera **X-frame-options** inställning. Mer information finns i [X-frame-options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).


>[!IMPORTANT]
>
>Instrumentpanelssidor stöds inte längre som inbäddade externa sidor i Dashboards. Följande Workfront.com-underdomäner stöds inte längre:
>
>* /dashboards &#x200B;
>* /dashboard/ID-&#x200B;
>* /portfolio/:ID/content-dashboard__:dashboardID &#x200B;
>* /program/ID/content-dashboard__:dashboardID &#x200B;
>* /project/:ID/content-dashboard__:dashboardID &#x200B;
>* /task/:ID/content-dashboard__:dashboardID &#x200B;
>* /template/:ID/content-dashboard__:dashboardID &#x200B;
>* /templateTask/:ID/content-dashboard__:dashboardID &#x200B;
>* /resourceManagement/:ID/content-dashboard__:dashboardID &#x200B;
>* /team/ID/content-dashboard__:dashboardID &#x200B;
>* /iteration/:ID/content-dashboard__:dashboardID &#x200B;
>* /requests/:ID/content-dashboard__:dashboardID &#x200B;
>* /group/:ID/content-dashboard__:dashboardID &#x200B;
>* /billingrecord/:ID/content-dashboard__:dashboardID


## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Hantera behörigheter på kontrollpanelen</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste skapa en kontrollpanel innan du kan bädda in en extern sida i den.

Mer information om hur du skapar kontrollpaneler finns i [Skapa en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Bädda in en extern sida i en kontrollpanel

>[!IMPORTANT]
>
>Du kan ta bort en extern sida från en kontrollpanel om den inte längre behövs. Du kan dock inte ta bort en extern sida efter att den har skapats i Workfront. Du kan bara ta bort en extern sida med API:t. Mer information finns i [Ta bort en extern sida från en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. Leta reda på webbadressen till den sida som ska visas i Workfront och kopiera webbadressen som finns i adressfältet.

   >[!NOTE]
   >
   >Om du delar URL:er till Workfront-objekt bör du komma ihåg att vissa URL:er upphör att gälla över tid. Dokument-URL:er förfaller till exempel efter att de har öppnats. Detta är konfigurerat som en säkerhetsåtgärd, och enligt design betraktas de som icke-statiska URL:er och bör inte delas.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png)och sedan klicka **Kontrollpaneler**.

1. Om du vill redigera en befintlig instrumentpanel väljer du den instrumentpanel som du vill bädda in webbplatssidan i och klickar sedan på **Instrumentpanelsåtgärder** och markera **Redigera** på menyn.\
   eller\
   Om du vill skapa en ny kontrollpanel klickar du på **Ny instrumentpanel**.\
   Mer information om hur du skapar en kontrollpanel finns i [Skapa en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Klicka **Lägg till extern sida**.

   ![](assets/qs-add-external-page-350x239.png)

1. Ange en **Namn** för den externa sidan.
1. Ange en **Beskrivning**.
1. Klistra in den URL du kopierade tidigare i **URL** fält.\
   Du kan ange följande typer av URL-adresser:

   * En https (krypterad) URL till en webbsida.\
      Endast https-sidor (krypterade) läses in med URL-adressen.\
      ![](assets/add-external-page-dialog-qs-350x247.png)

   * En mall-URL som innehåller sessionsinformation för en specifik webbplats.\
      Till exempel: *https://localhost/?session={!$$SESSION}*
Du måste vara inloggad på den angivna webbplatsen för att kunna visa den externa sidan.\
      Mer information om hur du hämtar ett sessions-ID från Workfront finns i [Grunderna i API](../../../wf-api/general/api-basics.md).\
      Din Workfront-administratör kan konfigurera dina systeminställningar på ett sätt som av säkerhetsskäl inte tillåter användning av sessionsinformation på externa sidor. I det här fallet läses den externa sidan inte in på instrumentpanelen.\
      Mer information om systemsäkerhetsinställningar finns i [Konfigurera säkerhetsinställningar för system](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
      ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

1. Klicka **Spara**.\
   Sidan läggs automatiskt till på kontrollpanelen. Om framtida instrumentpaneler skapas kan den externa sidan läggas till. Den externa sidan finns bland Tillgängliga rapporter.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Alina: *** This is linked to: Creating Dashboards, and Editing Dashboards.)
   </MadCap:conditionalText>
   -->

## Uppdatera en extern sida på en kontrollpanel

Så här uppdaterar du informationen för en extern sida som används i en kontrollpanel:

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png)och sedan klicka **Kontrollpaneler**.
1. Välj den instrumentpanel som du vill uppdatera och klicka sedan på **Redigera** ![](assets/edit-icon.png).

   ![Välj ikonen Redigera.](assets/nwe-editdashboard2021-350x188.png)

1. Till höger på skärmen letar du reda på den externa sida som du vill uppdatera och klickar på **Redigera** ikon.\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. I **Redigera extern sida** uppdaterar du fälten som du vill ändra och klickar sedan på **Spara**.
1. (Valfritt) Klicka på **Ta bort** icon ![](assets/delete.png) för att ta bort den externa sidan från kontrollpanelen. Mer information finns i [Ta bort en extern sida från en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. Klicka i det nedre vänstra hörnet på **Spara + Stäng**.

## Visa externa sidor i en rapport

Du kan visa alla externa sidor i Workfront i en extern sidrapport.

1. Gå till **Huvudmeny** icon ![](assets/main-menu-icon.png) > **Rapporter**.
1. Klicka **Ny rapport** > markera **Extern sida**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Valfritt) Uppdatera rapportens flikar Visa, Filter eller Grupperingar.

   Mer information finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Klicka **Spara+stäng**.

   I den nya rapporten kan du visa namnet och URL:en som är kopplade till de externa sidorna i systemet.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
