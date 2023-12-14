---
title: Bevilja åtkomst för användare
description: Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till andra användare i Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5e87cad4-4a5d-4cb2-848f-7c97ff11d0e8
source-git-commit: 3c5bcb85080a882a8b69bffcd01563a0479f98a5
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---


# Bevilja åtkomst för användare

Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att definiera en användares åtkomst till andra användare i Workfront, vilket förklaras i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Åtkomstkrav

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
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Konfigurera åtkomst för användare

Du kan hantera vilken information användare kan visa och redigera för andra användare med en standardåtkomstnivå eller en anpassad åtkomstnivå som du skapar. Användare med standardlicenser för Planera och Arbeta kan visa kontaktinformation för andra användare. Alla följande användare kan skapa och redigera andra användare:

* En Workfront-administratör.

  Mer information finns i [Bevilja användaren fullständig administrativ åtkomst](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

* En användare med en standardplanlicens som även har åtkomst till användare, vilket förklaras i den här artikeln.

  Användare som är begränsade att bara se användare från sitt företag eller det primära företaget har tillgång till att redigera endast de användare som de kan se. Mer information finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* En användare med en standardplanlicens som också är angiven som hanterare för en annan användare.

  Användare som har behörighet att redigera för användare på åtkomstnivå kan hantera användare som rapporterar till dem. Mer information om hur du hanterar en användare finns i [Visa organisationsschemat](../../../people-teams-and-groups/work-directly-with-others/view-the-org-chart.md).

* En användare med en standardplanlicens som har skapat en användare kan inaktivera, ta bort eller redigera användaren som han/hon skapade. Mer information om hur du skapar nya användare finns i [Lägg till användare](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Konfigurera användaråtkomst för att redigera användare med en anpassad åtkomstnivå

1. Börja skapa eller redigera åtkomstnivån enligt beskrivningen i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Så här ändrar du möjligheten för användare med en plan- eller arbetslicens att visa profiler för andra användare:

   1. Klicka på kugghjulsikonen ![](assets/gear-icon-settings.png) på **Visa** till höger om **Användare**.

   1. Inaktivera **Visa kontaktinformation** klickar du sedan på X för att stänga **Finjustera inställningarna** box.

1. Klicka på kugghjulsikonen om du vill ändra möjligheten för användare med planlicens att redigera andra användare ![](assets/gear-icon-settings.png) på **Redigera** till höger om **Användare** väljer du sedan de funktioner du vill tilldela:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Skapa</strong> </td> 
      <td> <p>Tillåter användare att skapa användare.<br>Det här alternativet är aktiverat som standard.</p> 
      &lt;!—
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Kontrollera att den här ändringen görs innan du raderar dessa två anteckningar. Den 29 mars 2019 säger req doc att detta beror på undersökningsresultaten.</p>

       &lt;p>&lt;b>Obs&lt;/b>! Detta är inte tillgängligt om din organisation har anslutit sig till Adobe Admin Console. Kontakta nätverks- eller IT-administratören om du behöver mer information.&lt;/p>
       —>  &lt;/td>
   </tr> 
     <tr> 
      <td role="rowheader"><strong>Ta bort</strong> </td> 
      <td> <p> Tillåter användare att ta bort de användare som de själva har skapat.<br>Det här alternativet är aktiverat som standard.</p> <p><b>ANMÄRKNING</b>: Detta är inte tillgängligt om din organisation har anslutit sig till Adobe Admin Console. Kontakta nätverks- eller IT-administratören om du behöver mer information.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Användaradministratör (alla användare)</strong> </td> 
      <td> <p>Tillåter användare att göra följande för alla användare i Workfront:</p> 
       <ul> 
        <li>Redigera, ta bort eller inaktivera användaren</li> 
        <li>Logga in som användare</li> 
        <li>Återställ användarens lösenord</li> 
       </ul> <p>Det här alternativet är inaktiverat som standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Användaradministratör (gruppanvändare)</strong> </td> 
      <td> <p>Tillåter användare att göra följande för alla användare i en grupp som de administrerar: 
        <ul>
         <li><p>Redigera, ta bort eller inaktivera användaren</p></li>
         <li>Logga in som användare</li>
         <li><p>Återställ användarens lösenord</p><p><b>ANMÄRKNING</b>: En gruppadministratör kan inte logga in som eller återställa lösenordet för en Workfront-administratör.</p></li>
        </ul><p>Det här alternativet är inaktiverat som standard.</p></p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Om du inte vill ge gruppadministratörer åtkomst till alla medlemmar i de grupper som de administrerar kan du inaktivera båda alternativen för användaradministratörer ovan. Gruppadministratörer kan fortfarande komma åt gruppmedlemmar som de lägger till i Workfront eller som rapporterar till dem i Workfront.

1. (Valfritt) Om du vill konfigurera åtkomstinställningar för andra objekt och områden på den åtkomstnivå du arbetar med ska du fortsätta med någon av artiklarna i [Konfigurera åtkomst till Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), till exempel [Bevilja åtkomst till uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) och [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. När du är klar klickar du **Spara**.

## Tillgång till användare per licenstyp

Mer information om vad användare på varje åtkomstnivå kan göra med användare finns i avsnittet [Användare](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#users) i artikeln [Tillgängliga funktioner för varje objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
