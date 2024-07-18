---
content-type: reference
product-area: reporting
keywords: granskning,spåra,anpassad,fält
navigation-topic: calculate-custom-data-reports
title: "Exempel på beräknat anpassat fält: visa redigeringshistorik för ett fält"
description: Om användare uppdaterar anpassade fält regelbundet och du vill samla in en logg över alla ändringar som gjorts i ett fält samt ett datum när ändringarna inträffar, kan du spara informationen i ett beräknat anpassat fält.
author: Nolan
feature: Reports and Dashboards
exl-id: e233ef28-c95a-42a1-b2eb-448dad5feddb
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 0%

---

# Exempel på beräknat anpassat fält: visa ett fälts redigeringshistorik

Om användare uppdaterar anpassade fält regelbundet och du vill samla in en logg över alla ändringar som gjorts i ett fält samt ett datum när ändringarna inträffar, kan du spara informationen i ett beräknat anpassat fält.

I följande exempel visas hur du skapar beräkningsfältet *Instruktioner för redigeringshistorik* för att fånga alla ändringar som gjorts i ett textfält med en rad som kallas *Instruktioner*.

>[!TIP]
>
>Du kan följa det här exemplet för alla typer av anpassade fält, inte bara enkelradiga textfält.

Detta gör följande: 

* Begränsar fältet *Instruktioner, Redigera historik* till de senaste 2 000 tecknen för att ligga inom Workfront-databasgräns.
* Kontrollerar om det aktuella värdet för fältet *Instruktioner* matchar framsidan av värdet *Instruktioner, Redigera historik* . Det förutsätter att det är tomt och om det inte är det gör det följande: 

   * Om de matchar lämnas *Instruktionerna Redigera historik* som de är;
   * Om de inte matchar ersätter den *Instruktioner/redigeringshistorik* med det senaste värdet i fältet *Instruktioner*, följt av aktuellt datum inom parentes, ett lodrätt fält och föregående *Instruktioner/redigeringshistorik* som bevarar föregående värden och datum när de angavs.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-plan*</p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td> <p>Workfront-licens*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Åtkomstnivåkonfigurationer*</strong> </td> 
   <td> <p>Administrativ åtkomst till anpassad Forms</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Objektbehörigheter</strong> </p> </td> 
   <td> <p>Hantera behörigheter i anpassade formulär </p> <p>Mer information finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Dela ett anpassat formulär</a>.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

## Förutsättningar

Om du vill lägga till ett beräkningsfält som visar ett fälts redigeringshistorik i ett anpassat formulär måste du först:

* Skapa det anpassade formuläret
* Lägg till fältet vars historik du vill hämta till det anpassade formuläret

## Visa redigeringshistorik för ett fält

1. Gå till ett anpassat formulär där du vill lägga till beräkningsfältet.

1. Så här skapar du det anpassade textfältet med en rad:

   1. Klicka på **Textfält med en rad**.
   1. Ange en **etikett** för det anpassade fältet, till exempel *Instruktioner*.
   1. Klicka på **Använd**.

1. Välj **Lägg till ett fält** och välj sedan **Beräknat** för att lägga till ett beräknat anpassat fält i formuläret.
1. Ange en **etikett** för det beräknade anpassade fältet, till exempel *Instruktioner, Redigera historik*.

   Det här är det fält som kommer att fånga ändringar som gjorts i det första fältet som du skapade (*Instruktioner*).

1. Klicka på **Spara + Stäng**.
1. Klicka på namnet på formuläret där du har lagt till två fält för att öppna det igen.
1. Klicka på det beräknade anpassade fältet *Instruktioner > Redigera historik* och kopiera sedan och klistra in följande i rutan Beräkning:
1. I fältet **Beräkning** anger du följande beräkning för ditt anpassade fält:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Rekommenderas) Klistra in samma beräkning i fältet **Instruktioner** i beräkningsfältet i formuläret.
1. Se till att  **Text** markeras i fältet **Format** för att formatera det beräknade anpassade fältet som text.

   Det här är standardinställningen.

1. Klicka på **Spara+Stäng**.

   När du kopplar det anpassade formuläret till ett objekt och sedan ändrar informationen i fältet *Instruktioner* visas det senaste värdet i fältet *Instruktioner, Redigera historik, följt av det aktuella datumet inom parentes och ett lodrätt streck. Om ytterligare ändringar görs läggs de till i informationen på samma sätt.

   I ovanstående beräkning kan du ersätta *Instruktioner* med det exakta namnet på det enkelradiga textfält vars historik du vill spåra och *Instruktioner Redigera historik* med det exakta namnet på det beräknade fältet.
