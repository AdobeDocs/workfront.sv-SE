---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Hantera användar- och rollallokeringstimmar för uppgifter
description: När du tilldelar användare eller roller till en uppgift, tilldelas de ett visst antal timmar för att slutföra uppgiften. Du kan manuellt ändra hur många timmar varje användare eller jobbroll tilldelas när de tilldelas till en uppgift när uppgiftens varaktighetstyp är Enkel.
author: Alina
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: ad5d6bfda24119076df8336ed291c0ba63e2c88a
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# Hantera användar- och rollallokeringstimmar för uppgifter

{{highlighted-preview}}

När du tilldelar användare eller roller till en uppgift, tilldelas de ett visst antal timmar för att slutföra uppgiften. Du kan manuellt ändra hur många timmar varje användare eller jobbroll tilldelas när de tilldelas till en uppgift när uppgiftens varaktighetstyp är Enkel.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute eller högre behörigheter för aktiviteten</p> <p>Redigera behörigheter för att uppdatera allokeringstimmar i rutan Redigera uppgift</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Överväganden för att ändra allokeringstimmar för en aktivitet

>[!IMPORTANT]
>
>När du har ändrat allokeringarna för varje tilldelning för uppgifter manuellt kan aktiviteternas planerade timmar uppdateras i enlighet med detta. Mer information finns i avsnittet [Uppdatera planerade timmar för aktiviteter vid hantering av användarallokeringar](../../../manage-work/tasks/task-information/planned-hours.md#update) i artikeln [Översikt över planerade timmar](../../../manage-work/tasks/task-information/planned-hours.md).

* Det totala antalet timmar som tilldelas enskilda resurser som tilldelats till aktiviteten representerar aktivitetens planerade timmar.
* Om det finns en användar- eller rolltilldelning för en aktivitet, matchar antalet timmar som tilldelats användaren eller rollen aktivitetens planerade timmar.
* När det gäller flera tilldelningar tilldelas varje användare eller jobbroll som standard ett lika stort antal timmar att arbeta med uppgiften, om uppgiftens varaktighetstyp är Enkel. Mer information finns i följande artiklar:

   * [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Översikt över varaktighetstyp: Enkel](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* När aktiviteten har en enkel varaktighetstyp kan du manuellt ändra antalet allokerade timmar för varje användare eller jobbroll för att ange att en del av uppgiftstilldelningarna kan ha mer tid att arbeta med en uppgift än andra.
* Du kan inte ändra antalet timmar som tilldelats team som tilldelats aktiviteter.
* Du kan inte ändra användar- eller jobbrollallokeringen manuellt för utgåvor.
* Du kan också hantera dagliga, veckovisa eller månadsvisa tilldelningar av användare till uppgifter eller ärenden med hjälp av Utjämning av arbetsbelastning. Mer information finns i [Hantera användarallokeringar i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Ändra användar- eller rollallokeringstimmar för en uppgift

1. Gå till en uppgift vars tilldelningar du vill ändra allokeringstimmar för.
1. Klicka på **Mer** meny ![](assets/qs-more-icon-on-an-object.png) bredvid namnet på uppgiften och klicka sedan på **Redigera** sedan **Uppdrag**.

   eller

   Klicka på **Uppdrag** i uppgiftshuvudet och klicka sedan **Avancerat**.

1. Se till att **Varaktighetstyp** för uppgiften är **Enkel**.
1. Ändra **Allokeringar** för varje tilldelad uppgift. Detta är övergripande allokeringar för varje tilldelning för den här aktiviteten, under hela aktivitetens varaktighet. Detta kan även uppdatera aktivitetens totala planerade timmar.

   Exempelbild i produktionsmiljön:
   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

   <span class="preview">Exempelbild i förhandsvisningsmiljön:</span>
   ![Ändra allokeringar](assets/advanced-assignments-duration-type-allocations.png)

1. Klicka **Spara**.
