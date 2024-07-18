---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Överför dokument och korrektur från  [!DNL Adobe Workfront plugin] till  [!DNL Creative Cloud]
description: Överför dokument och korrektur från  [!DNL Adobe Workfront plugin] till  [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
source-git-commit: 0ca335bf0db934d23f607d3f8ce7cfb67e629053
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Överför dokument och korrektur från [!DNL Adobe Workfront plugin] till [!DNL Creative Cloud]

Du kan överföra dina projekt som dokument för snabb granskning och godkännande eller bara lagra dem i [!DNL Adobe Workfront].

>[!NOTE]
>
>Överföring av dokument och korrektur stöds för närvarande inte i Premiere Pro och After Effects.


## Dokumentbegränsningar

I det här avsnittet beskrivs kända dokumentbegränsningar i [!DNL Workfront for Adobe Creative Cloud plugins].

### Nya dokumentversioner accepterar endast en fil för överföring

Eftersom [!DNL Workfront]-dokument inte kan innehålla flera filer måste vissa inställningar inaktiveras för att du ska kunna överföra nya dokumentversioner till Workfront.

>[!NOTE]
>
>Om du måste generera flera filer kan du skapa ett korrektur i stället. Det nya korrekturet kopplas inte till originaldokumentet.



Så här ändrar du växeln tillbaka till en enda fil i [!DNL InDesign]:

1. Öppna dialogrutan **Ange inställningar för exportfil**.

   ![](assets/file-export-settings.png)

1. Hitta den resurstyp som du vill exportera och justera inställningarna enligt nedan:

   <table>
    <tr>
    <td><strong>PDF och PDF-PRINT</strong>
    </td>
    <td>Avmarkera <strong>Skapa separata PDF-filer</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Välj <strong>Intervall</strong> och skriv ett enda sidnummer. 
    <p>
    <strong>Obs!</strong> Om du vill överföra det fullständiga dokumentet måste du skapa ett korrektur. 
    </td>
    </tr>
    <tr>
    <td><strong>EPUB och EPUB-FIXED</strong>
    </td>
    <td>Inga justeringar behövs.
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>Inga justeringar behövs.
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td>Välj <strong>Intervall</strong> och skriv ett enda sidnummer. 
    <p>
    <strong>Obs!</strong> Om du vill överföra det fullständiga dokumentet måste du skapa ett korrektur. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>Välj <strong>Intervall</strong> och skriv ett enda sidnummer. 
    <p>
    <strong>Obs!</strong> Om du vill överföra det fullständiga dokumentet måste du skapa ett korrektur. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>Inga justeringar behövs. 
    </td>
    </tr>
    </table>
