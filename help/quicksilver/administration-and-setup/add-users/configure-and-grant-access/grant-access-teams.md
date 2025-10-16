---
title: Bevilja åtkomst för team
description: Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till team i Workfront
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '663'
ht-degree: 0%

---

# Bevilja åtkomst för team

Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till team i Workfront, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurera användaråtkomst för att redigera användare med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicka på kugghjulsikonen ![](assets/gear-icon-settings.png) på knappen **Visa** eller **Redigera** till höger om Team och välj sedan de funktioner du vill ge under **Finjustera dina inställningar**.

   ![finjustera team](assets/fine-tune-teams.png)

   * **Visa**: Om du konfigurerar hur användare med en licens kan visa team kan du ändra något av följande alternativ:

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Visa team som är associerade med mina grupper</td>
         <td>
          <p><b>Aktiverad</b>: När användare söker efter team i ett Team type-ahead-fält kan användarna se de team som är associerade med deras grupper, oavsett om de är teammedlemmar eller inte. </p>
          <p><b>Inaktiverad</b>: När användare söker efter team i ett Team type-ahead-fält kan användarna bara se de team som är associerade med deras grupper där de är teammedlemmar</p><p>Det här alternativet är aktiverat som standard.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">Visa alla team</td>
         <td><p>När det här alternativet är aktiverat och användarna letar efter team i ett Team type-ahead-fält kan användarna visa och välja vilket team som helst.</p><p>Det här alternativet är aktiverat som standard. </p></td>
        </tr>
       </tbody>
      </table>

   * **Redigera**: Om du konfigurerar hur användare med en planlicens och en arbetslicens kan hantera team ändrar du något av följande alternativ:

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Skapa</td>
         <td><p>Tillåter användare med en planlicens eller en arbetslicens att skapa team.</p><p>Det här alternativet är aktiverat som standard.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Ta bort</td>
         <td><p> Tillåter användare med en planlicens att ta bort de team som de har tillgång till för redigering (inte tillgängliga för användare med en arbetslicens).</p><p>Det här alternativet är aktiverat som standard.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Redigera team i grupper som jag hanterar (endast gruppadministratörer)</td>
         <td><p>Tillåter planlicensanvändare som har utsetts till gruppadministratörer att redigera team som är kopplade till de grupper som de hanterar.</p><p>Det här alternativet är aktiverat som standard.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Redigera team som jag är på</td>
         <td><p>Tillåter användare att planera licens eller arbetslicens för att redigera team där de är medlemmar.</p><p>Det här alternativet är inaktiverat som standard.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Visa team som är associerade med mina grupper</td>
         <td>
         <p><b>Aktiverad</b> När användare söker efter team i ett Team type-ahead-fält kan användarna se de team som är associerade med deras grupper, oavsett om de är teammedlemmar eller inte. </p>
         <p><b>Inaktiverad</b>: När användare söker efter team i ett Team type-ahead-fält kan användarna bara se de team som är associerade med deras grupper där de är teammedlemmar</p><p>Det här alternativet är aktiverat som standard.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">Visa alla team</td>
         <td><p>När det här alternativet är aktiverat och användarna letar efter team i ett Team type-ahead-fält kan användarna visa och välja vilket team som helst.</p><p>Det här alternativet är aktiverat som standard. </p></td>
        </tr>
       </tbody>
      </table>



1. Klicka på krysset för att stänga rutan **Finjustera dina inställningar**.
1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med en av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till aktiviteter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) och [Bevilja åtkomst till ekonomiska data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. När du är klar klickar du på **Spara**.

>[!NOTE]
>
>* Följande gäller oavsett åtkomstnivåinställningar:
>
>   * Teamägare kan alltid visa och redigera sina team
>   * Användarna har alltid tillgång till de team de är i
>
>* Konfigurationen av de alternativ som är tillgängliga för både Visa och Redigera (till exempel &quot;Visa team som är kopplade till mina grupper&quot;) behålls om du väljer Visa i stället för Redigera eller Redigera i stället för Visa på en åtkomstnivå.
>

## Åtkomst till team per licenstyp

Mer information om vad användare på varje åtkomstnivå kan göra med problem finns i avsnittet [Team](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) i artikeln [Tillgängliga funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
