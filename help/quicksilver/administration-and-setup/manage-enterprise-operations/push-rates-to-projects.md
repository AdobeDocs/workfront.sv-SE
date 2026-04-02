---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Justera hastighetsändringar i projekt
description: Ett tariffkort representerar det avtalsavtal med kunden där timtaxor har definierats för de jobbroller som kommer att slutföra arbetet. I ett avgiftskort kan du definiera flera faktureringsfrekvenser per jobbroll, baserat på attribut.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 38441ec5ae6fd8cf5c79f939403d5966c5616c98
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Justera hastighetsändringar i projekt

{{highlighted-preview-article-level}}

När ett tariffkort är kopplat till ett projekt <!--or a staffing plan--> kan tarifferna på tariffkortet fortfarande justeras. Sedan kan du om du vill skicka dessa frekvenser till projekten <!--and staffing plans --> som tariffkortet är kopplat till. Om du inte flyttar de nya tarifferna kommer de ursprungliga priserna att finnas kvar i projektet <!-- or staffing plan-->.

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
1. I dialogrutan [!UICONTROL **Använd för alla projekt**]<!--/staffing plans--> är alla projekt <!--and staffing plans --> som använder det här tariffkortet markerade som standard. Om du inte vill att ett projekt <!--or staffing plan --> ska tillämpa hastighetsändringarna måste du avmarkera det.
1. Klicka på [!UICONTROL **Spara**].

   De nya priserna visas nu i de projekt <!--and staffing plans --> som använder tariffkortet.