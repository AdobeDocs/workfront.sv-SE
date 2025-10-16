---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Visa objekt efter status med samma namn när statusvärdena är kopplade till olika grupper'
description: Du kan ha en uppgiftsstatus tilldelad till Grupp A med namnet Ny status med nyckeln NST med tre bokstäver. Du kan ha en annan uppgiftsstatus tilldelad Grupp B med namnet Ny status med nyckeln NES med tre bokstäver. Även om namnen för de två statusarna kan vara identiska är koden med tre bokstäver alltid unik. Mer information om gruppstatus finns i Skapa eller redigera en gruppstatus.
author: Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Filter: visa objekt efter status med samma namn när statusvärdena är kopplade till olika grupper

<!--Audited: 10/2024-->

Du kan ha en uppgiftsstatus tilldelad grupp A med namnet *Ny status* med nyckeln *NST* med tre bokstäver. Du kan ha tilldelats en annan uppgiftsstatus till grupp B som även heter *Ny status* med nyckeln *NES med tre bokstäver.* Även om namnen för de två statusvärdena kan vara identiska är 3-bokstavskoden alltid unik.

Mer information om gruppstatus finns i [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Med filterverktyget kan du inte identifiera mellan de två statusvärdena som har samma namn. Du måste använda textläge i ett anpassat filter för att skilja mellan de två statusvärdena.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Medarbetare eller begäran om att ändra ett filter </p>
   <p>Standard eller Plan för att ändra en rapport</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa objekt efter status med samma namn när statusvärdena är kopplade till olika grupper

1. Gå till listrutan **Filter** för det filter som du vill anpassa för en lista med uppgifter, till exempel.\
   Detta fungerar likadant för projekt och frågor.
1. Klicka på **Nytt filter**.
1. Välj Aktivitet > Status i den första listrutan i det övre vänstra hörnet.
1. Välj **Lika med** för modifieraren och välj sedan en av de statusar som du vill rapportera om.

   I en aktivitetsrapport lägger du till exempel till **Status är lika med ny status** om du bara vill visa aktiviteter som har statusen **Ny status**.

   >[!TIP]
   >
   >Observera att du bara har ett alternativ för statusen Ny status.

1. Klicka på **Textläge**.\
   Följande kod ska visas i det tillgängliga utrymmet:

   <pre>OR:1:status=NST<br>OR:1:status_Mod=in </pre>

   >[!NOTE]
   >
   >Endast en status visas här. Statusraden visar en av 3-bokstavstangenterna för ett av statusvärdena.

1. Lägg till följande två kodrader för att lägga till den status som saknas i filtret:

   <pre>OR:2:status=NES<br>OR:2:status_Mod=in</pre>

1. Klicka på **Använd** och sedan på **Spara som ny**.

   I listan visas båda aktiviteterna med statusen &quot;Ny status&quot; från grupp A och med statusen &quot;Ny status&quot; från grupp B.
