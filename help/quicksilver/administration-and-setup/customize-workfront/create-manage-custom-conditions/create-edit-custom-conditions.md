---
title: Skapa eller redigera ett anpassat villkor
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Som Adobe Workfront-administratör kan du skapa eller redigera anpassade villkor för projekt, uppgifter och ärenden som passar din organisations behov.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5c950862-4358-4aab-997b-223972662150
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 0%

---

# Skapa eller redigera ett anpassat villkor

Som Adobe Workfront-administratör kan du skapa eller redigera anpassade villkor för projekt, uppgifter och ärenden som passar din organisations behov.

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
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa eller redigera ett anpassat villkor

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Villkor**.

1. Klicka på fliken för den objekttyp (**Projekt**, **Aktivitet** eller **Problem**) som du vill associera med villkoret.

1. Om du vill skapa ett nytt villkor klickar du på **Lägg till ett nytt villkor**.

   eller

   Om du vill redigera ett befintligt villkor håller du pekaren över villkoret som du vill redigera och klickar sedan på ikonen **Redigera** som visas längst till höger.

   ![Anpassat villkor](assets/custom-condition-edit-nwe.jpg)

1. Konfigurera ditt anpassade tillstånd med följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Villkorsnamn</td> 
      <td>(Obligatoriskt) Ange ett beskrivande namn för villkoret.</td> 
     </tr> 
     <tr> 
      <td>Beskrivning</td> 
      <td>(Valfritt) Skriv en beskrivning av syftet med villkoret för dem som ska använda det.</td> 
     </tr> 
     <tr> 
      <td>Färg</td> 
      <td>(Valfritt) Klicka på färgikonen och välj sedan den färg som du vill använda för villkoret när det visas i projekt, uppgifter eller ärenden. Du kan också skriva ett hexadecimalt tal.</td> 
     </tr> 
     <tr> 
      <td>Liknar med </td> 
      <td><p>(Obligatoriskt, endast för projekt) Klicka på det alternativ i listrutan som bäst beskriver funktionen för det nya villkoret. För ett villkor som heter Spärra bra klickar du på På mål. Detta avgör hur standardvillkoren fungerar. Alla villkor du skapar måste motsvara något av alternativen i listrutan.</p>
      <p>Mer information om standardvillkor finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md" class="MCXref xref">Ange ett anpassat villkor som standard för projekt</a> och <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md" class="MCXref xref">Ange ett anpassat villkor som standard för uppgifter och ärenden</a>.</p>
      <p>Det här alternativet kan inte ändras när du har skapat villkoret.</p></td> 
     </tr> 
     <tr> 
      <td>Nyckel</td> 
      <td><p>(Obligatoriskt) Ange en alfanumerisk förkortning som användarna kan identifiera för ett projektvillkor. För en uppgift eller ett utleverans skriver du en tvåsiffrig numerisk kod från 01 till 99. </p>
      <p>Nyckeln, som används i API:t och kan användas för rapportering, måste vara unik för varje objekt.</p>
      <p>Du kan inte ändra nyckeln för ett villkor när du har sparat villkoret. </p></td> 
     </tr> 
     <tr> 
      <td>Dölj villkor</td> 
      <td><p>(Valfritt) Det här alternativet är tillgängligt för anpassade villkor som du inte längre vill att personer ska använda, men som du vill behålla av historiska skäl. </p>
      <p>Om du döljer ett anpassat villkor som har använts på arbetsobjekt fortsätter det att visas på de arbetsobjekten när du har dolt det. </p></td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Du kan standardisera villkorsterminologi och färger för alla tre objekttyperna. Det gör du genom att kopiera villkorsnamnet och färghexkoden från en flik (Projekt, Aktivitet, Utgåva) till motsvarande villkor på de två andra flikarna.

1. (Valfritt) Dra ikonen ![Flytta](assets/move-icon---dots.png) om det finns ett villkor till en ny plats om du vill ändra ordningen på listan.

   Detta ändrar den ordning i vilken villkoren visas i projekt, uppgifter och ärenden:

   * När en användare redigerar ett projekt

     ![Ändra villkor vid redigering av projekt](assets/change-condition-edit-project.png)

   * När en användare ändrar villkoret för en uppgift eller ett problem på fliken Uppdateringar:

     ![Ändra villkor vid uppdatering av kommentar](assets/change-condition-update-comment.png)

   * När en användare ändrar villkoret för en uppgift eller ett problem i en listvy:

     ![Ändra villkor i listan](assets/change-conditions-list-dropdown-only.png)

1. Klicka på **Spara**.

Du kan ange ditt anpassade villkor som standardvillkor för projekt eller för uppgifter och ärenden. Mer information finns i [Ange ett anpassat villkor som standard för projekt](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md) och [Ange ett anpassat villkor som standard för uppgifter och ärenden](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md).

Mer information om anpassade villkor finns i [Anpassade villkor](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
