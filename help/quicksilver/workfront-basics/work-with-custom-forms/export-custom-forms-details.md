---
title: Exportera anpassade formulär och objektinformation
description: Exportera anpassade formulär och objektinformation
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1670edf153e57152e51adcfbda052eb74541d931
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 0%

---

# Exportera anpassade formulär och objektinformation

Du kan exportera översikten och den anpassade formulärinformationen från avsnittet Detaljer för ett objekt till en PDF-fil. Du kan sedan skriva ut eller dela PDF med andra användare.

Den här funktionen stöds för följande objekt:

* Projekt
* Uppgifter
* Problem
* Portfolio
* Program

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>Fälten i detaljavsnittet som din Workfront- eller gruppadministratör har tagit bort med en layoutmall visas inte.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-licens*</p> </td> 
   <td> <p>Begär eller högre för problem</p> <p>Granska eller högre för projekt och uppgifter</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong> </td> 
   <td> <p>Visa eller högre för projekt, uppgifter och ärenden</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objektbehörigheter</p> </td> 
   <td> <p>Visa eller högre behörigheter för det projekt, den uppgift eller det problem vars formulär du vill exportera</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar måste du ha följande:

1. Skapa ett anpassat formulär för ett specifikt objekt som du vill exportera det från.
1. Låt det anpassade formuläret vara kopplat till objektet

   eller

   Ha rätt åtkomst för att bifoga ett anpassat formulär och redigera informationen i formuläret.

Mer information om hur du skapar anpassade formulär finns i [Skapa eller redigera ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

Mer information om hur du bifogar formulär till objekt finns i [Lägga till ett anpassat formulär i ett objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Exportera information i detaljavsnittet

Att exportera information från detaljavsnittet för ett objekt är identiskt för alla objekt där det stöds.

1. Gå till ett projekt, en uppgift, en portfölj, ett program eller ett problem som du har minst behörigheten Visa.
1. Klicka på **Detaljer** på den vänstra panelen, som **Uppgiftsinformation**.
1. (Valfritt) Om det inte finns något anpassat formulär kopplat till objektet börjar du skriva namnet på ett anpassat formulär i **Lägg till anpassat formulärfält** klickar du på den när den visas i listan.

   Du kan lägga till upp till 10 formulär.

1. (Valfritt) Uppdatera informationen i detaljavsnittet och klicka sedan på **Spara ändringar**.
1. Klicka på **Exportera** nedrullningsbar meny i det övre högra hörnet väljer **Översikt** eller de formulär du vill exportera och klicka sedan på **Exportera**.

   Du kan också välja **Markera alla** om du vill exportera området Översikt och alla anpassade formulär.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >Följande scenarier kan finnas:
   >
   >   
   >   
   >   * När gruppadministratören eller Workfront-administratören avmarkerar alla fält i översiktsområdet och objektet har anpassade formulär bifogade, visas inte översiktsavsnittet.
   >   * När gruppadministratören eller Workfront-administratören avmarkerar alla fält i området Översikt och objektet inte har några anpassade formulär bifogade visas inte listrutan Exportera.
   >   * När objektet inte har några anpassade formulär kan du bara exportera området Översikt.
   >   * Anpassade fält som ligger bakom logik och inte är synliga i formuläret exporteras inte. Mer information om hur du lägger till logik i ett anpassat formulär finns i [Lägga till visningslogik och hoppa över logik i ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md).


   En PDF-fil skapas och hämtas till din dator. Filen PDF innehåller följande information:

   * Namnet på objektet som formuläret är kopplat till
   * Namnet på den användare som exporterade PDF
   * Datum och tid då PDF producerades
   * Namnet på de formulär som du har exporterat
   * Information från de fält som fyllts i i formuläret
