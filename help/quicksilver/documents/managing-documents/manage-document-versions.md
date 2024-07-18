---
product-area: documents
navigation-topic: manage-documents
title: Hantera dokumentversioner
description: Du kan hantera flera versioner av ett dokument i Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Hantera dokumentversioner

Du kan hantera flera versioner av ett dokument i Workfront.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p> Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser*</td> 
   <td> <p>Begäran eller senare</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst till dokumentet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

* I den här artikeln antas att dokumentet har flera versioner.

  Om du behöver information om hur du överför nya versioner av ett dokument till Workfront läser du [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md).

## Visa en lista över alla versioner av ett dokument

1. Bläddra i sammanfattningen till vyn **Alla versioner**. Här kan du se alla versioner av dokumentet.

## Visa och hantera information om en tidigare dokumentversion

1. Långt upp på sidan Dokumentinformation klickar du på listrutan bredvid namnet och sedan på namnet på den version som du vill visa och hantera.

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Förutom att visa information om versionen kan du göra ändringar i versionen, till exempel namn, metadata och korrekturinställningar (om det är ett dokumentkorrektur).

## Ladda ned en enda dokumentversion

1. Klicka på menyn Mer ![](assets/more-icon.png) till höger om versionen under **Versioner** i Sammanfattning och klicka sedan på **Hämta** i listrutan som visas.

   ![](assets/more-versions-350x143.png)

## Hämta alla versioner av ett dokument

1. Klicka på **Dokumentinformation** och välj sedan **Alla versioner** i den vänstra panelen.

1. Klicka på **Hämta alla** överst i listan.

## Ta bort en dokumentversion

Om du överför en version av ett dokument av misstag, eller om en version inte längre behövs, kan du ta bort versionen och underhålla det ursprungliga dokumentet.

>[!IMPORTANT]
>
>Det går inte att återställa en dokumentversion som du tar bort individuellt.

Tänk på följande när du tar bort en dokumentversion:

* Endast en version i taget kan tas bort. Om en version tas bort visas den här åtgärden i **uppdateringarna** i dokumentet.
* Om du överför en ny version efter att ha tagit bort en version får den nya versionen nästa sekvensnummer. Om det till exempel finns tre versioner av ett dokument och du tar bort version 3, kommer nästa överförda dokument att vara version 4.
* Systemuppdateringar och kommentarer som görs i en version sparas i Workfront när versionen har tagits bort.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Så här tar du bort en dokumentversion:

1. Gå till det projekt, den uppgift eller det problem som innehåller dokumentet och välj sedan **Dokument**.Hitta det dokument du behöver.
1. Klicka på versionen under **Version** i Sammanfattning och klicka sedan på **Ta bort** i listrutan som visas. Alternativet **Ta bort** visas bara om det finns minst två versioner.

   Om dokumentet är länkat till en extern källa tas länken bort och dokumentet är inte längre tillgängligt via Workfront.

   ![](assets/more-versions-350x143.png)
