---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Förhindra dubblerade användare
description: När du skapar en ny användare i Adobe Workfront kan du inte längre använda en e-postadress som redan används av en annan användare, även om e-postadressen varierar beroende på fall (till exempel JohnDoe@example.com och johndoe@example.com). Om du dessutom vill förbereda dig för framtida autentiseringsförbättringar ser du till att alla användare har unika e-postadresser i en Workfront-instans.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# Förhindra dubblerade användare

När du skapar en ny användare i Adobe Workfront kan du inte längre använda en e-postadress som redan används av en annan användare, även om e-postadressen varierar beroende på fall (till exempel JohnDoe@example.com och johndoe@example.com). Om du dessutom vill förbereda dig för framtida autentiseringsförbättringar ser du till att alla användare har unika e-postadresser i en Workfront-instans.

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
   <td> <p>Du måste vara Workfront-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de har angett ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Skapa användare med unika mejladresser

Från och med version 2019.4 kan du när du skapar en ny användare i Workfront inte längre använda en e-postadress som redan används av en annan användare, även om e-postadressen varierar från fall till fall. Du kan till exempel inte skapa en användare med e-postadressen JohnDoe@example.com om en annan användare har e-postadressen johndoe@example.com.

## Uppdatera e-postadresser till befintliga användare i din Workfront-instans

Som Workfront-administratör måste du uppdatera befintliga användare som har matchande e-postadresser som bara skiljer sig åt från fall till fall.
Så här korrigerar du dubbla e-postadresser i en Workfront-instans:

1. Undersök eventuella duplicerade användare och bestäm vilken användare som inte längre behövs.

   1. Klicka på ikonen **Huvudmeny** ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Användare**. ![](assets/users-icon-in-main-menu.png)

   1. Välj **Alla** på menyn **Filter**.

   1. Välj **Användarinloggning** på menyn **Visa**.

   1. Välj **Ingenting** på menyn **Gruppering**.

   1. Anpassa vyn för användarinloggning.

      1. Klicka på **Visa** > **Anpassa vy**.

      1. Ersätt kolumnen **ID** med kolumnen **E-postadress**.

      1. Byt namn på vyn och spara den.

   1. Skapa en ny gruppering.

      1. Klicka på **Gruppering** > **Ny gruppering**.

      1. Klicka på **Växla till textläge** i det övre högra hörnet på sidan.
      1. Klistra in följande kod för textläge:

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`

   1. Byt namn på grupperingen och spara den.

1. Gör något av följande:

   * (Önskad metod) Lägg till en +-adress till användarens e-postadress för varje ytterligare konto.

     Välj det här alternativet om en enskild användare i organisationen behöver åtkomst till mer än ett användarkonto. Om din e-postleverantör inte stöder plusteringsadress måste du ange ett separat e-postkonto för varje Workfront-konto.

     John Doe kan till exempel ha ett användarkonto för sitt dagliga bruk och ett som ska användas i testsyfte:

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com

   * Ändra domänen till en falsk domän genom att lägga till följande text till e-postadressen:

     `.inactive`

     John Doe kan till exempel ha följande domäner: (Dessa måste vara unika.)

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

     Du kan inte längre logga in på dessa konton eftersom lösenordsåterställning kräver en giltig e-postadress. De här kontona kan bara nås via funktionen Logga in som.

   * Ta bort användare som inte behövs

     >[!IMPORTANT]
     >
     >Välj det här alternativet endast för konton som har skapats av misstag eller för testkonton. Det här alternativet utförs vanligtvis bara för konton med noll eller 1 felaktig inloggning. Konton som har använts regelbundet bör aldrig tas bort.

Om du har användare i en Workfront-instans med matchande e-postadresser som bara skiljer sig åt från fall till fall, kommer Workfront att kontakta dig med ytterligare information och en tidslinje när dessa behöver uppdateras.
