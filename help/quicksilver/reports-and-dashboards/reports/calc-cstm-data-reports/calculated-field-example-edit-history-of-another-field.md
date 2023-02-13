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
source-wordcount: '666'
ht-degree: 0%

---

# Exempel på beräknat anpassat fält: visa redigeringshistorik för ett fält

Om användare uppdaterar anpassade fält regelbundet och du vill samla in en logg över alla ändringar som gjorts i ett fält samt ett datum när ändringarna inträffar, kan du spara informationen i ett beräknat anpassat fält.

I följande exempel visas hur du skapar *Instruktioner Redigera historik* beräknat fält för att fånga alla ändringar som gjorts i ett textfält med en rad som kallas *Instruktioner*.

>[!TIP]
>
>Du kan följa det här exemplet för alla typer av anpassade fält, inte bara enkelradiga textfält.

Detta gör följande: 

* Begränsar *Instruktioner Redigera historik* till de senaste 2000 tecknen för att ligga inom databasgränsen för Workfront.
* Kontrollerar om det aktuella värdet för *Instruktioner* fältet matchar framsidan av *Instruktioner Redigera historik* värde, den förutsätter att den är tom, och om den inte är det gör den följande: 

   * Om de matchar, lämnar det *Instruktioner Redigera historik* i befintligt skick,
   * Om de inte matchar ersätter det *Instruktioner Redigera historik* med det senaste värdet i *Instruktioner* fält, följt av aktuellt datum inom parentes, ett lodrätt streck och föregående *Instruktioner Redigera historik*, som bevarar tidigare värden och datum när de angavs.

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
   <td><strong>Konfigurationer på åtkomstnivå*</strong> </td> 
   <td> <p>Administrativ åtkomst till anpassad Forms</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Objektbehörigheter</strong> </p> </td> 
   <td> <p>Hantera behörigheter i anpassade formulär </p> <p>Mer information finns i <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Dela ett eget formulär</a>.<br></p> </td> 
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

   1. Klicka **Textfält med en rad**.
   1. Ange en **Etikett** för det anpassade fältet, till exempel *Instruktioner*.
   1. Klicka **Använd**.

1. Välj **Lägg till ett fält** väljer **Beräknat** om du vill lägga till ett beräknat anpassat fält i formuläret.
1. Ange en **Etikett** för det beräknade anpassade fältet, som *Instruktioner Redigera historik*.

   Det här är fältet som kommer att fånga ändringar som gjorts i det första fältet som du skapade (*Instruktioner*).

1. Klicka **Spara + Stäng**.
1. Klicka på namnet på formuläret där du har lagt till två fält för att öppna det igen.
1. Klicka på det beräknade anpassade fältet *Instruktioner Redigera historik,* sedan kopiera och klistra in följande i rutan Beräkning:
1. I **Beräkning** anger du följande beräkning för ditt anpassade fält:

   ```
   LEFT(IF(LEFT({DE:Instructions Edit History},LEN(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})))={DE:Instructions},{DE:Instructions Edit History},CONCAT(IF(ISBLANK({DE:Instructions}),"-",{DE:Instructions})," (",$$NOW,") | ",{DE:Instructions Edit History})),2000)
   ```

1. (Rekommenderas) Klistra in samma beräkning i **Instruktioner** på beräkningsfältet i formuläret.
1. Se till att  **Text** är markerat i **Format** för att formatera det beräknade anpassade fältet som text.

   Detta är standardinställningen.

1. Klicka **Spara+stäng**.

   När du kopplar det anpassade formuläret till ett objekt och sedan ändrar någon informationen i *Instruktioner* i fältet *Instructions Edit History&quot; visas det senaste värdet, följt av aktuellt datum inom parentes och ett vertikalt streck. Om ytterligare ändringar görs läggs de till i informationen på samma sätt.

   I ovanstående beräkning kan du ersätta *Instruktioner* med det exakta namnet på det enkelradiga textfält vars historik du vill spåra, och *Instruktioner Redigera historik* med det exakta namnet på det beräknade fältet.
