---
title: Begränsa åtkomst till ekonomiska data i anpassade fält
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: När du skapar ett anpassat fält kan du definiera valfria inställningar för att begränsa åtkomsten till ekonomiska data.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 5cdaccd9381b02f183b837208eaac4389b0b7a24
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 0%

---


# Begränsa åtkomst till ekonomiska data i anpassade fält

{{highlighted-preview-article-level}}

När du skapar ett anpassat fält kan du definiera valfria inställningar för att begränsa åtkomsten till ekonomiska data. På så sätt kan användare som har vissa behörigheter angivna i åtkomstnivåer se data och de hindras från att se ekonomiska data som de inte ska ha tillgång till.

Mer information om hur du skapar ett anpassat fält finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Mer information om åtkomstnivåer finns i [Översikt över åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md). Mer information om delning och behörigheter finns i [Översikt över delningsbehörigheter för objekt](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Alla</td> 
  </tr>  
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Administrativ åtkomst till anpassade formulär</td> 
  </tr>  
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Begränsa åtkomst till ekonomiska data i ett anpassat fält

1. Skapa ett nytt anpassat formulär eller öppna ett befintligt formulär.

   Mer information finns i [Skapa ett anpassat formulär](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Lägg till ett anpassat fält i formuläret eller markera ett befintligt fält.

   Dessa fälttyper kan begränsas baserat på åtkomst av ekonomiska data:

   * Enkelradig text
   * Stycke
   * Listruta med ett val
   * Listruta för flera val
   * Kryssrutegrupp
   * Alternativknappar
   * Extern sökning
   * Flerval extern sökning
   * Beräknat

1. Välj **Valuta** i fältet **Format**.

   >[!NOTE]
   >
   >För beräkningsfält tillåts alla format. Alla andra fälttyper måste ha formatet **Valuta**, annars är fältet **Ekonomisk behörighetstyp** inte tillgängligt.

1. (Valfritt) Aktivera alternativet **Automatisk behörighet** för enbart beräknade fält om du vill tillåta att de ekonomiska behörigheterna automatiskt kommer från fälten i formeln.

1. Välj ett alternativ för behörighetstypen **Ekonomi**.

   Användarna måste ha den här behörighetstypen innan de kan visa eller redigera det här anpassade fältet i formuläret.

   * **Ingen behörighet krävs:** Alla användare kan se det här fältet
   * **Allmänt:** Användare måste ha behörighet att redigera eller visa Allmän ekonomi
   * **Faktura:** Användare måste ha behörighet att redigera eller visa faktureringsfrekvenser
   * **Kostnad:** Användare måste ha behörighet att redigera eller visa kostnadstariffer

   För beräknade fält:

   * Fältet **Ekonomisk behörighetstyp** är inte tillgängligt för manuell behörighetsinställning om fältet **Automatisk behörighet** är aktiverat.
   * Fälten som används i formeln avgör om behörighetsfältet är aktivt eller inte. Om behörighetsfältet är tomt (och automatiska behörigheter inte är aktiverade) stöder inte formelfälten de ekonomiska behörigheterna.
   * Åtkomst krävs för alla fält i formeln. Om till exempel två fält används i ett beräkningsfält, och ett av dem har faktureringsbehörighet och det andra har kostnadstillstånd, måste användaren ha behörighet att visa både fakturerings- och kostnadstariffer för att kunna se det beräknade värdet.

1. Om du vill spara ändringarna klickar du på **Använd** och fortsätter att skapa formuläret.

   eller

   Klicka på **Spara och stäng**.

## Exempel

Två projekt delas med en användare:

* Användaren har behörighet att redigera alla finansieringsalternativ i det första projektet
* Användaren har behörighet att visa faktureringstariffer och allmän finansiering för det andra projektet

När användaren redigerar det första projektet går det att redigera alla ekonomiska fält i det anpassade formuläret. När användaren redigerar det andra projektet är fälten inställda på **Bill** eller **General** skrivskyddade och fälten inställda på **Cost** visas inte.

När användaren visar projekten i en lista eller rapport:

* Ekonomifält kan visas eller redigeras enligt behörigheter och rapportinställningar
* Ekonomifält är tomma om användaren inte har behörighet att visa dem

När du exporterar projektinformation visas samma värden för ekonomiska fält (eller tomma fält) som i listan.

När du gruppredigerar båda projekten visas fakturerings- och finansfälten som skrivskyddade och kostnadsfälten visar inget.

