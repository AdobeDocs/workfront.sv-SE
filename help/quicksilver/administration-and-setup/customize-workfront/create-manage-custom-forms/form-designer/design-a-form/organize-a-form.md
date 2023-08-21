---
title: Organisera och förhandsgranska ett formulär med Form Designer
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan ordna ett anpassat formulär med Form Designer.
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 961e0451ce9011a8a9f511d7d5da99368d22d6fb
workflow-type: tm+mt
source-wordcount: '1113'
ht-degree: 0%

---

# Organisera och förhandsgranska ett formulär med formulärdesignern

Du kan ordna ett anpassat formulär med formulärdesignern.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td>
   <p>Aktuell plan: Standard</p>
   <p>eller</p>
   <p>Gammal plan: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> <p>Mer information om hur Workfront administratörer beviljar den här åtkomsten finns i <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Ge användarna administrativ åtkomst till vissa områden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## Lägga till en avsnittsbrytning

Du kan gruppera anpassade fält och widgetar i ett anpassat formulär i avsnitt med rubriker. Detta är användbart för att ge en välordnad upplevelse till användare som fyller i formuläret. Om du dessutom behöver begränsa åtkomsten till vissa anpassade fält och widgetar för vissa användare, kan du placera dem i ett avsnitt och sedan ge åtkomst till avsnittet till endast dessa användare.

Om du till exempel behöver spåra känslig information som bara systemadministratörer ska kunna visa eller redigera, kan du skapa en avsnittsbrytning med enbart administratör och placera de känsliga fälten i det avsnittet.

De åtkomstinställningar som du väljer för ett avsnitt är direkt knutna till de behörigheter som användare har på det Workfront-objekt där det anpassade formuläret bifogas. Du kan dölja eller visa ett avsnitt baserat på om användaren har åtkomst till att visa, bidra till eller hantera objektet. Du kan också ange ett avsnitt som Endast administratör så att bara användare med en systemadministratörsåtkomstnivå kan komma åt det.

Mer information om objektbehörigheter finns i [Översikt över delningsbehörigheter för objekt](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Mer information om anpassade fält och widgetar i anpassade formulär finns i [Designa ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Skapa och konfigurera åtkomst för ett avsnitt i ett anpassat formulär

1. Börja skapa eller redigera ett anpassat formulär och lägga till fält, enligt beskrivningen i [Designa ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicka **Avsnittsbrytning** och dra den till önskad plats på arbetsytan.

1. Konfigurera de alternativ du vill använda för avsnittet i den högra panelen:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför avsnittet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Använd inte specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Skriv text om du vill förklara för användarna vad avsnittet är till för. Detta visas under avsnittets etikett i det anpassade formuläret.</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>Ge åtkomst</p> </td> 
      <td> <p> Markera de behörigheter som användare behöver för ett objekt där det anpassade formuläret är kopplat för att visa det här avsnittet och redigera fältvärdena. 
       <p>Följande behörigheter är tillgängliga under <b>Användare med denna åtkomst till objektet kan visa fältvärden</b>:</p> 
         <ul>
          <li><strong>Visa</strong>: Visa behörigheter för objektet</li>
          <li><p><b>Begränsad redigering</b>: (Endast tillgängligt om objektet är ett projekt, en uppgift, ett problem eller en användare):</p> 
          <p>Tillåter användare att bidra till objektet om det är ett projekt, en uppgift eller ett problem.</p>
          <p>Tillåter användare att redigera profilen eller äger profilbehörigheten till objektet om det är en användare.</p></li> 
          <li><b>Redigera</b>: Hantera behörigheter för objektet </li> 
          <li><b>Endast administratör</b>: Åtkomstnivå för systemadministratör</li> 
         </ul> </li> 
        <p>Följande behörigheter är tillgängliga under <b>Användare med den här åtkomsten till objektet kan redigera fältvärden</b>: </p> 
         <ul> 
          <li> <p><b>Begränsad redigering</b>: (Endast tillgängligt om objektet är ett projekt, en uppgift, ett problem eller en användare):</p> 
           <p>Om objektet är ett projekt, en uppgift eller ett problem, ger den här behörigheten användarna möjlighet att bidra till objektet</p>
          <p>Om objektet är en användare, ger den här behörigheten användare behörighet att redigera profilen eller äga profilbehörigheten till objektet.</p> 
          <li><b>Redigera</b>: Hantera behörigheter för objektet </li> 
          <li><b>Endast administratör</b>: Åtkomstnivå för systemadministratör</li> 
         </ul> </li> 
       </ul> 
       <p>Mer information om objektbehörigheter finns i <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Översikt över delningsbehörigheter för objekt</a>.</p> 
       <p><b>ANMÄRKNING</b>:  
       <ul> 
       <li> <p>Användare som saknar de behörigheter som du anger här kan inte se anpassade fält och widgetar i avsnittet. </p> <p>Detta gäller även om du visar fältets värden i rapporter eller använder dem i beräknade fält i textlägesrapporter.</p> </li> 
       <li> <p>Om du kopplar flera objekttyper till formuläret kan du ändra de visnings- och redigeringsbehörigheter som är tillgängliga i de här stegen. Mer information finns i <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Hur flera objekttyper kan påverka avsnittsbrytningsbehörigheter i ett anpassat formulär</a> i den här artikeln.</p> </li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Dra eller lägg till minst ett anpassat fält eller en widget till det nya avsnittet. Detta krävs innan du sparar avsnittet.

1. Klicka **Klar**.

   >[!TIP]
   >
   >Klicka **Använd** när som helst medan du skapar ett anpassat formulär för att spara ändringarna och behålla formuläret öppet.

### Hur flera objekttyper kan påverka avsnittsbrytningsbehörigheter {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

Behörigheten för begränsad redigering för anpassade formuläravsnittsbrytningar är bara tillgänglig för objekttyperna Projekt, Aktivitet, Utgåva och Användare.

Om du lägger till en annan objekttyp i formuläret (Portfolio, Program, Dokument, Företag, Faktureringspost, Iteration, Expense eller Grupp) i ett anpassat formulär med en avsnittsbrytning som är konfigurerad med behörigheten Begränsad redigering, uppmanas du att växla till behörigheten Redigera, som är kompatibel med både den objekttypen och de befintliga objekttyperna i formuläret.

>[!INFO]
>
>**Exempel:** I ett anpassat formulär som är associerat med projektobjekttypen konfigureras en avsnittsbrytning med behörigheten Begränsad redigering.
>
>Du lägger till objekttypen Portfolio i formuläret, vilket innebär att behörighetsalternativet Begränsad redigering inte längre är tillgängligt för avsnittsbrytningen i formuläret.
>
>Ett meddelande på skärmen uppmanar dig att växla till behörigheten Redigera, som är den lägsta behörighetsnivån som är kompatibel med både objekttypen och objekttypen Portfolio.


## Placera anpassade fält och widgetar i ett anpassat formulär


1. Börja skapa eller redigera ett anpassat formulär, enligt beskrivningen i [Designa ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Om du vill placera anpassade fält och widgetar på samma rad drar du det ena bredvid det andra tills en linje visas mellan dem.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* Du kan använda **Förhandsgranska** i det övre högra hörnet för att få en uppfattning om hur anpassade fält och widgetar visas i formuläret.
>* Anpassade fält och widgetar kanske inte alltid visas på samma sätt i formuläret, beroende på hur mycket skärmutrymme som är tillgängligt när användaren visar det. Det tredje fältet i en rad med fält kan t.ex. radbrytas till nästa rad med fält om det vågräta utrymmet är begränsat.

1. (Valfritt) Om du vill placera ett anpassat fält eller en widget ovanför eller under ett annat fält drar du fältet ovanför eller nedanför tills en vågrät blå linje visas mellan objekten.

1. Klicka på **Använd**

   eller

   Klicka **Spara och stäng**.

## Förhandsgranska ett anpassat formulär

1. Börja skapa eller redigera ett anpassat formulär och lägga till fält, enligt beskrivningen i [Designa ett formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicka **Förhandsgranska** i det övre vänstra hörnet för att se hur formuläret kommer att se ut när det används och klicka sedan på **Avsluta förhandsgranskning** för att återgå till att redigera formuläret.
