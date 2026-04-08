---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Konfigurera AI-samarbetspartners
description: Som Adobe Workfront-administratör kan du konfigurera AI-medarbetare och tilldela dem till projekt och uppgifter.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: 25d5fef46bc8f02e92d778685c2ad6e93439f9ff
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Konfigurera AI-samarbetspartners

{{highlighted-preview-article-level}}

AI-samarbetspartners är ett sätt att införliva AI-agenter i projekt och uppgifter. Du kan konfigurera en AI-medarbetare och sedan tilldela den på samma sätt som en användare.

Du kan till exempel konfigurera en granskare-typ av AI Collaborator med varumärkesriktlinjer och sedan tilldela denne medarbetare att granska ett dokument.

Tillgängliga AI Collaborator-typer är:

* Granskare: Skapa en medarbetare med varumärken <!-- or Adobe Brand Intelligence--> och tilldela sedan medarbetaren som granskare för resurser.

  Mer information finns i [Kom igång med Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

  >[!NOTE]
  >
  >För närvarande är Reviewer den enda tillgängliga typen av AI Collaborator. Fler funktioner för AI Collaborator kommer att vara tillgängliga i framtiden.


## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Standard, Prime eller Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licens</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
  </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar



* Din organisation måste ha ett signerat Adobe Gen AI-avtal till hands.

  Mer information finns i [Signera Adobe Gen AI-avtalet](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) i artikeln AI Assistant i Workfront.
* Du måste ha konfigurerat ett varumärke i Workfront innan du kan använda det för en AI-medarbetare av typen Reviewer.

  Instruktioner finns i [Skapa och hantera varumärken för Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Skapa en ny granskare-typ av AI Collaborator

{{step-1-to-setup}}

1. Klicka på **AI-medarbetare** i den vänstra navigeringen.
1. Klicka på **Ny medarbetare** i skärmens övre högra hörn.
1. Klicka på **Granskare** och sedan på **Fortsätt**.

   >[!NOTE]
   >
   >För närvarande är endast granskartypen tillgänglig. Fler typer av AI Collaborator kommer att vara tillgängliga i framtiden.

1. Ange ett namn för medarbetaren i fältet Medarbetarens namn. Det här namnet visas i listan med tillgängliga tilldelningar för en uppgift.
   <!--1. Select whether the collaborator will use a brand or Adobe Brand Intelligence for its reviews.-->
   <!--1. (Conditional) If the AI Collaborator will use Adobe Brand Intelligence, select the tenant that it will use.-->
1. <!--(Conditional) If the AI Collaborator will use a Brand,-->Välj det varumärke och den varumärkesriktlinje som ska användas.
1. Klicka på **Spara**.

## Hantera AI-samarbetspartners

Du kan redigera, kopiera och ta bort befintliga AI-medarbetare.

{{step-1-to-setup}}

1. Klicka på **AI-medarbetare** i den vänstra navigeringen.
1. (Villkorligt) Om du vill redigera en medarbetare klickar du på namnet på den medarbetare som du vill redigera, gör eventuella ändringar i fönstret Redigera medarbetare och klickar på **Spara**.
1. (Villkorligt) Om du vill kopiera en medarbetare klickar du på ikonen Kopiera ![Kopiera](assets/copy-ai-collaborator.png) på raden i AI-medarbetaren som du vill kopiera, klickar på kopians namn, gör eventuella ändringar i fönstret Redigera medarbetare och klickar på **Spara**.
1. (Villkorligt) Om du vill ta bort en medarbetare klickar du på ikonen Ta bort ![Ta bort](assets/delete-collaborator-icon.png) på raden i den AI-medarbetare som du vill ta bort och sedan på **Ta bort**.
