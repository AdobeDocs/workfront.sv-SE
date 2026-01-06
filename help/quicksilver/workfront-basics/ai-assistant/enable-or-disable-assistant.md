---
title: Aktivera eller inaktivera AI Assistant
content-type: reference
description: Du kan styra vilka åtkomstnivåer i organisationen som har tillgång till AI Assistant.
author: Becky
feature: Get Started with Workfront
exl-id: eec9f484-e29b-4256-b9ef-b45eb2e78eac
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 0%

---

# Aktivera eller inaktivera AI Assistant

Som Workfront-administratör kan du styra vilka användare i organisationen som har AI Assistant aktiverat. Detta hanteras via åtkomstnivåer.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktivera eller inaktivera AI-assistenten i Workfront

Så här aktiverar du AI-assistenten för en given åtkomstnivå:

{{step-1-to-setup}}

1. Välj **Åtkomstnivåer** i den vänstra navigeringen.
1. Välj önskad åtkomstnivå och klicka sedan på ikonen **Redigera** ![Redigera](assets/edit-icon.png) ovanför listan.
1. Avmarkera kryssrutan **Inaktivera Workfront AI Assistant** i området **Ange ytterligare begränsningar..** i rutan **Redigera åtkomstnivå**.
1. Klicka på **Spara**.
1. Upprepa steg 3-5 för varje åtkomstnivå som du vill aktivera AI Assistant för.



>[!NOTE]
>
>* AI Assistant är inaktiverat som standard för icke-administratörer.
>* Om en icke-administratör interagerar med AI Assistant-ikonen i Workfront, visas AI Assistant-avtalet som uppmanar den icke-administratörer att acceptera villkoren. Om de godkänner avtalet kan de använda AI Assistant även om det är inaktiverat i deras layoutmall.

