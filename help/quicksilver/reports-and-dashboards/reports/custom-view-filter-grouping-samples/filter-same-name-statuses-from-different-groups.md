---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: visa objekt efter status med samma namn när statusvärdena är kopplade till olika grupper'
description: Du kan ha en uppgiftsstatus tilldelad till Grupp A med namnet Ny status med nyckeln NST med tre bokstäver. Du kan ha en annan uppgiftsstatus tilldelad Grupp B med namnet Ny status med nyckeln NES med tre bokstäver. Även om namnen för de två statusarna kan vara identiska är koden med tre bokstäver alltid unik. Mer information om gruppstatus finns i Skapa eller redigera en gruppstatus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Filter: visa objekt efter status med samma namn när statusvärdena är kopplade till olika grupper

Du kan ha en uppgiftsstatus tilldelad grupp A med namnet *Ny status* med nyckeln *NST* med tre bokstäver. Du kan ha tilldelats en annan uppgiftsstatus till grupp B som även heter *Ny status* med nyckeln *NES med tre bokstäver.* Även om namnen för de två statusvärdena kan vara identiska är 3-bokstavskoden alltid unik.\
Mer information om gruppstatus finns i [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Med filterverktyget kan du inte identifiera mellan de två statusvärdena som har samma namn. Du måste använda textläge för att skilja mellan de två statusvärdena.

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
   <td> <p>Begäran om att ändra ett filter </p>
   <p>Planera att ändra en rapport</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar för att ändra en rapport</p> <p>Redigera åtkomst till filter, vyer och grupperingar för att ändra ett filter</p> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i en rapport</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Visa objekt efter status med samma namn när statusvärdena är kopplade till olika grupper

1. Gå till det filter som du vill anpassa, t.ex. för en lista med uppgifter.\
   Detta fungerar likadant för projekt och frågor.
1. Klicka på **Lägg till en filterregel** för fältet **Status** för objektet i listan.\
   Lägg till exempel till **Status lika med ny status** i en aktivitetsrapport om du bara vill visa uppgifter som har statusen **Ny status**.

   >[!TIP]
   >
   >Observera att du bara har ett alternativ för statusen Ny status.

1. Klicka på **Växla till textläge**.\
   Följande kod ska visas:
   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Endast en status visas här. Statusraden visar en av 3-bokstavstangenterna för ett av statusvärdena.

1. Lägg till följande två kodrader för att lägga till den status som saknas i filtret:
   <pre>OR:1:status=NES<br>OR:1:status_Mod=in</pre>

1. Klicka på **Klar** och sedan på **Spara filter**.

   I listan visas båda aktiviteterna med statusen &quot;Ny status&quot; från grupp A och med statusen &quot;Ny status&quot; från grupp B.
