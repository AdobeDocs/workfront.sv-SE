---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Anpassade statusvärden i en grupp som har flyttats eller tagits bort
description: I den här artikeln förklaras vad som händer med grupperade anpassade statusvärden när du flyttar eller tar bort en grupp.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Anpassade statusvärden i en grupp som har flyttats eller tagits bort

I den här artikeln förklaras vad som händer med grupperade anpassade statusvärden när du flyttar eller tar bort en grupp.

## Anpassade statusvärden i en grupp som har flyttats

Tänk på följande scenarier som beskriver vad som händer med gruppanpassade statusvärden när du flyttar en grupp till en ny plats under en annan grupp.

Mer information om hur du flyttar en grupp finns i [Flytta en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">När du flyttar en grupp under en annan grupp </td> 
   <td> <p>Alla den flyttade gruppens statusvärden behålls. De läggs inte till i statusvärdena för gruppens nya överordnade grupp.</p> <p>Men den flyttade gruppen ärver låsta statusvärden i gruppen eller grupper som nu är högre upp i hierarkin. Om en administratör låser en status högre i hierarkin ärver den flyttade gruppen den statusen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">När en status i båda grupperna har samma nyckel men olika attribut</td> 
   <td> <p>Anta att två olika undergrupper ärver samma olåsta status från en överordnad grupp. Gruppadministratörerna för de två grupperna kan sedan anpassa statusen för sina grupper på olika sätt.</p> <p>Senare flyttas en av de två grupperna under den andra. Nu har de båda status med samma nyckel, men de har olika attribut i de två grupperna.</p> <p>I det här fallet är något av följande sant:</p> 
    <ul> 
     <li>Om statusen i den nya överordnade gruppen är olåst behåller den flyttade gruppens status sina attribut, som inte påverkas av flyttningen.</li> 
     <li>Om statusen i den nya överordnade gruppen är låst åsidosätter attributen för statusen i den överordnade gruppen statusvärdena i den flyttade gruppen.</li> 
    </ul> <p>Mer information om statusnycklar finns i <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Skapa eller redigera en status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>När en flyttad grupp har statusar som ärvts från den tidigare överordnade gruppen </td> 
   <td> <p>Alla anpassade statusvärden som ärvts från den tidigare överordnade gruppen följer med den flyttade gruppen och blir egna anpassade statusvärden. De är inte längre anslutna till den tidigare överordnade gruppen.</p> 
    <ul> 
     <li>Om den tidigare överordnade gruppen redigerar en låst anpassad status efter flytten, påverkar ändringarna inte den flyttade undergruppens status.</li> 
     <li>Om den tidigare överordnade gruppen låser en anpassad status som låstes upp när gruppen flyttades, är den flyttade undergruppens status inte låst.</li> 
     <li>Den flyttade gruppen kan nu låsa upp lägen som var låsta när den ärvde dem från den tidigare överordnade gruppen.</li> 
    </ul> 
     <p><b>EXEMPEL:</b><p> 
     <p>Olivia, gruppadministratören för marknadsföringsgruppen, skapar två statusar för gruppen. Hon namnger en First Review med nyckeln ABC och låser den. Hon namnger den andra Final Review, med nyckeln XYZ, och låser den inte.</p> 
     <p>Hon skapar också en undergrupp under marknadsföringsgruppen som kallas produktmarknadsföring. För tillfället när den skapas ärver den automatiskt både First Review (Första granskning) och Final Review (Slutgranskning) från marknadsföringsgruppen.</p> 
     <p>Därefter flyttar Olivia produktmarknadsundergruppen under produktgruppen. Både First Review och Final Review följer med produktmarknadsföringsgruppen till den nya platsen under produktgruppen.</p> 
     <p>Även om den första granskningen var låst före flytten kan administratören för produktmarknadsföringsgruppen redigera den nu eftersom den inte längre är en ärvd status som styrs av den överordnade grupp som den kommer från.</p> 
     <p>Den slutliga granskningen är olåst och kan redigeras som vanligt.</p> 
     <p>För marknadsföringsgruppen ändrar Olivia färgerna i First Review (Första granskning) och Final Review (Slutgranskning) och byter namn på dem till First Review (Redigerad) och Final Review-Edited (Slutlig granskning). Hon låser även Final Review-Edited. I gruppen för produktmarknadsföring ändras inte färger och namn för statusvärdena Första granskning och Slutgranskning.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassade statusar i en grupp som har tagits bort

När du tar bort en grupp eller undergrupp tilldelar du om informationen som är kopplad till den, inklusive dess anpassade status, till en annan grupp eller undergrupp. Den borttagna gruppens status läggs till i målgruppens.

Om en av den borttagna gruppens statusar också användes av målgruppen (statusen i båda grupperna har samma nyckel) och målgruppen anpassade statusen på olika sätt, åsidosätter inställningarna för målgruppens version inställningarna inställningarna för den flyttade gruppens version inställningarna.

>[!INFO]
>
>**EXEMPEL:**
>
>Gruppadministratören för grupp A byter namn på en olåst systemnivå för sin grupp. Gruppadministratören för en grupp B byter också namn på den statusen för den här gruppen. Även om statusen har olika namn i de två grupperna har den samma nyckel.
>
>Senare tas grupp A bort och all information om gruppen omfördelas till grupp B.
>
>* Namnet på grupp B-versionen av statusen åsidosätter namnet på grupp A-versionen.
>* Om statusen tillämpades på ett objekt av någon i grupp A innan gruppen togs bort, uppdateras objektets statusnamn till namnet på den status som används av grupp B.
>
>Mer information om nyckeln för en status finns i tabellen i den här artikeln under [Skapa eller redigera en anpassad status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [Skapa eller redigera en status för en grupp](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>Mer information om hur du tar bort en grupp finns i [Ta bort en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
