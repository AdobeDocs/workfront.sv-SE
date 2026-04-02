---
content-type: overview
product-area: projects
navigation-topic: financials
title: Ställ in en jobbroll för fakturering
description: Med Workfront kan du fakturera en användare med en annan jobbroll än den primära rollen. Detta är användbart när en person tillfälligt utför arbete som ska faktureras till en annan avgift.
author: Lisa
feature: Work Management
source-git-commit: d92908d358ca53ae9d443fd76556e3e8b273e3cb
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Ställ in en jobbroll för fakturering

{{highlighted-preview-article-level}}

Med Workfront kan du fakturera en användare med en annan jobbroll än den primära rollen. Detta är användbart när en person tillfälligt utför arbete som ska faktureras till en annan avgift.

Du kan tilldela en jobbroll för fakturering på två sätt:

* På projektnivå: Använd detta när personen ska faktureras under samma jobbroll för hela projektet.
* På tilldelningsnivå: Använd det här alternativet när du vill fakturera olika för specifika uppgifter.

>[!NOTE]
>
>* En jobbroll för fakturering gäller endast personer (användare). Det gäller inte allmänna jobbroller eller platshållare.
>* Om du lägger till en jobbroll för fakturering påverkas endast faktureringstakten, inte kostnaden.
>* Fakturering på uppdragsnivå har alltid företräde framför fakturering på projektnivå.

Mer information finns i [Översikt över intäkt- och kostnadshierarkin](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) och [Skapa avancerade tilldelningar](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Arbetsflöde Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> Redigera åtkomst till tariffkort</td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Hantera behörigheter för projektet </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tilldela en jobbroll för fakturering på projektnivå

När du skapar en jobbroll för fakturering av ett projekt:

* Faktureringsrollen gäller för alla aktiviteter och tilldelningar i projektet för den användaren.
* Fakturering använder den valda jobbrollens faktureringsfrekvens, men kostnaden följer ändå användarens primära roll.

Så här tilldelar du en jobbroll för fakturering på projektnivå:

1. Öppna ett projekt.
1. Klicka på **Resurs för fakturering** i den vänstra panelen.
1. Välj fliken **Jobbroll för fakturering** om den inte redan visas.
1. Klicka på **Lägg till > Lägg till jobbroll för fakturering**.
1. Välj **Användare** i rutan **Lägg till jobbroll för fakturering**.
1. Välj den **jobbroll** som ska användas som jobbroll för fakturering av den här användaren i det här projektet.
1. (Valfritt) Klicka på **Lägg till jobbroll** för att definiera giltighetsdatum för jobbrollen för fakturering. Ange datumen **Start** och **End** för jobbrollen.

[Lägg till jobbroll för fakturering på projektnivå](assets/jrfb-project-level.png)

1. Klicka på **Lägg till jobbroll** igen om du vill ange ytterligare faktureringsroller för olika tidsperioder.
1. Klicka på **Spara**.

### Exempel på projektnivå

>[!BEGINSHADEBOX]

Johns primära roll är Designer 1. Projektet kräver en Senior Designer, och John håller på att fylla i.

Jobbrollen för fakturering skulle vara **Senior Designer** på projektnivå.

Resultat:

* Faktureringsintäkterna är den högsta Designer-räntan
* Kostnaden är Designer 1 - kostnad (John&#39;s actual cost rate)

>[!ENDSHADEBOX]

## Tilldela en jobbroll för fakturering på tilldelningsnivå

När du lägger till en jobbroll för fakturering av ett uppdrag åsidosätter inställningen en faktureringsroll på projektnivå endast för det specifika uppdraget.

Så här tilldelar du en jobbroll för fakturering på tilldelningsnivå:

1. Öppna ett projekt och leta upp uppgiften.
1. Gå till aktivitetens **avancerade tilldelningar**.

   Mer information finns i [Skapa avancerade uppdrag](/help/quicksilver/manage-work/tasks/assign-tasks/create-advanced-assignments.md).

1. Leta reda på kolumnen **Jobbroll för fakturering** i rutnätet för aktivitetstilldelning.
1. Välj en jobbroll för varje tilldelning där du vill ha olika fakturering.

   >[!NOTE]
   >
   >Om en jobbroll för fakturering har tilldelats på projektnivå visas den i tilldelningen. Du kan klicka i fältet **Jobbroll för fakturering** och välja en annan jobbroll att använda för tilldelningen.
   >Informationsikonen meddelar dig om en jobbroll för fakturering har definierats på projekt- eller tilldelningsnivån.

   ![Jobbroll för fakturering av en tilldelning](assets/jrfb-assignment-level.png)

### Exempel på tilldelningsnivå

>[!BEGINSHADEBOX]

Johns primära roll är Designer 1. Han faktureras som Senior Designer på projektnivå, men det finns en särskild uppgift som kräver Designer faktureringsränta.

Du ställer bara in Jobbrollen för fakturering på Designer för det uppdraget.

Resultat:

* John&#39;s övriga uppgifter räknas som Senior Designer
* Den här aktiviteten räknas som Designer Principal
* Kostnad återstår för Designer 1

>[!ENDSHADEBOX]
