---
title: Ge användarna administrativ åtkomst till vissa områden
description: Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att ge användare med en avtalslicens administrativ åtkomst till vissa delar av systemet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 0%

---

# Ge användarna administrativ åtkomst till vissa områden

<!--Linked in several places, do not rename or change URL.-->

Som Adobe Workfront-administratör kan du använda en åtkomstnivå för att ge användare med en avtalslicens administrativ åtkomst till vissa delar av systemet.

>[!NOTE]
>
>Detta skiljer sig från att ge en användare fullständig administrativ åtkomst till Workfront, vilket förklaras i [Bevilja användaren fullständig administrativ åtkomst](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md). &#x200B;

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

## Bevilja plananvändare administrativ åtkomst till vissa delar av Workfront

>[!IMPORTANT]
>
>Vi rekommenderar att du låter de inbyggda åtkomstnivåerna vara oförändrade så att du kan referera till dem när du har konfigurerat användarna. Om du vill anpassa en åtkomstnivå kopierar du standardåtkomstnivån och ändrar kopian. (Du kan göra detta för alla åtkomstnivåer förutom systemadministratör och extern användare.)

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka på i den vänstra panelen **Åtkomstnivåer**.
1. Klicka på namnet på den åtkomstnivå som du vill använda för att ge användare administrativ åtkomst till vissa delar av Workfront.
1. I **Tillåt administrativ åtkomst för** markerar du kryssrutor för att ge nödvändig administrativ åtkomst.

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
      <td role="rowheader">Jobbroller</td> 
      <td> <p>Med den här åtkomsten kan användaren göra följande:</p> 
       <ul> 
        <li>Visa och redigera befintliga jobbroller</li> 
        <li>Lägg till nya jobbroller</li> 
        <li>Redigera rollfakturering och kostnadstariffer</li> 
       </ul> <p><b>VIKTIGT</b>: Om du ger en planerare administratörsbehörighet för jobbroller aktiveras inställningen Redigera rollfakturering och kostnadstariffer automatiskt för användaren. Om du senare inaktiverar administrativ åtkomst till jobbroller för planeraren, visas jobbrollerna fortfarande för användaren eftersom inställningen Redigera rollfakturering och kostnadstariffer fortfarande är aktiverad. Om detta inträffar och du måste ta bort användarens åtkomst för att kunna visa jobbroller, måste du inaktivera användarens behörighetsinställning Redigera rollfakturering och kostnadstariffer. Instruktioner finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Bevilja åtkomst till finansiella uppgifter</a>.</p> </td> 
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
      <td> <p>Tillåter användare att visa alla timmar och tidrapporter i Workfront.</p> <p>När det här alternativet är inaktiverat kan användare bara visa timmar på:</p> 
       <ul> 
        <li>Projekt, uppgifter eller problem som de hanterar</li> 
        <li>Deras egen tidrapport</li> 
        <li>En tidrapport med någon som rapporterar till dem</li> 
        <li>En tidrapport som de godkänner</li> 
       </ul> <p><b>ANMÄRKNING</b>:  <p>Vare sig det här alternativet är aktiverat eller inaktiverat kan gruppadministratörer skapa tidrapportprofiler för de grupper och undergrupper som de hanterar och tilldela dem till gruppmedlemmar vars användarprofiler de har tillgång till för redigering.</p> <p>Om du aktiverar det här alternativet kan det ge för mycket åtkomst för vissa gruppadministratörer eftersom de kan visa de tidrapporter som genereras av tidrapportprofiler (och timmar) för alla användare i systemet, inte bara för dem i de grupper de administrerar. Du kan inaktivera det här alternativet för gruppadministratörer som inte behöver så här mycket åtkomst.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. När du är klar klickar du på **Spara**.
1. Tilldela den nya åtkomstnivån till en användare enligt beskrivningen i [Lägg till användare](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Du kan tillåta användare att ha administrativ åtkomst till användare. Mer information om hur du ger användare administrativ åtkomst till användare så att de kan hantera användarkonton finns i [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
