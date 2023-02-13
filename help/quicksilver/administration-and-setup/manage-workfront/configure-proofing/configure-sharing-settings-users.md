---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Konfigurera delningsinställningar för användarna
description: Som Adobe Workfront-administratör eller Workfront Proof-administratör kan du konfigurera användarkonton med vilka korrektur kan delas, om användare kan se alla versioner av ett korrektur och när användare får åtkomst till delade objekt.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Konfigurera delningsinställningar för användarna

Som Adobe Workfront-administratör eller Workfront Proof-administratör kan du konfigurera användarkonton med vilka korrektur kan delas, om användare kan se alla versioner av ett korrektur och när användare får åtkomst till delade objekt.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Aktuell plan: Pro eller högre</p> <p>eller</p> <p>Äldre plan: Premium eller Select</p> <p>Mer information om åtkomst till korrektur med olika planer finns i <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Tillgång till korrekturfunktioner i Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Aktuell plan: Arbete eller plan</p> <p>Äldre plan: Valfritt (Du måste ha språkkontroll aktiverat för användaren)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Administratör måste vara markerat i din behörighetsprofil för korrektur. Mer information finns i <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Konfigurera en användares språkkontroll</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Konfigurera delning med andra konton

1. Klicka på huvudmenyn i Workfront ![](assets/main-menu-icon.png)klickar du sedan på Korrektur ![](assets/proofing-in-main-menu.png) för att få tillgång till Workfront Proof.

1. Klicka **Inställningar** > **Kontoinställningar** klickar du på **Inställningar** -fliken.

1. I **Delning** till höger om **Tillåt delning med**, klicka **Inställningar**.

1. I listrutan som visas väljer du ett alternativ som anger om du vill göra korrektur tillgängliga för någon, begränsa delning av dina korrektur till ditt eget konto eller begränsa det till ditt eget konto och eventuella partnerkonton som du samarbetar med.
1. Klicka **Spara.**

## Konfigurera synlighet för alla versioner av ett delat korrektur

1. Klicka på huvudmenyn i Workfront ![](assets/main-menu-icon.png)klickar du sedan på Korrektur ![](assets/proofing-in-main-menu.png) för att få tillgång till Workfront Proof.

1. Klicka **Inställningar** > **Kontoinställningar** klickar du på **Inställningar** -fliken.

1. I **Delning** till höger om **Mottagarna kan visa alla versioner**, markera **Aktivera** eller **Inaktivera** för att ange om du vill tillåta mottagarna att visa alla versioner av ett korrektur i korrekturläsaren när korrektur-URL är aktiverat.

## Konfigurera korrektursynlighet baserat på arbetsflödesfasaktivitet

Du kan ange när korrektur med ett automatiserat arbetsflöde ska visas för användare som är kopplade till en viss fas.

>[!NOTE]
>
>* Det här alternativet är endast tillgängligt när du använder den fristående Workfront Proof-applikationen. den är inte tillgänglig när du använder en Workfront Proof-instans som är integrerad med Workfront eller vid korrektur i Workfront.
>* Användarna får ett e-postmeddelande om korrekturet först när de kommer in på den scen som användaren är kopplad till, oavsett den här inställningen.
>


Så här konfigurerar du när korrektur med ett automatiserat arbetsflöde visas för användarna:

1. Klicka på huvudmenyn i Workfront ![](assets/main-menu-icon.png)klickar du sedan på Korrektur ![](assets/proofing-in-main-menu.png) för att få tillgång till Workfront Proof.

1. Klicka **Inställningar** > **Kontoinställningar** klickar du på **Inställningar** -fliken.

1. I **Delning** -sektion, aktivera eller inaktivera **Synlighetsbevis baserat på scenaktivering**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Handikappade</strong> (standard)</td> 
      <td>Korrektur visas för användarna när korrekturet skapas.<br><p>Alla användare som är kopplade till en fas i arbetsflödet för korrekturet kan se korrekturet i sökresultaten direkt efter att korrekturet har skapats.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aktiverad</strong> </td> 
      <td> <p>Korrektur visas bara för användare efter den scen de är kopplade till <strong>aktiv.</strong></p> <p><b>ANMÄRKNING</b>:   
        <ul> 
         <li><em style="font-style: normal;">När du har aktiverat det här alternativet är befintliga korrektur fortfarande synliga för användare som kunde visa det när det skapades.</em> </li> 
         <li>När en användare får tillgång till en version av ett korrektur (eftersom den scen som användaren är kopplad till blir aktiv) kan användaren bara se den version där scenen är aktiverad. Om en tidigare version aldrig nått det stadium som användaren är kopplad till kan användaren inte se den versionen av korrekturet.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
