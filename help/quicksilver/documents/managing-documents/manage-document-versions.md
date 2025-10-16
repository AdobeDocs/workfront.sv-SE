---
product-area: documents
navigation-topic: manage-documents
title: Hantera dokumentversioner
description: Du kan hantera flera versioner av ett dokument i Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: 4a0448583cbcfd1f1df10d6474fdf4e77e7bff3e
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Hantera dokumentversioner

<!-- Audited: 5/2025 -->

Du kan hantera flera versioner av ett dokument i Workfront.

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
   <p>Begäran eller senare </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Visa åtkomst till dokument</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst till dokumentet</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

* I den här artikeln antas att dokumentet har flera versioner.

  Om du behöver information om hur du överför nya versioner av ett dokument till Workfront läser du [Överföra en ny version av ett dokument](../../documents/managing-documents/upload-new-document-version.md).

## Visa en lista över alla versioner av ett dokument

{{step1-to-documents}}

1. Markera ett dokument i listan på sidan **Dokument**.

1. Klicka på ikonen **Öppna sammanfattning** ![Öppna sammanfattning](assets/qs-summary-in-new-toolbar-small.png) i det övre högra hörnet på sidan. Sidpanelen **Dokumentsammanfattning** öppnas.

1. Bläddra ned till avsnittet **Versioner** om du vill visa alla dokumentversioner.

## Visa och hantera information om en tidigare dokumentversion

{{step1-to-documents}}

1. Håll markören över dokumentet och klicka sedan på **Dokumentinformation**.

1. Klicka på listrutan bredvid namnet längst upp på sidan **Dokumentinformation** och klicka sedan på namnet på den version som du vill visa och hantera.

   ![Listrutan Version på sidan Dokumentinformation](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Förutom att visa information om versionen kan du göra ändringar i versionen, till exempel namn, metadata och korrekturinställningar (om det är ett dokumentkorrektur).

## Ladda ned en enda dokumentversion

{{step1-to-documents}}

1. Markera ett dokument i listan på sidan **Dokument**.

1. Klicka på ikonen **Öppna sammanfattning** ![Öppna sammanfattning](assets/qs-summary-in-new-toolbar-small.png) i det övre högra hörnet på sidan. Sidpanelen **Dokumentsammanfattning** öppnas.

1. Klicka på menyn **Mer** **Mer** till höger om versionen i avsnittet ![Versioner](assets/more-icon.png) och klicka sedan på **Hämta** i listrutan som visas.

   ![Hämta ett enstaka dokument](assets/more-versions-350x143.png)

## Hämta alla versioner av ett dokument

{{step1-to-documents}}

1. Markera ett dokument i listan på sidan **Dokument**.

1. Klicka på ikonen **Öppna sammanfattning** ![Öppna sammanfattning](assets/qs-summary-in-new-toolbar-small.png) i det övre högra hörnet på sidan. Sidpanelen **Dokumentsammanfattning** öppnas.

1. Bläddra ned till avsnittet **Versioner** och klicka sedan på **Hämta alla**.

## Ta bort en dokumentversion

Om du överför en version av ett dokument av misstag, eller om en version inte längre behövs, kan du ta bort versionen och underhålla det ursprungliga dokumentet.

>[!IMPORTANT]
>
>Det går inte att återställa en dokumentversion som du tar bort individuellt.

Tänk på följande när du tar bort en dokumentversion:

* Endast en version i taget kan tas bort. Om en version tas bort visas den här åtgärden i avsnittet Uppdateringar i dokumentet.
* Om du överför en ny version efter att ha tagit bort en version får den nya versionen nästa sekvensnummer. Om det till exempel finns tre versioner av ett dokument och du tar bort version 3, kommer nästa överförda dokument att vara version 4.
* Systemuppdateringar och kommentarer som görs i en version sparas i Workfront när versionen har tagits bort.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Så här tar du bort en dokumentversion:

{{step1-to-documents}}

1. Välj dokumentet från listan på sidan **Dokument**.

1. Klicka på ikonen **Öppna sammanfattning** ![Öppna sammanfattning](assets/qs-summary-in-new-toolbar-small.png) i det övre högra hörnet på sidan. Sidpanelen **Dokumentsammanfattning** öppnas.

1. Bläddra ned till avsnittet **Versioner** om du vill visa alla dokumentversioner.
1. Klicka på menyn **Mer** **Mer** till höger om versionen i avsnittet ![Versioner](assets/more-icon.png) och klicka sedan på **Ta bort** i listrutan som visas.

   >[!NOTE]
   >
   >* Alternativet **Ta bort** visas bara om det finns minst två versioner.
   >* Om dokumentet är länkat till en extern källa tas länken bort och dokumentet är inte längre tillgängligt via Workfront.

   ![Ta bort dokumentversionen](assets/more-versions-350x143.png)
