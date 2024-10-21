---
title: Anpassa panelen Sammanfattning med en layoutmall
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Du kan använda en layoutmall för att konfigurera vad användare ser när de klickar på en uppgift eller ett problem i sammanfattningen. Varje konfiguration som du gör enligt stegen nedan påverkar panelen Sammanfattning. Dessa anpassningar gäller inte för panelen Dokumentsammanfattning.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 43cf88c533b80324266f0660648c6a1ab13ca8fc
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 0%

---

# Anpassa panelen Sammanfattning med hjälp av en layoutmall


Du kan använda en layoutmall för att konfigurera vad användare ser när de klickar på en uppgift eller ett problem i sammanfattningen. Varje konfiguration som du gör enligt stegen nedan påverkar panelen Sammanfattning. Dessa anpassningar gäller inte för panelen Dokumentsammanfattning.

Du kan konfigurera

* Vilka fält som visas för en uppgift eller ett problem i området Detaljer, och i vilken ordning
* Vare sig uppdateringar, loggad tid, bifogade dokument och tidsstämplar visas för en vald uppgift eller utgåva

Du kan också anpassa fälten som användarna ser i området Hem när användarna klickar på ett projektgodkännande, dokumentgodkännande eller godkännande av dokumentversion som de har tilldelats.

Mer information om panelen Sammanfattning finns i [Översikt över sammanfattning](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Mer information om hur du skapar layoutmallar finns i [Skapa och hantera layoutmallar](../use-layout-templates/create-and-manage-layout-templates.md).

Mer information om layoutmallar för grupper finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

När du har konfigurerat en layoutmall måste du tilldela den till användare för att de ändringar du har gjort ska kunna visas för andra. Mer information om hur du tilldelar en layoutmall till användare finns i [Tilldela användare till en layoutmall](../use-layout-templates/assign-users-to-layout-template.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td><p>Nytt: Standard</p>
  <p> Aktuell: Planera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>För att kunna utföra dessa steg på systemnivå måste du ha åtkomstnivån Systemadministratör.
Om du vill utföra dem för en grupp måste du vara chef för den gruppen.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anpassa panelen Sammanfattning med hjälp av en layoutmall

1. Börja arbeta med en layoutmall enligt beskrivningen i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klicka på nedpilen ![](assets/dropdown-arrow.png) under **Anpassa det som visas för användarna** och klicka sedan på **Sammanfattningspanelen**.

1. Klicka i listan till vänster på objekttypen (**Åtgärder**, **Problem**, **Projekt**, **Dokument** eller **Dokumentversioner**) som du vill anpassa på panelen Sammanfattning.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Uppgifter</td> 
      <td><p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Problem</td> 
      <td><p>I en lista över problem påverkar den här inställningen panelen Sammanfattning som visas på sidans högra sida när en användare väljer ett problem och sedan klickar på ikonen Öppna sammanfattning <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projekt</td> 
      <td><p>När en användare klickar på ett projektgodkännande som tilldelats dem i Hem, påverkar konfigurationen för den här inställningen området till höger om godkännandet.</p>
      <p>VIKTIGT: Det här är en inaktuell funktion. Alla ändringar du gör i det här området är relaterade till en funktion som Workfront har tagit bort. Det här alternativet tas bort från Workfront med en senare underhållsuppdatering.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokument</td> 
      <td><p>När en användare klickar på ett dokumentgodkännande som tilldelats dem i Hem, påverkar konfigurationen för den här inställningen området till höger om godkännandet.</p>
      <p>VIKTIGT: Det här är en inaktuell funktion. Alla ändringar du gör i det här området är relaterade till en funktion som Workfront har tagit bort. Det här alternativet tas bort från Workfront med en senare underhållsuppdatering.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumentversioner</td> 
      <td><p>När en användare klickar på ett godkännande som tilldelats dem för en viss version av ett dokument i Hem, påverkar konfigurationen för den här inställningen området till höger om godkännandet.</p>
      <p>VIKTIGT: Det här är en inaktuell funktion. Alla ändringar du gör i det här området är relaterade till en funktion som Workfront har tagit bort. Det här alternativet tas bort från Workfront med en senare underhållsuppdatering.</p>
      </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Om en uppgift inte har tilldelats kan användaren som är tilldelad layoutmallen inte se fältanpassningarna i Sammanfattning.

1. (Villkorligt) Om du klickade på Åtgärder eller Problem i föregående steg väljer du den kategori av uppgift eller problem som du vill anpassa.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Villkorligt) Om listrutan **Ange primär åtgärd** visas (om du väljer **Åtgärder** eller **Problem** i listan till vänster) klickar du på den primära åtgärd (**Klar** eller **Status**) som du vill ska vara tillgänglig för användare på sammanfattningspanelen när de visar en uppgift eller ett problem.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Lägg till ![](assets/add-item-plus-in-circle-blue.png) eller dölj ![](assets/close-or-hide---x.png) fält för den valda objekttypen.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Upprepa steg 3-6 för att anpassa panelen Sammanfattning för andra objekttyper.
1. Klicka på **Globala inställningar**, nära det nedre vänstra hörnet, och aktivera eller inaktivera sedan något av följande alternativ för Adobe Workfront-objekt i sammanfattningen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visa uppdateringar för arbete</td> 
      <td>Visar alla uppdateringar som gjorts för en vald uppgift eller ett valt problem på panelen Sammanfattning. Detta omfattar både systemuppdateringar och uppdateringar som görs av en användare. Användare kan fortfarande filtrera bort systemuppdateringar enligt beskrivningen i <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Aktivera eller inaktivera systemuppdateringar</a> i <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Uppdateringsarbete</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Logga tid för arbete</td> 
      <td>Visar alternativet Logga tid mot arbete när en uppgift eller ett problem har valts, vilket gör att användare kan logga tid på arbetsobjekt direkt från Hem- och sammanfattningsområdena.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa dokument som är kopplade till arbetet</td> 
      <td>Visar ett dokumentområde på panelen Sammanfattning när en uppgift eller ett problem har valts, med en lista över eventuella dokument som har kopplats till uppgiften eller problemet. Användarna kan klicka på dokumenten för att visa dem i ett förhandsgranskningsfönster.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dölj tidsstämpel</td> 
      <td>Döljer tidsstämplar för följande datumfält på panelen Sammanfattning:
       <ul>
        <li>Planerat slutförandedatum</li>
        <li>Bekräftelsedatum</li>
        <li>Skickat den</li>
       </ul></td> 
     </tr> 
    </tbody> 
   </table>

1. Fortsätt att anpassa layoutmallen.

   eller

   Klicka på **Spara** om du är klar med anpassningen.

Mer information om layoutmallar finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
