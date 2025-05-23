---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Upprätta en anslutning till Workfront Data Connect
description: Med Workfront Data Connect kan ni använda företagets Workfront-data med verktyg för affärsintelligens eller lagra dem på ett externt datalager.
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Upprätta en anslutning till Workfront Data Connect

Med Workfront Data Connect kan ni använda företagets Workfront-data med verktyg för affärsintelligens eller lagra dem på ett externt datalager.

Om du vill ansluta Data Connect-datasjön till en extern produkt måste du först skapa en anslutning enligt beskrivningen i [Skapa ett läsarkonto eller en anslutning för Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). Sedan måste du lägga till alla nödvändiga IP-adresser till tillåtelselista enligt beskrivningen i [Lägg till IP-adresser till tillåtelselista](#add-ips-to-the-allowlist) nedan.

De flesta produkter kräver följande information om din datasjön för att upprätta en anslutning:

| Fältnamn | Värde |
|---------------|-------------|
| Server | URL:en för anslutningen, utan delen `https://` (finns på sidan **Data Connect** i Workfront*) |
| Port | `443` |
| Databas | `WORKFRONT` |
| Lagerställe | `READER_WH` |
| Schema | `WF` |
| Roll | `READER_ROLE` |
| Användarnamn | Användarnamnet som valdes när anslutningen skapades (finns på sidan **Data Connect** i Workfront*) |
| Lösenord | Lösenordet som väljs vid första inloggning från Snowflake* |

*Information om var du hittar sidan **Data Connect** som innehåller dina anslutningar finns i [Skapa ett läsarkonto eller en anslutning för Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>När en post har lagts till i IP-tillåtelselista tillåts inte längre alla andra IP-adresser. Se till att du har angett alla IP-adresser som krävs - både för att skapa och läsa upplevelser i visualiseringsverktyget - innan du försöker använda verktyget. Annars kan du råka ut för ett fel med ogiltiga autentiseringsuppgifter.
>
>Om du inte har några IP-adresser i tillåtelselista men fortfarande har problem med att ansluta till ett BI-verktyg, kontrollerar du proxyserverkonfigurationen för BI-verktyget.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Ingår i följande planer:</p>
    <ul>
        <li><p>Ultimate</p></li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect är inte tillgängligt för tidigare Workfront-planer.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till IP-adresser i tillåtelselista

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Konfigurera**.

1. Klicka på **System** > **Dataanslutning** i den vänstra panelen.

1. Klicka på fliken **Tillåtna IP-adresser** och klicka sedan på knappen **Lägg till en IP-adress till Tillåtelselista** .

1. Ange ett namn för IP-adressen i **IP-adressbeskrivningen** och ange IP-adressen (eller CIDR-blocket) för verktyget som du vill använda i **IP-adressen**. Klicka sedan på **Lägg till IP i Tillåtelselista**.

   ![Lägg till IP-adress](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Ta bort en IP-adress från tillåtelselista

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](/help/_includes/assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront, eller (om den är tillgänglig) klicka på **[!UICONTROL Main Menu]** -ikonen ![Huvudmeny](/help/_includes/assets/main-menu-icon-left-nav.png) i det övre vänstra hörnet och klicka sedan på **Konfigurera**.

1. Klicka på **System** > **Dataanslutning** i den vänstra panelen.

1. Klicka på fliken **Tillåtna IP-adresser** och klicka sedan på papperskorgsikonen ![Ta bort ikon](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) till höger om den IP-adress du vill ta bort.

1. Markera rutan för att bekräfta i fönstret som visas och klicka sedan på **Ta bort**.

## Dela data med verktyg för affärsinformation

Ett antal vanliga verktyg för affärsintelligens listas nedan. Besök deras dokumentationssajter för att lära dig mer om hur du ansluter till din datasjön.

* Tableau
* Power BI
* Domo
* SAP HANA

## Lagra data i ett externt datalager

Ett antal vanliga datalager listas nedan. Gå till deras dokumentationssajter och läs mer om hur du ansluter till din datalinje.

* Databricks
* AWS Redshift
