---
title: Bevilja användare administrativ åtkomst till vissa områden
description: Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att ge användare med en avtalslicens administrativ åtkomst till vissa delar av systemet.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 85399542ce8e92de6da5a1de0960194e72958987
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Ge användarna administrativ åtkomst till vissa områden

<!--Linked in several places, do not rename or change URL.-->

Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att ge användare med en Standard- eller Plan-licens administrativ åtkomst till vissa delar av systemet.

>[!NOTE]
>
>Detta skiljer sig från att ge en användare fullständig administrativ åtkomst till Workfront, vilket förklaras i [Bevilja en användare fullständig administrativ åtkomst](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md). &#x200B;

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
   <td>   <p>Standard</p>
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

## Ge användare av Standard eller Plan administrativ åtkomst till vissa delar av Workfront

>[!IMPORTANT]
>
>Vi rekommenderar att du låter de inbyggda åtkomstnivåerna vara oförändrade så att du kan referera till dem när du har konfigurerat användarna. Om du vill anpassa en åtkomstnivå kopierar du standardåtkomstnivån och ändrar kopian. (Du kan göra detta för alla åtkomstnivåer förutom systemadministratör och extern användare.)

{{step-1-to-setup}}

1. Klicka på **Åtkomstnivåer** i den vänstra panelen.
1. Klicka på namnet på den åtkomstnivå som du vill använda för att ge användare administrativ åtkomst till vissa delar av Workfront.
1. I avsnittet **Tillåt administrativ åtkomst för** markerar du kryssrutorna för att ge nödvändig administrativ åtkomst.

   Med dessa alternativ kan du tilldela följande funktioner:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Godkännandeprocesser</td> 
      <td><p>Skapa och hantera godkännandeprocesser som kan användas i hela systemet och för specifika grupper.</p><p>Utan den här åtkomsten kan användare bara skapa ad hoc-godkännandeprocesser för objekt som de har åtkomst till att hantera.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Företag</td> 
      <td><p>Lägga till nya och redigera befintliga företag i Workfront</p>
      <p>Utan den här åtkomsten kan användare bara visa befintliga företag.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Egna formulär</td> 
      <td><p>Skapa och redigera (lägg till, redigera och ta bort fält) anpassade formulär inom gruppen.</p><p>Utan den här åtkomsten kan användare bara bifoga befintliga formulär till objekt där de har åtkomst att bidra eller hantera.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Växelkurser</td> 
      <td> <p>Lägg till ny valuta i Workfront.</p> <p>Utan den här åtkomsten kan användaren bara lägga till en befintlig valuta i ett projekt som han/hon skapar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Utgifter</td> 
      <td><p>Visa alla utgifter för objekt i Workfront.</p><p>Detta gör att användaren inte kan skapa nya utgiftstyper.</p><p>Utan den här åtkomsten kan användaren bara visa följande:</p>
       <ul>
        <li>Utgifter för projekt, uppgifter eller ärenden som de hanterar</li>
        <li>Deras egna utgifter</li>
        <li>Utgifter för underordnade</li>
       </ul></td> 
     </tr>
     <tr> 
      <td role="rowheader">Milstolpar i min grupp</td> 
      <td>Visa alla milstolpesökvägar i systemet under menyn Milstolpbanor i Konfigurera. Användare kan också redigera eller ta bort alla milstolpbanor som tillhör någon av deras grupper. Användare kan inte hantera (redigera eller ta bort) de milstolpbanor som inte är tilldelade någon av deras grupper.<br><p>Utan den här åtkomsten kan användare bara visa befintliga milstolpbanor och använda dem i projekt som de har tillgång till för att hantera.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Påminnelsemeddelanden</td> 
      <td>Skapa och hantera påminnelsemeddelanden i Workfront.<br>Utan den här åtkomsten begränsas användarna till att ta emot och visa meddelanden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tidrapporter och timmar</td> 
      <td> <p>Låter användare visa alla timmar och tidrapporter i Workfront.</p> <p>När det här alternativet är inaktiverat kan användare bara visa timmar på:</p> 
       <ul> 
        <li>Projekt, uppgifter eller problem som de hanterar</li> 
        <li>Deras egen tidrapport</li> 
        <li>En tidrapport med någon som rapporterar till dem</li> 
        <li>En tidrapport som de godkänner</li> 
       </ul> <p><b>OBS</b>:  <p>Vare sig det här alternativet är aktiverat eller inaktiverat kan gruppadministratörer skapa tidrapportprofiler för de grupper och undergrupper som de hanterar och tilldela dem till gruppmedlemmar vars användarprofiler de har tillgång till för redigering.</p> <p>Om du aktiverar det här alternativet kan det ge för mycket åtkomst för vissa gruppadministratörer eftersom de kan visa de tidrapporter som genereras av tidrapportprofiler (och timmar) för alla användare i systemet, inte bara för dem i de grupper de administrerar. Du kan inaktivera det här alternativet för gruppadministratörer som inte behöver så här mycket åtkomst.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. När du är klar klickar du på **Spara**.
1. Tilldela den nya åtkomstnivån till en användare enligt beskrivningen i [Lägg till användare](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Du kan tillåta användare att ha administrativ åtkomst till användare. Mer information om hur du ger användare administrativ åtkomst till användare så att de kan hantera användarkonton finns i [Bevilja åtkomst till användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).


<!--     
     <tr> 
      <td role="rowheader">Job roles</td> 
      <td> <p><b>NOTE</b>: In the Preview environment, access to job roles is controlled as an object type in the access level. See <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-job-roles.md">Grant access to job roles</a>.</p>
      <p>With this access, the user is allowed to do the following:</p> 
       <ul> 
        <li>View and edit existing job roles</li> 
        <li>Add new job roles</li> 
        <li>Edit role billing and cost rates</li> 
       </ul> <p><b>IMPORTANT</b>: If you grant a Standard or Plan user administrative access to job roles, the Financial Data access setting Edit Role Billing &amp; Cost Rates is enabled for the user automatically. Later, if you disable administrative access to job roles for the Standard or Plan user, job roles are still visible to the user because the Edit Role Billing &amp; Cost Rates setting is still enabled. If this happens and you need to remove the user's access to view job roles, you need to disable the user's Edit Role Billing &amp; Cost Rates permission setting. For instructions, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>.</p> </td> 
     </tr>
-->
