---
title: Ordna och förhandsgranska ett formulär
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan ordna ett anpassat formulär med Form Designer.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 796c7e0a15a7a26c5cd3f0115d72946f0f28bcf2
workflow-type: tm+mt
source-wordcount: '1353'
ht-degree: 0%

---

# Ordna och förhandsgranska ett formulär

{{preview-fast-release-general}}

Du kan ordna ett anpassat formulär med formulärdesignern och förhandsgranska det för att kontrollera att det är korrekt konfigurerat.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> </td> 
  </tr>  
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägga till en avsnittsbrytning

Du kan gruppera anpassade fält och widgetar i ett anpassat formulär i avsnitt med rubriker. Detta är användbart för att ge en välordnad upplevelse till användare som fyller i formuläret. Om du dessutom behöver begränsa åtkomsten till vissa anpassade fält och widgetar för vissa användare, kan du placera dem i ett avsnitt och sedan ge åtkomst till avsnittet till endast dessa användare.

Om du till exempel behöver spåra känslig information som bara systemadministratörer ska kunna visa eller redigera, kan du skapa en avsnittsbrytning med enbart administratör och placera de känsliga fälten i det avsnittet.

De åtkomstinställningar som du väljer för ett avsnitt är direkt knutna till de behörigheter som användare har på det Workfront-objekt där det anpassade formuläret bifogas. Du kan dölja eller visa ett avsnitt baserat på om användaren har åtkomst till att visa, bidra till eller hantera objektet. Du kan också ange ett avsnitt som Endast administratör så att bara användare med en systemadministratörsåtkomstnivå kan komma åt det.

Mer information om behörigheter för objekt finns i [Översikt över delningsbehörigheter för objekt](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Mer information om anpassade fält och widgetar i anpassade formulär finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Skapa och konfigurera åtkomst för ett avsnitt i ett anpassat formulär

1. Börja skapa eller redigera ett anpassat formulär och lägga till fält, vilket beskrivs i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicka på **Avsnittsbrytning** och dra den till önskad plats på arbetsytan.

1. Konfigurera de alternativ du vill använda för avsnittet i den högra panelen:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etikett</td> 
      <td> <p>(Obligatoriskt) Skriv en beskrivande etikett som ska visas ovanför avsnittet. Du kan när som helst ändra etiketten.</p> <p><b>VIKTIGT</b>: Undvik att använda specialtecken i den här etiketten. De visas inte korrekt i rapporter.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Skriv text om du vill förklara för användarna vad avsnittet är till för. Detta visas under avsnittets etikett i det anpassade formuläret.</td> 
     </tr> 
      <td><span class="preview">Komprimerad som standard</span></td>
      <td><span class="preview">Som standard expanderas alla avsnitt i ett anpassat formulär när själva formuläret expanderas. Välj det här alternativet om du vill att avsnittet ska komprimeras som standard när en användare öppnar formuläret.</span></td>
     <tr>
     </tr>
     <tr> 
      <td role="rowheader"> <p>Ge åtkomst</p> </td> 
      <td> <p> Markera de behörigheter som användare behöver för ett objekt där det anpassade formuläret är kopplat för att visa det här avsnittet och redigera fältvärdena. 
       <p>Följande behörigheter är tillgängliga under <b>Användare med den här åtkomsten till objektet kan visa fältvärden</b>:</p> 
         <ul>
          <li><strong>Visa</strong>: Visa behörigheter för objektet</li>
          <li><p><b>Begränsad redigering</b>: (Endast tillgängligt om objektet är ett projekt, en aktivitet, ett problem eller en användare):</p> 
          <p>Tillåter användare att bidra till objektet om det är ett projekt, en uppgift eller ett problem.</p>
          <p>Tillåter användare att redigera profilen eller äger profilbehörigheten till objektet om det är en användare.</p></li> 
          <li><b>Redigera</b>: Hantera behörigheter för objektet </li> 
          <li><b>Endast administratör</b>: Åtkomstnivå för systemadministratör</li> 
         </ul> </li> 
        <p>Följande behörigheter är tillgängliga under <b>Användare med den här åtkomsten till objektet kan redigera fältvärden</b>: </p> 
         <ul> 
          <li> <p><b>Begränsad redigering</b>: (Endast tillgängligt om objektet är ett projekt, en aktivitet, ett problem eller en användare):</p> 
           <p>Om objektet är ett projekt, en uppgift eller ett problem, ger den här behörigheten användarna möjlighet att bidra till objektet</p>
          <p>Om objektet är en användare, ger den här behörigheten användare behörighet att redigera profilen eller äga profilbehörigheten till objektet.</p> 
          <li><b>Redigera</b>: Hantera behörigheter för objektet </li> 
          <li><b>Endast administratör</b>: Åtkomstnivå för systemadministratör</li> 
         </ul> </li> 
       </ul> 
       <p>Mer information om behörigheter för objekt finns i <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Översikt över delningsbehörigheter för objekt</a>.</p> 
       <p><b>OBS</b>:  
       <ul> 
       <li> <p>Användare som saknar de behörigheter som du anger här kan inte se anpassade fält och widgetar i avsnittet. </p> <p>Detta gäller även om du visar fältets värden i rapporter eller använder dem i beräknade fält i textlägesrapporter.</p> </li> 
       <li><p>För anpassade formulär för begäran/utfärdande: Om åtkomst till vyn krävs för att se fälten i avsnittsbrytningen, men administratörsåtkomst krävs för att redigera fälten, kommer avsnittet och alla fält inte att vara synliga för icke-administratörer när de fyller i formuläret. När begäran har skapats kan användare med behörigheten Visa visa fälten i avsnittet.</p></li>
       <li> <p>Om du kopplar flera objekttyper till formuläret kan du ändra de visnings- och redigeringsbehörigheter som är tillgängliga i de här stegen. Mer information finns i <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Hur flera objekttyper kan påverka behörigheter för avsnittsbrytningar i ett anpassat formulär</a> i den här artikeln.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Lägg till logik</p></td> 
      <td><p>Använd visningslogik för att ange om avsnittet ska visas i formuläret, baserat på de val som användare gör i anpassade fält med flera val när de fyller i formuläret.</p><p><strong>Obs!</strong> Om alla enskilda fält under en avsnittsbrytning har visningslogik tillämpad på dem och alla är dolda som ett resultat av logiken, döljs hela avsnittet i det anpassade formuläret. Detta inträffar även om visningslogik inte används för avsnittsbrytningen.</p><p>Mer information finns i <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref">Lägga till visningslogik och hoppa över logik med formulärdesignern</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Dra eller lägg till minst ett anpassat fält eller en widget till det nya avsnittet. Detta krävs innan du sparar avsnittet.

1. Klicka på **Klar**.

   >[!TIP]
   >
   >Du kan klicka på **Använd** när som helst medan du skapar ett anpassat formulär för att spara ändringarna och behålla formuläret öppet.

### Hur flera objekttyper kan påverka avsnittsbrytningsbehörigheter {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

Behörigheten för begränsad redigering för anpassade formuläravsnittsbrytningar är bara tillgänglig för objekttyperna Projekt, Aktivitet, Utgåva och Användare.

Om du lägger till en av de andra objekttyperna i formuläret (Portfolio, Program, Dokument, Företag, Faktureringspost, Iteration, Expense eller Grupp) i ett anpassat formulär med en avsnittsbrytning som är konfigurerad med behörigheten Begränsad redigering, uppmanas du att växla till behörigheten Redigera, som är kompatibel med både den objekttypen och de befintliga objekttyperna i formuläret.

>[!INFO]
>
>**Exempel:** I ett anpassat formulär som är associerat med projektobjekttypen konfigureras en avsnittsbrytning med behörigheten Begränsad redigering.
>
>Du lägger till Portfolio-objekttypen i formuläret, vilket innebär att behörighetsalternativet Begränsad redigering inte längre är tillgängligt för avsnittsbrytningen i formuläret.
>
>Ett meddelande på skärmen uppmanar dig att växla till behörigheten Redigera, som är den lägsta behörighetsnivån som är kompatibel med både objekttypen och Portfolio-objekttypen.


## Placera anpassade fält och widgetar i ett anpassat formulär


1. Börja skapa eller redigera ett anpassat formulär, enligt beskrivningen i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Om du vill placera anpassade fält och widgetar på samma rad drar du det ena bredvid det andra tills en linje visas mellan dem.

   >[!NOTE]
   >
   >* Du kan använda knappen **Förhandsgranska** i det övre högra hörnet för att få en uppfattning om hur anpassade fält och widgetar visas i formuläret.
   >* Anpassade fält och widgetar kanske inte alltid visas på samma sätt i formuläret, beroende på hur mycket skärmutrymme som är tillgängligt när användaren visar det. Det tredje fältet i en rad med fält kan t.ex. radbrytas till nästa rad med fält om det vågräta utrymmet är begränsat.

1. (Valfritt) Om du vill placera ett anpassat fält eller en widget ovanför eller under ett annat fält drar du fältet ovanför eller nedanför tills en vågrät blå linje visas mellan objekten.

1. Om du vill flytta ett anpassat fält till ett annat avsnitt i formuläret kan du dra och släppa det på plats eller klicka på ikonen **Flytta till** i fältet och markera det avsnitt som du vill flytta det till.

   ![Flytta fält till ett avsnitt](assets/move-field-to-section.png)

1. Om du vill spara ändringarna klickar du på **Använd**

   eller

   Klicka på **Spara och stäng**.

## Förhandsgranska ett anpassat formulär

1. Börja skapa eller redigera ett anpassat formulär och lägga till fält, vilket beskrivs i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicka på **Förhandsgranska** i det övre högra hörnet för att se hur formuläret kommer att se ut när det används och klicka sedan på **Avsluta förhandsgranskning** för att återgå till att redigera formuläret.

   >[!NOTE]
   >
   >Avancerad logik stöds inte i förhandsgranskningsläget för formulärdesignern.


