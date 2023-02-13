---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Skapa ett korrektur för flera sidor
description: Du kan kombinera flera filer till ett enda flersidigt korrektur. Granskarna kan använda navigeringsverktygen i korrekturläsaren för att bläddra igenom sidorna i ett flersidigt korrektur.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# Skapa ett korrektur för flera sidor

Du kan kombinera flera filer till ett enda flersidigt korrektur. Granskarna kan använda navigeringsverktygen i korrekturläsaren för att bläddra igenom sidorna i ett flersidigt korrektur.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Välj eller Premium</p> <p>Mer information om åtkomst till korrektur med olika planer finns i <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Tillgång till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Valfritt (Du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Behörighetsprofil för korrektur </td> 
   <td>Chef eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till dokument</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Om du vill veta vilken plan, licens eller behörighetsprofil du har kontaktar du Workfront- eller Workfront-administratören.

## Skapa ett korrektur för flera sidor

När det här alternativet är aktiverat är statiska filer och webbplatser tillgängliga i ett enda korrektur. När det här alternativet är inaktiverat genereras alla dokument och webbplatser som individuella korrektur, och du kan överföra upp till 100 filer vid en given tidpunkt.

Så här skapar du ett flersidigt korrektur:

1. Gå till projektet, aktiviteten eller utgåvan där du vill ha korrekturet och klicka sedan på **Dokument** -avsnitt.
1. Klicka **Lägg till ny** > **Korrektur** .
1. Dra och släpp filerna eller bläddra och välj dem i Utforskaren. Du kan överföra upp till 50 filer i taget. Mer information om filbegränsningar finns i [Överväganden](#considerations) i den här artikeln.

   >[!NOTE]
   >
   >Interaktiva filer, inklusive videor och interaktiva webbplatser, kan inte kombineras till ett enda korrektur.

1. Under **Enkelt provtryck**, aktivera alternativet, **Kombinera alla kompatibla filer till ett enda korrektur**.
1. I **Korrekturnamn** anger du ett nytt namn för det kombinerade korrekturet.
1. (Valfritt) I listan över filer som du har överfört ändrar du ordning på filerna genom att dra dem. Filernas ordning är sidordningen för det kombinerade korrekturet.
1. (Valfritt) Om du vill ta bort en enskild fil från sidan Nytt korrektur för du pekaren över filen och klickar på **Papperskorgen** -ikon som visas till höger.

   eller

   Om du vill ta bort alla överförda filer samtidigt klickar du på **Ta bort alla** i listans övre högra hörn.

1. När alla filer har överförts måste du bestämma om du vill konfigurera ett grundläggande korrektur eller ett automatiskt korrektur:

   * Med ett grundläggande korrektur kan du lägga till så många granskare som du vill i ett korrektur, men de är inte ordnade i steg. Alla granskare som du lägger till får tillgång till korrekturet direkt när du har skapat det. Information om hur du konfigurerar ett grundläggande korrektur finns i [Skapa ett avancerat korrektur med ett grundläggande arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Med ett automatiskt korrektur flyttas korrekturet från scen till scen och Adobe Workfront meddelar varje användare när det är deras tur att granska det. om du vill konfigurera ett automatiskt korrektur kan du läsa [Skapa ett avancerat korrektur med ett automatiserat arbetsflöde](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Överväganden {#considerations}

Tänk på följande när du kombinerar filer till ett enda korrektur:

* Du kan överföra upp till 500 separata filer.
* Du kan kombinera statiska filer av olika typer (till exempel PDF, JPG, DOC, PPT, EXC), upp till totalt 2 000 sidor.
* Du kan kombinera statiska webbklipp.
* Du kan kombinera GIF-filer; animerat GIF bearbetas dock som statiska filer.
* Du kan inte kombinera AV-filer och interaktiva webbklipp.
* Provtryckets miniatyrbild hämtas från korrekturens första sida (se [Hantera korrekturinformation i Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* Du kan kontrollera namnen på de filer som kombinerats för att skapa korrekturet på sidan Korrekturinformation. Mer information finns i [Hantera korrekturinformation i Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Om alternativet att hämta originalfilerna är aktiverat på korrekturet kan du hämta alla filer som har kombinerats för att skapa korrekturet som en ZIP-fil. Mer information finns i  [Ladda ned filer som lagras i Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
