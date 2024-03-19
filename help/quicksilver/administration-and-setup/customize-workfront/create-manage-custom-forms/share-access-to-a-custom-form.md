---
title: Dela ett eget formulär
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Du kan konfigurera åtkomst för ett anpassat formulär för att styra vem - person, roll, grupp, team, företag - som kan visa, dela och redigera det.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# Dela ett eget formulär

<span class="preview">Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder eller i produktionsmiljön för kunder som aktiverat snabba versioner.</span>

<span class="preview">Mer information om snabba versioner finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Mer information om den aktuella versionen finns i [Andra utgåvan, kvartal 2024, översikt](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Du kan konfigurera åtkomst för ett anpassat formulär för att styra vem - person, roll, grupp, team, företag - som kan visa, dela och redigera det.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Standard</p>
   <p>eller</p>
   <p>Aktuell: Planera</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Administrativ åtkomst till anpassade formulär</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Tillgång till anpassade formulär {#access-to-custom-forms}

När du skapar ett nytt anpassat formulär och någon kopplar det till ett objekt kan alla användare som är tilldelade till objektet som standard visa och fylla i formuläret. Detta gäller även användare med licenser för begärande och externa användare.

På ett objekt där det anpassade formuläret inte redan är bifogat kan en användare (även om de har åtkomstnivån Planering) inte bifoga det från den anpassade Forms-listrutan såvida inte något av följande är sant:

* Någon delade det anpassade formuläret med användaren eller med deras team, jobbroll, grupp eller företag och beviljade minst behörigheten Visa med Bifoga till anpassade data markerad
* Användaren har en planlicens och deras åtkomstnivå ger administrativ åtkomst till anpassade formulär

## Dela ett eget formulär

I stället för att lämna ett anpassat formulär i standarddelningsläget (beskrivs i [Tillgång till anpassade formulär](#access-to-custom-forms) i den här artikeln) kan du konfigurera specifika åtkomstnivåer för formuläret för vissa användare, jobbroller, grupper, team och företag.

{{step-1-to-setup}}

1. Klicka på i den vänstra panelen **Anpassad Forms**.
1. Markera det anpassade formuläret och klicka sedan på **Dela** <span class="preview">eller ![Delningsikon](assets/share-icon.png).</span>
1. I rutan som visas, under **Ge anpassade formulär åtkomst till** börjar skriva namnet på den användare, det team, den roll, den grupp eller det företag som du vill dela det anpassade formuläret med och trycker sedan på **Retur** när namnet visas.
1. Om du vill justera åtkomsten för användaren, teamet, jobbrollen, gruppen eller företaget som du just lade till klickar du på listrutan till höger om namnet och konfigurerar sedan något av följande tillgängliga alternativ och någon av de avancerade inställningarna:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Se det</td> 
      <td> <p>Möjlighet att visa och fylla i det anpassade formuläret på objekt.</p> <p><b>ANMÄRKNING</b>: För användare med licens för Work, Review och Request är detta det högsta tillgängliga alternativet.</p> <p>Klicka <strong>Avancerade inställningar</strong> för att ange om du vill tillåta följande:</p> 
       <ul> 
        <li><strong>Koppla till anpassade data</strong>: Möjlighet att bifoga det anpassade formuläret till projekt, uppgifter och ärenden som de har tillgång till i Hantera</li> 
        <li> <p><strong>Dela</strong>: Möjlighet att dela det anpassade formuläret med andra i systemet</p> <p>Användare med en licens för Work, Review eller Request kan endast dela anpassade formulär via API:t eller en anpassad formulärrapport. Mer information finns i .</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hantera det</td> 
      <td> <p>Endast tillgängligt för användare med en planlicens. </p> <p>Förutom att kunna lägga till formuläret i objekt som de har tillgång till för redigering kan användarna även redigera det anpassade formuläret fullständigt, inklusive lägga till, redigera och ta bort fält.</p> <p>Klicka <strong>Avancerade inställningar</strong> om du vill tillåta följande:</p> 
       <ul> 
        <li> <p><strong>Koppla till anpassade data</strong>: Möjlighet att bifoga det anpassade formuläret till projekt, uppgifter och ärenden som de har tillgång till i Hantera</p> </li> 
        <li><strong>Ta bort</strong>: Ta bort det anpassade formuläret från systemet</li> 
        <li><strong>Dela</strong>: Dela det anpassade formuläret med andra i systemet</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Upprepa steg 4-5 om du vill lägga till andra namn i listan och konfigurera deras alternativ.
1. (Valfritt) Om du vill begränsa åtkomsten till det anpassade formuläret (på objekt som det är kopplat till) till de som du har angett i föregående steg klickar du på kugghjulsikonen ![](assets/gear-icon-settings-with-dn-arrow.jpg) i det övre högra hörnet av delningsrutan och klicka sedan på **Ta bort systemomfattande åtkomst**.

   Om du ångrar dig kan du klicka **Gör detta synligt för hela systemet** (standardalternativet).

   >[!NOTE]
   >
   >* När du gör ett anpassat formulär synligt i hela systemet tillåter du bara användare att se och fylla i det på objekt som de har tilldelats, inte att bifoga det till andra objekt. Du kan ge möjlighet att bifoga det anpassade formuläret till objekt med alternativet &quot;Bifoga till anpassade data&quot; som förklaras under steg 5.
   >* De flesta organisationer vill säkerställa att alla i systemet kan fylla i ett anpassat formulär när det bifogas till objekt som de arbetar med och visa data i rapporter. Om detta stämmer för din organisation rekommenderar vi att du använder &quot;**Gör detta synligt för hela systemet**.&quot; När alternativet är konfigurerat på det här sättet visas&quot;Synligt system-Wide&quot; i dialogrutan:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Om du är orolig för ett anpassat formulär där användarna kan ange känsliga data när de är kopplade till vissa objekt, begränsar du delning för dessa *objekt* kan vara bättre än att begränsa åtkomsten till själva formuläret.

1. Klicka **Spara**.

## Ta bort åtkomst till anpassade formulär

{{step-1-to-setup}}

1. Klicka på i den vänstra panelen **Anpassad Forms**.
1. Markera det anpassade formuläret och klicka sedan på **Dela** <span class="preview">eller ![Delningsikon](assets/share-icon.png).</span>
1. I den ruta som visas klickar du på X till höger om namnet på den användare, det team, den roll, den grupp eller det företag som du inte längre vill ha särskild åtkomst till formuläret.
1. (Valfritt) Upprepa föregående steg för andra namn som du vill ta bort.
1. Klicka **Spara**.
