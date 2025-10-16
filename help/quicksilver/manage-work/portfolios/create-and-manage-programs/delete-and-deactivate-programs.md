---
product-area: programs
navigation-topic: Create and manage programs
title: Ta bort och inaktivera program
description: Ett program representerar en samling projekt som delar en gemensam strategi, mål eller mål som överskrider projektgränserna. Programmen utgör en underindelning av portföljer och får inte finnas utanför en portfölj. Program har vanligtvis samma resurser som andra program i samma portfölj. Du kan ta bort eller inaktivera ett program när det inte är relevant.
author: Alina
feature: Work Management, Strategic Planning
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Ta bort och inaktivera program

Ett program representerar en samling projekt som delar en gemensam strategi, mål eller mål som överskrider projektgränserna. Programmen utgör en underindelning av portföljer och får inte finnas utanför en portfölj. Program har vanligtvis samma resurser som andra program i samma portfölj.

När ett program blir irrelevant kan du göra något av följande för att hindra användare från att associera projekt med programmet:

* Inaktivera den: Avslutar projekt som är kopplade till programmet och till respektive portfölj. Användarna ser inte längre programmet som ett alternativ när de försöker associera nya projekt med programmet.
* Ta bort den: Befintliga projekt förlorar sin koppling till programmet och de flyttas direkt under portföljen. Användarna ser inte längre programmet som ett alternativ när de försöker associera sina framtida projekt med programmet.

Vi rekommenderar att du inaktiverar en portfölj, i stället för att ta bort den, för att bevara den historiska informationen för dina projekt. Ibland kan det dock vara nödvändigt att ta bort ett program.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkraven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td>

<td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>[!UICONTROL Standard]</p><p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] tillgång till portföljer och program </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] behörighet till portföljen</p> <p>När du har skapat ett program har du som standard [!UICONTROL Manage] behörighet till det.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ta bort ett program

{{step1-to-programs}}

1. Klicka på namnet på ett program för att öppna det.
1. Klicka på menyn **Mer** till höger om programnamnet och klicka sedan på **Ta bort program**.
1. Bekräfta genom att klicka på **Ja, ta bort**.

   Programmet tas bort och följande sker:

   * Befintliga projekt förlorar sin koppling till programmet och de går direkt under portföljen.
   * Användarna ser inte längre programmet som ett alternativ när de försöker associera sina framtida projekt med programmet.

## Inaktivera ett program

{{step1-to-programs}}

1. Klicka på namnet på ett program för att öppna det.
1. Klicka på menyn **Mer** till höger om programnamnet och klicka sedan på **Inaktivera program**.

   Programmet inaktiveras omedelbart och följande inträffar:

   * Avslutade projekt är fortfarande kopplade till programmet och till dess respektive portfölj.
   * Användarna ser inte längre programmet som ett alternativ när de försöker associera nya projekt med programmet.