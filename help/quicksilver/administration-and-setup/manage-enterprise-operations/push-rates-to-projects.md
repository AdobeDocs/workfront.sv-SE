---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Justera hastighetsändringar i projekt
description: Ett tariffkort representerar det avtalsavtal med kunden där timtaxor har definierats för de jobbroller som kommer att slutföra arbetet. I ett avgiftskort kan du definiera flera faktureringsfrekvenser per jobbroll, baserat på attribut.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c38e60dd-7fb2-4afc-976a-b0966398c162
source-git-commit: 7686cd33a5c761dc57cb488ea49a4139665949d9
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Justera hastighetsändringar i projekt

När ett tariffkort är kopplat till ett projekt <!--or a staffing plan--> kan tarifferna på tariffkortet fortfarande justeras. Sedan kan du välja att överföra dessa priser till de projekt som tariffkortet är kopplat till. Om ni inte tänjer på de nya priserna ligger de ursprungliga priserna kvar på projektet.
<!-- and staffing plans -->
<!-- or staffing plan -->

Mer information om hur du bifogar ett tariffkort till ett projekt finns i [Koppla ett tariffkort till ett projekt](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td>Arbetsflöde Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till [!UICONTROL Rate Cards]</td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Om du vill redigera ett tariffkort som delas med dig måste du ha behörigheten Hantera för tariffkortet.</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Justera hastighetsändringar i projekt

{{step-1-to-setup}}

1. Klicka på [!UICONTROL **Klassificera kort**] i den vänstra panelen.
1. Klicka på kortnamnet i listan Klassificeringskort.
1. Kontrollera att taxorna är korrekta och redigera eventuella taxor efter behov på skärmen Klassificeringskort > Jobbroller och taxor.
1. Klicka på [!UICONTROL **Push changes**].
1. I dialogrutan [!UICONTROL **Använd för alla projekt**] väljs alla projekt som använder det här tariffkortet som standard. Om du inte vill att ett projekt ska tillämpa hastighetsändringarna måste du avmarkera det.

   <!--/staffing plans-->
   <!--and staffing plans -->
   <!--or staffing plan -->

1. Klicka på [!UICONTROL **Spara**].

   De nya priserna visas nu i de projekt <!--and staffing plans --> som använder tariffkortet.
