---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Skriva ut en korrektursammanfattning i Adobe Workfront
description: Du kan skriva ut en korrektursammanfattning, spara den som PDF eller exportera den som en XLS-fil eller PDF-fil som är optimerad för Adobe Reader.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 1b85267e811f5832480316be5322ee819abaf190
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Skriva ut en korrektursammanfattning i Adobe Workfront

Du kan skriva ut en korrektursammanfattning, spara den som PDF eller exportera den som en XLS-fil eller PDF-fil som är optimerad för Adobe Reader.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om korrekturåtkomst för olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Åtkomst till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Alla (du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för bevis </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront- eller Workfront Proof-administratören om du vill ta reda på vilken plan, roll eller behörighetsprofil du har.

+++

## Skriva ut en korrektursammanfattning eller spara den som en PDF-fil

Du kan skriva ut en korrektursammanfattning direkt från dokumentlistan.

>[!NOTE]
>
>Du kan inte skriva ut flera korrektursammanfattningar från dokumentlistan samtidigt.

1. I dokumentlistan som innehåller korrekturet för du muspekaren över raden som innehåller dokumentet och klickar sedan på **Skriv ut sammanfattning**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   eller

   När du visar korrekturet i korrekturläsaren klickar du på ikonen **Skriv ut** ![](assets/print-icon-in-pv.png) i det vänstra verktygsfältet. (Om det vänstra verktygsfältet inte visas klickar du på menyikonen ![](assets/menu-icon-in-pv.png) i det övre vänstra hörnet i korrekturläsaren.)

1. Använd något av följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visa</td> 
      <td> <p>Ange vad du vill skriva ut:</p> 
       <ul> 
        <li><strong>Aktuell version</strong> eller <strong>Alla versioner</strong> av korrekturet</li> 
        <li>Endast <strong>Sidorna med kommentarer</strong> eller <strong>Alla sidor</strong></li> 
        <li>Endast <strong>Sidminiatyrer</strong> (en liten återgivning av varje sida) eller <strong>Fullständiga sidor</strong> (en fullständig återgivning av korrekturet)<br></li> 
        <p>Obs! Om du vill visa PIN-nummer på markeringar i utskriften måste du markera Hel sida, inte Sidminiatyrer. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sortera kommentarer efter</td> 
      <td> <p>(Endast tillgängligt om du har valt Sidminiatyrer ovan) Ange i vilken ordning du vill att korrekturens kommentarer ska skrivas ut:</p> 
       <ul> 
        <li><strong>Äldst</strong>: Från den första kommentaren till den sista</li> 
        <li><strong>Senaste</strong>: Från den senaste kommentaren till den första</li> 
        <li><strong>Sida</strong>: Efter sida, från första sidan till sista sidan eller från sista sidan till första</li> 
        <li><strong>Skapare</strong>: Efter namnen på de användare som lade till dem, från A-Z eller från Z-A</li> 
       </ul> <p>Dessa alternativ påverkar inte utdata som du exporterar som en XLS- eller PDF-fil.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filtrera kommentarer efter</td> 
      <td> <p>Du kan använda valfri kombination av dessa alternativ för att endast inkludera vissa kommentarer i utdata som du skriver ut eller exporterar som en XLS- eller PDF-fil:</p> 
       <ul> 
        <li>Författare som du väljer (standard)</li> 
        <li>Åtgärder som du väljer</li> 
        <li><strong>Olöst</strong>-status</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbetsflöde</td> 
      <td> <p>(Endast tillgängligt om korrekturet har ett automatiserat arbetsflöde) Du kan klicka på <strong>Visa diagram</strong> om du vill inkludera ett diagram i utskriften som visar stegen på korrekturet och besluten som fattas på varje fas. I det diagram som visas representerar färgerna beslut som fattas på en scen:</p> <p><strong>Grön</strong>: Godkänd</p> <p><strong>Blå</strong>: Väntar på ett beslut</p> <p><strong>Röd</strong>: Ändringarna krävs</p> <p><strong>Grå</strong>: Har inte startats än</p> <p><strong>Gul</strong>: Godkänd med ändringar</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Skriv ut**.
1. Om du vill skriva ut sammanfattningen klickar du på menyn **Mål** i den högra panelen i fönstret som visas och sedan på **Visa mer**. Klicka på den skrivare som du vill använda i listan som visas och klicka sedan på **Skriv ut**.

   eller

   Om du vill spara sammanfattningen som en PDF-fil klickar du på menyn **Mål**, klickar på **Spara som PDF** och sedan på **Spara**.

## Exportera en korrektursammanfattning som XLS eller PDF

Du kan exportera en korrektursammanfattning för statiskt innehåll som en XLS-fil eller som en PDF-fil. Korrekturexporter innehåller endast innehållet i korrekturet.

1. I dokumentlistan som innehåller korrekturet för du muspekaren över raden som innehåller dokumentet och klickar sedan på **Skriv ut sammanfattning**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Klicka på ikonen XLS eller PDF i det övre högra hörnet av sidan.

   ![](assets/xls-pdf-icons-350x136.png)

När den exporterade filen är klar får du ett e-postmeddelande där du kan hämta filen.

Om du har exporterat sammanfattningen som en PDF-fil visas kommentarer på korrekturet i läsaren för PDF. Om en kommentar har flera kopplade markeringar visas kommentaren flera gånger i kommentarlistan (en gång för varje markering).
