---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Ladda upp dokument och korrektur från [!DNL Adobe Workfront plugin] till [!DNL Creative Cloud]
description: Ladda upp dokument och korrektur från [!DNL Adobe Workfront plugin] till [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
source-git-commit: 67952bf88a782595e13e559bfbc14ce1c622d432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Ladda upp dokument och korrektur från [!DNL Adobe Workfront plugin] till [!DNL Creative Cloud]

Du kan överföra dina projekt som dokument för snabb granskning och godkännande eller bara lagra dem i [!DNL Adobe Workfront].

>[!NOTE]
>
>Överföring av dokument och korrektur stöds för närvarande inte i Premiere Pro och After Effects.


## Dokumentbegränsningar

I det här avsnittet beskrivs kända dokumentbegränsningar i [!DNL Workfront for Adobe Creative Cloud plugins].

### Nya dokumentversioner accepterar endast en fil för överföring

För [!DNL Workfront] -dokument kan inte innehålla flera filer. Vissa inställningar måste vara inaktiverade för att du ska kunna överföra nya dokumentversioner till Workfront.

>[!NOTE]
>
>Om du måste generera flera filer kan du skapa ett korrektur i stället. Det nya korrekturet kopplas inte till originaldokumentet.



Byta tillbaka till en enda fil i [!DNL InDesign]:

1. Öppna **Ange inställningar för exportfil** -dialogrutan.

   ![](assets/file-export-settings.png)

1. Hitta den resurstyp som du vill exportera och justera inställningarna enligt nedan:

   <table>
    <tr>
    <td><strong>PDF och PDF</strong>
    </td>
    <td>Avmarkera <strong>Skapa separata filer i PDF</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Välj <strong>Intervall</strong> och skriv ett enda sidnummer. 
    <p>
    <strong>Anteckning</strong>: Om du vill överföra hela dokumentet måste du skapa ett korrektur. 
    </td>
    </tr>
    <tr>
    <td><strong>ePub OCH EPUB</strong>
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
    <strong>Anteckning</strong>: Om du vill överföra hela dokumentet måste du skapa ett korrektur. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>Välj <strong>Intervall</strong> och skriv ett enda sidnummer. 
    <p>
    <strong>Anteckning</strong>: Om du vill överföra hela dokumentet måste du skapa ett korrektur. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>Inga justeringar behövs. 
    </td>
    </tr>
    </table>
